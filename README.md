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
| Statsig | Rule Fall-Through Simulator | Toggle a shopper's targeting and Rule 2 rollout to watch a gate evaluate rules top-to-bottom | `statsig/feature-gates/01_rules-rollout_fall-through-simulator/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/feature-gates/01_rules-rollout_fall-through-simulator/) |
| Statsig | AND vs OR Trap | Side-by-side showing two conditions in one rule (AND) vs. two separate rules (OR via fall-through) | `statsig/feature-gates/01_rules-rollout_and-or-trap/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/feature-gates/01_rules-rollout_and-or-trap/) |
| Statsig | Rollout Dots | 100-dot grid where lowering the rollout % kicks passing users back out, showing deterministic re-evaluation | `statsig/feature-gates/01_rules-rollout_rollout-dots/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/feature-gates/01_rules-rollout_rollout-dots/) |
| Statsig | Per-Rule Lift Panel | Drag Rule 2's rollout to see why a rule at 100% shows no lift (no comparison group) | `statsig/feature-gates/02_gate-metrics_per-rule-lift/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/feature-gates/02_gate-metrics_per-rule-lift/) |
| Statsig | Exposure Cutoff Ticker | Live exposure-event stream that goes quiet at 0% and 100% rollout, by design | `statsig/feature-gates/02_gate-metrics_exposure-cutoff/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/feature-gates/02_gate-metrics_exposure-cutoff/) |
| Statsig | Archive Incident Stepper | 4-step walkthrough of how archiving a live gate removes it from the SDK payload and hides the feature | `statsig/feature-gates/03_safe-ops_archive-incident/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/feature-gates/03_safe-ops_archive-incident/) |
| Statsig | Scorecard Guided Tour | Column-by-column walkthrough of a Pulse scorecard: tier, lift, CI, p-value, and the guardrail trap | `statsig/reading-results/01_scorecard_guided-tour/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/reading-results/01_scorecard_guided-tour/) |
| Statsig | Assignment vs Participation | Animated funnel showing 20 assigned users become 3 participants, and why that gap is normal | `statsig/reading-results/02_participation_assignment-vs-participation/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/reading-results/02_participation_assignment-vs-participation/) |
| Statsig | Observed vs Projected | Animated bars contrasting observed conversions at 5% rollout with the Impact tab's 100% projection | `statsig/reading-results/03_lift_observed-vs-projected/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/reading-results/03_lift_observed-vs-projected/) |
| Statsig | SRM Balance Scale | Animated scale that settles at 54/46 and flags a sample ratio mismatch | `statsig/reading-results/04_diagnostics_srm-scale/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/reading-results/04_diagnostics_srm-scale/) |
| Statsig | CI Narrowing | Days-of-data slider showing a confidence interval tighten around a true +2.5% until it clears zero | `statsig/reading-results/04_diagnostics_ci-behavior/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/reading-results/04_diagnostics_ci-behavior/) |
| Statsig | Ship / Keep / Kill Practice | Three no-stakes decision scenarios teaching the primary-secondary-guardrail synthesis routine | `statsig/reading-results/05_the-call_decision-practice/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/reading-results/05_the-call_decision-practice/) |
| Statsig | Statsig-to-Amplitude Decoder | Searchable table mapping 23 Statsig terms to their Amplitude equivalents with match confidence | `statsig/reading-results/06_decoder_term-search/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/reading-results/06_decoder_term-search/) |
| Statsig | Stats Models At A Glance | Comparison table of nine statistical methods and whether each is default, optional, or absent on Statsig vs Amplitude | `statsig/stats-models/01_glance_stats-comparison/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/stats-models/01_glance_stats-comparison/) |
| Statsig | T-Test Signal vs Luck | Two distributions with a lift slider showing when a gap is separable from noise | `statsig/stats-models/02_ttest_signal-vs-luck/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/stats-models/02_ttest_signal-vs-luck/) |
| Statsig | CUPED Variance Reduction | Apply-CUPED toggle that shrinks a wide confidence interval until it clears zero | `statsig/stats-models/03_cuped_variance-reduction/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/stats-models/03_cuped_variance-reduction/) |
| Statsig | Winsorization Cap the Whale | Bar chart where capping one outlier order at P99 pulls the mean back to typical spend | `statsig/stats-models/04_winsorization_cap-the-whale/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/stats-models/04_winsorization_cap-the-whale/) |
| Statsig | Bonferroni Twelve Tests | 12-metric grid showing false wins appear without correction and vanish with it | `statsig/stats-models/05_bonferroni_twelve-tests/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/stats-models/05_bonferroni_twelve-tests/) |
| Statsig | Sequential Peek Anytime | Animated narrowing decision band showing why you can peek at a sequential test | `statsig/stats-models/06_sequential_peek-anytime/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/stats-models/06_sequential_peek-anytime/) |
| Statsig | SPRT Evidence Race | Evidence line crossing a decision boundary early for a strong effect, never for a null | `statsig/stats-models/07_sprt_evidence-race/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/stats-models/07_sprt_evidence-race/) |
| Statsig | Bayesian Updating | Posterior curve sharpening toward a probability-to-beat-control as data feeds in | `statsig/stats-models/08_bayesian_updating/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/stats-models/08_bayesian_updating/) |
| Statsig | Warehouse vs Cloud | Flow diagram contrasting where experiment math runs: vendor copy vs inside your own warehouse | `statsig/amplitude-mechanics/01_prologue_warehouse-vs-cloud/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/amplitude-mechanics/01_prologue_warehouse-vs-cloud/) |
| Statsig | Web vs Feature Experiment | One-question chooser routing a change to a visual web experiment or an SDK feature experiment | `statsig/amplitude-mechanics/01_prologue_web-vs-feature/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/amplitude-mechanics/01_prologue_web-vs-feature/) |
| Statsig | Deterministic Bucketing | Sort three shoppers by hash, then again, to show the same ID always lands on the same variant | `statsig/amplitude-mechanics/02_bucketing_deterministic-sort/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/amplitude-mechanics/02_bucketing_deterministic-sort/) |
| Statsig | Bucketing Salt Reshuffle | 40-shopper grid where changing the salt re-sorts about half of them mid-test | `statsig/amplitude-mechanics/02_bucketing_salt-reshuffle/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/amplitude-mechanics/02_bucketing_salt-reshuffle/) |
| Statsig | Sticky Bucketing Ramp | Ramp a split with sticky on vs off, marking shoppers who get re-dealt into a new variant | `statsig/amplitude-mechanics/02_bucketing_sticky/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/amplitude-mechanics/02_bucketing_sticky/) |
| Statsig | Deployment Keys | Deliver a flag to one of three surfaces to show client vs server keys and blast-radius hygiene | `statsig/amplitude-mechanics/03_delivery_deployment-keys/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/amplitude-mechanics/03_delivery_deployment-keys/) |
| Statsig | Local vs Remote Evaluation | Compare who decides the variant: enriched HQ round trip vs sub-millisecond local rulebook | `statsig/amplitude-mechanics/03_delivery_local-vs-remote/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/amplitude-mechanics/03_delivery_local-vs-remote/) |
| Statsig | Client-Server Matrix | Clickable 2x2 of client/server vs local/remote with each combo's best use and trap | `statsig/amplitude-mechanics/03_delivery_client-server-matrix/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/amplitude-mechanics/03_delivery_client-server-matrix/) |
| Statsig | Significance Explorer | Two sliders (effect size, users) driving a significance gauge past the 95% bar | `statsig/amplitude-mechanics/04_stats_significance-explorer/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/amplitude-mechanics/04_stats_significance-explorer/) |
| Statsig | Duration Estimator | Lift and traffic sliders returning days-to-significance to triage which tests are worth running | `statsig/amplitude-mechanics/05_epilogue_duration-estimator/` | [link](https://nlivni-amplitude.github.io/academy-interactives/statsig/amplitude-mechanics/05_epilogue_duration-estimator/) |

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
