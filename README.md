# Academy Interactives

Custom HTML/CSS/JS learning objects for Amplitude Academy courses, embedded in Rise 360 via iframe.

**Hosted at:** `https://nlivni-amplitude.github.io/academy-interactives/`

---

## Catalog

| Course | Object | Description | Path | Live URL |
|--------|--------|-------------|------|----------|
| Event Segmentation | Metric Toggle | Toggle between metric types (count, unique users, sum, avg) and see how the chart updates | `chart_event_segmentation/metric-toggle/` | [link](https://nlivni-amplitude.github.io/academy-interactives/chart_event_segmentation/metric-toggle/) |
| Event Segmentation | Metrics Panel | Annotated diagram of the Amplitude metrics panel with labeled UI components | `chart_event_segmentation/metrics-panel/` | [link](https://nlivni-amplitude.github.io/academy-interactives/chart_event_segmentation/metrics-panel/) |
| Agent Analytics | Two Users Comparison | Side-by-side event timeline showing identical events producing opposite outcomes (task completed vs. hallucination) | `aa/two-users-comparison/` | [link](https://nlivni-amplitude.github.io/academy-interactives/aa/two-users-comparison/) |
| Agent Analytics | Three-Layer Stack | Positioning diagram showing LLM Observability, Agent Analytics, and Product Analytics as connected layers | `aa/three-layer-stack/` | [link](https://nlivni-amplitude.github.io/academy-interactives/aa/three-layer-stack/) |
| Agent Analytics | Three-Step Process | Clickable L→R diagram showing See it → Judge it → Tie it to outcomes | `aa/three-step-process/` | [link](https://nlivni-amplitude.github.io/academy-interactives/aa/three-step-process/) |
| Session Replay | Frustration Signals | 2×2 card grid of the four frustration signal types: rage click, dead click, error click, form abandonment | `sr/frustration-signals/` | [link](https://nlivni-amplitude.github.io/academy-interactives/sr/frustration-signals/) |
| Session Replay | Agent Flow | 3-step flow diagram: Ask → Analyze → Surface — how Session Replay Agent processes sessions | `sr/agent-flow/` | [link](https://nlivni-amplitude.github.io/academy-interactives/sr/agent-flow/) |
| Session Replay | Session List Tour | Clickable labeled graphic over the real All Replays screenshot: 4 hotspots (Experience Analytics, session list, filter panel, session card) | `sr/session-list/` | [link](https://nlivni-amplitude.github.io/academy-interactives/sr/session-list/) |
| Session Replay | Cart Rage-Click Replay | Autoplay/loop video (pausable) of a real AmpliStore checkout session: dead click, rage click, then abandon | `sr/cart-rage-click/` | [link](https://nlivni-amplitude.github.io/academy-interactives/sr/cart-rage-click/) |
| Session Replay | Agent Run | Autoplay/loop video (pausable) of the Session Replay Agent analyzing checkout drop-off and surfacing sessions | `sr/agent-run/` | [link](https://nlivni-amplitude.github.io/academy-interactives/sr/agent-run/) |
| Blog | Kirkpatrick Levels Tabs | Tabbed object showing Kirkpatrick's four evaluation levels applied to an AI agent (Smile Sheet blog post) | `blog/agent-analytics-kirkpatrick-levels-tabs/` | [link](https://nlivni-amplitude.github.io/academy-interactives/blog/agent-analytics-kirkpatrick-levels-tabs/) |
| Dashboards | Agent Setup Steps | Clickable 5-step stepper walking through creating a Dashboard Agent: start, pick template + dashboard, focus instruction, delivery, run | `dash/agent-setup-steps/` | [link](https://nlivni-amplitude.github.io/academy-interactives/dash/agent-setup-steps/) |
| Statsig | Selection Bias Demo | Split 12 users by targeting vs. coin flip and see why only random assignment makes a fair comparison | `statsig/statsig-101/01_the-loop_selection-bias-demo/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/statsig-101/01_the-loop_selection-bias-demo/) |
| Statsig | Hashing Lottery | Assign 8 users a fixed 0-99 ticket number and evaluate a 30% gate against it, twice, to show deterministic hashing | `statsig/statsig-101/02_ship-safely_hashing-lottery/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/statsig-101/02_ship-safely_hashing-lottery/) |
| Statsig | Identifier Flip Cards | Two flip cards contrasting logged-in user ID vs. device-level ID and the pre-login gate trap | `statsig/statsig-101/02_ship-safely_identifier-flip/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/statsig-101/02_ship-safely_identifier-flip/) |
| Statsig | P-Value Simulator | Run 100 simulated null experiments and see how often noise alone produces a 4-point gap | `statsig/statsig-101/03_stats-lab_pvalue-simulator/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/statsig-101/03_stats-lab_pvalue-simulator/) |
| Statsig | Peeking Simulator | Track a 14-day null experiment's daily gap on a line chart to show how peeking crosses "significant" by chance | `statsig/statsig-101/03_stats-lab_peeking-simulator/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/statsig-101/03_stats-lab_peeking-simulator/) |
| Statsig | Scorecard Basics | Three expandable cards on participation vs. assignment, bake windows, and the CI-zero rule | `statsig/statsig-101/04_reading-pulse_scorecard-basics/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/statsig-101/04_reading-pulse_scorecard-basics/) |
| Statsig | Day-1 Traps Flip Cards | Four flip cards on early-read mistakes: too-early calls, sample ratio mismatch, guardrail blind spots, novelty effect | `statsig/statsig-101/05_day1-traps_flip-cards/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/statsig-101/05_day1-traps_flip-cards/) |

---

## Structure

```
academy-interactives/
  [chart-type]/           ← chart or feature the object teaches (see table below)
    [object-name]/        ← kebab-case interaction type
      index.html          ← self-contained, no build step
  shared/                 ← reusable objects not tied to one chart type
    [object-name]/
      index.html
```

**Chart type folders:**

| Folder | Content |
|--------|---------|
| `chart_event_segmentation` | Event Segmentation chart interactives |
| `chart_funnel` | Funnel chart interactives |
| `chart_retention` | Retention chart interactives |
| `shared` | Reusable across chart types |

**Why chart type, not course slug:** Chart type is always known at build time. Course slugs depend on Skilljar course setup, which often doesn't exist yet for new courses.

**Object names:** lowercase kebab-case describing the interaction (`metric-toggle`, `funnel-builder`). No chart-type prefix in the name — the folder provides that context.

**When adding a new interactive:** add a row to the Catalog table above with course, object name, one-sentence description, path, and live URL.

---

## Embed in Rise

```html
<iframe
  src="https://nlivni-amplitude.github.io/academy-interactives/[chart-type]/[object-name]/?v=1"
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
SHA=$(gh api repos/nlivni-amplitude/academy-interactives/contents/[chart-type]/[object-name]/index.html --jq '.sha')

gh api repos/nlivni-amplitude/academy-interactives/contents/[chart-type]/[object-name]/index.html \
  --method PUT \
  --field message="update [object-name]" \
  --field content="$(base64 -i [chart-type]/[object-name]/index.html)" \
  --field sha="$SHA" \
  --jq '.commit.sha'
```

Omit `--field sha` for a new file.

**Token note:** Pushing `index.html` files requires `repo` scope. Modifying `.github/workflows/` requires the `workflow` scope (`gh auth refresh -h github.com --scopes workflow`).

**Collaborators** with write access can push via `git push` directly — no special setup needed.
