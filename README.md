# Academy Interactives

Custom HTML/CSS/JS learning objects for Amplitude Academy courses, embedded in Rise 360 via iframe.

**Hosted at:** `https://nlivni-amplitude.github.io/academy-interactives/`

---

## Catalog

| Course | Object | Path | Live URL |
|--------|--------|------|----------|
| Event Segmentation | Metric Toggle | `metric-toggle/` ⚠️ | [metric-toggle](https://nlivni-amplitude.github.io/academy-interactives/metric-toggle/) |
| Event Segmentation | Metrics Panel | `charts/metrics-panel/` ⚠️ | [metrics-panel](https://nlivni-amplitude.github.io/academy-interactives/charts/metrics-panel/) |

⚠️ Legacy path — predates naming convention. Migrate to `es/[name]/` on next major update.

---

## Structure

```
academy-interactives/
  [course-slug]/          ← short course abbreviation (see table below)
    [object-name]/        ← kebab-case interaction type
      index.html          ← self-contained, no build step
  shared/                 ← reusable objects not tied to one course
    [object-name]/
      index.html
```

**Course slugs:**

| Slug | Course |
|------|--------|
| `es` | Event Segmentation |
| `funnels` | Funnels |
| `dash` | Dashboards |
| `aa` | Amplitude Assistant / AI Agents |
| `shared` | Reusable across courses |

**Object names:** lowercase kebab-case describing the interaction (`metric-toggle`, `funnel-builder`). No course prefix in the name — the folder provides that context.

---

## Embed in Rise

```html
<iframe
  src="https://nlivni-amplitude.github.io/academy-interactives/[course-slug]/[object-name]/?v=1"
  width="100%"
  height="900"
  style="border:none; border-radius:8px;">
</iframe>
```

- Keep `width="100%"` — the HTML controls its own `max-width` and centering.
- Adjust `height` to match content height. 900px is a safe default.
- Bump `?v=N` on each update to bypass CDN cache.

---

## Deploying

Push to `main` and the [GitHub Actions workflow](.github/workflows/deploy.yml) deploys automatically (1–2 min).

**From this machine** (SSH not configured for `nlivni-amplitude`):

```bash
# Update existing file
SHA=$(gh api repos/nlivni-amplitude/academy-interactives/contents/[course-slug]/[object-name]/index.html --jq '.sha')

gh api repos/nlivni-amplitude/academy-interactives/contents/[course-slug]/[object-name]/index.html \
  --method PUT \
  --field message="update [object-name]" \
  --field content="$(base64 -i [course-slug]/[object-name]/index.html)" \
  --field sha="$SHA" \
  --jq '.commit.sha'
```

Omit `--field sha` for a new file.

**Token note:** Pushing `index.html` files requires `repo` scope. Modifying `.github/workflows/` requires the `workflow` scope (`gh auth refresh -h github.com --scopes workflow`).

**Collaborators** with write access can push via `git push` directly — no special setup needed.
