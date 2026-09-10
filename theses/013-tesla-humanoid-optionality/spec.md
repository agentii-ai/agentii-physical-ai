# Research Thesis: Tesla — Humanoid Optionality

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 3 — Company Deep Dives (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
Is Tesla's humanoid programme a separately valuable option, or is it already fully embedded in the automotive valuation?

**Claim**: Tesla's humanoid optionality is real but unquantifiable from disclosed data, and the automotive and energy businesses already dominate any defensible valuation.

## 1b. Pillars

### Pillar 1 — Humanoid contributes no disclosed revenue (Priority: P1) 🎯 Minimum Defensible View
The humanoid programme has no separately reported revenue or segment disclosure.

**Why this priority**: Any humanoid valuation is therefore a pure assumption rather than an audited figure.

**Independently falsifiable**: Disclosure of humanoid revenue or a reporting segment falsifies it.

**wrong_if**: `metric=tesla_humanoid_revenue_disclosure_present threshold=1 source=10K_segment_data`

**Subscribed**: `revenue-decomp × deep`, `segment data × deep`

### Pillar 2 — Automotive and energy dominate the defensible valuation (Priority: P2)
A scenario-weighted DCF of disclosed businesses accounts for the overwhelming majority of justified value.

**Why this priority**: Anchors the valuation to auditable cash flows rather than narrative.

**Independently falsifiable**: Humanoid optionality exceeding 25% of a defensible SOTP falsifies it.

**wrong_if**: `metric=humanoid_implied_share_of_sotp_pct threshold=>25 source=sotp_analysis op=>`

**Subscribed**: `sotp-valuation × deep`, `dcf × full`

### Pillar 3 — Data scale is the genuine, if indirect, asset (Priority: P3)
Tesla's deployed fleet provides embodied data collection capacity no competitor matches, even absent humanoid revenue.

**Why this priority**: Identifies the real strategic asset independent of the humanoid timeline.

**Independently falsifiable**: A competitor demonstrating larger embodied-data collection falsifies it.

**wrong_if**: `metric=deployed_fleet_embodied_data_collection_hours_vs_peers threshold=>1.0 source=operational_disclosure op=>`

**Subscribed**: `business-model × deep`, `operational-kpi × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| TSLA | Subject | Cons Disc | — | Integrated humanoid programme under review |
| F | Automotive peer | Cons Disc | — | Traditional automotive valuation anchor |
| AMZN | Automation comparator | Cons Disc | — | Alternative robotics deployment model |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `sotp-valuation` | models-and-pitches | deep | TSLA | none | Segment-level valuation |
| `dcf` | models-and-pitches | full | TSLA | none | Scenario-weighted cash flows |
| `revenue-decomp` | business-intelligence | deep | TSLA | none | Segment revenue isolation |
| `segment data` | quantitative-analysis | deep | TSLA | none | Automotive vs energy split |
| `risk` | equity-research-core | standard | TSLA | none | Programme execution risk |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
The 63,523 XBRL facts make TSLA the most data-rich name in the universe — use it as the depth benchmark for other company theses.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/013-tesla-humanoid-optionality_synthesis.md`
- Snapshot: `snapshots/013-tesla-humanoid-optionality/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Segment isolation | Automotive vs energy disclosure | Week 1 | T-008 complete |
| 2 — SOTP construction | Value disclosed businesses | Week 2 | Phase 1 |
| 3 — Optionality quantification | Bound the humanoid option | Week 3 | Phase 2 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Tesla's humanoid optionality is real but unquantifiable from disclosed data,
  and the automotive and energy businesses already dominate any defensible valuation.
pillars:
- id: PIL-1
  priority: P1
  title: Humanoid contributes no disclosed revenue
  wrong_if:
    metric: tesla_humanoid_revenue_disclosure_present
    threshold: '1'
    source: 10K_segment_data
  subscriptions:
  - revenue-decomp × deep
  - segment data × deep
- id: PIL-2
  priority: P2
  title: Automotive and energy dominate the defensible valuation
  wrong_if:
    metric: humanoid_implied_share_of_sotp_pct
    threshold: '>25'
    source: sotp_analysis
    op: '>'
  subscriptions:
  - sotp-valuation × deep
  - dcf × full
- id: PIL-3
  priority: P3
  title: Data scale is the genuine, if indirect, asset
  wrong_if:
    metric: deployed_fleet_embodied_data_collection_hours_vs_peers
    threshold: '>1.0'
    source: operational_disclosure
    op: '>'
  subscriptions:
  - business-model × deep
  - operational-kpi × default
budget:
  max_tasks: 80
  max_retries_per_task: 2
expiry_triggers:
- earnings_release
- constitution_bump
- skill_version_mix
macro_sensitivity: high
constitution_pin: 1.2.0
```
