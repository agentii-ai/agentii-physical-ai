# Research Thesis: Embodied Data and Model Layer

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 1 — Industry Structure (parallel)
**Time Horizon**: 2026-Q4 → 2028

## 1. Research Question
Who owns the embodied data flywheel, and does it constitute a defensible moat?

**Claim**: Embodied data is the scarcest input in physical AI; egocentric human video at roughly one-third the cost of teleoperation is the most likely escape route from the data wall, and it favours whoever aggregates the largest human-video corpus.

## 1b. Pillars

### Pillar 1 — The data wall is real and quantified (Priority: P1) 🎯 Minimum Defensible View
Embodied datasets trail LLM pretraining corpora by roughly four orders of magnitude.

**Why this priority**: Establishes data as the binding scarcity that the whole sector must resolve.

**Independently falsifiable**: A demonstrated embodied dataset at LLM-comparable token scale falsifies it.

**wrong_if**: `metric=embodied_to_llm_pretraining_data_gap_orders_of_magnitude threshold=<2 source=technical_publication op=<`

**Subscribed**: `secular-trends × deep`, `risk × default`

### Pillar 2 — Egocentric video displaces teleoperation on cost (Priority: P2)
Body-less human video capture costs roughly one-third of teleoperation and is scaling faster.

**Why this priority**: Shifts the moat from fleet operators to whoever owns human-video aggregation.

**Independently falsifiable**: Teleoperation cost per hour falling below egocentric capture cost falsifies it.

**wrong_if**: `metric=teleop_cost_per_hour_ratio_to_egocentric threshold=>1.0 source=industry_cost_disclosure op=<`

**Subscribed**: `unit-economics × default`, `operational-kpi × default`

### Pillar 3 — A model-ossification threshold constrains scaling (Priority: P3)
There is a parameter-count threshold below which embodied models fail to generalise, limiting small-model strategies.

**Why this priority**: Determines whether edge compute or cloud compute wins the inference layer.

**Independently falsifiable**: Reproduction showing generalisation below the stated threshold falsifies it.

**wrong_if**: `metric=generalisation_ossification_parameter_threshold_billions threshold=<7 source=technical_replication op=<`

**Subscribed**: `technical-execution × default`, `secular-trends × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| NVDA | Training and simulation compute | IT | — | Owns the simulation and world-model toolchain |
| TSLA | Fleet-scale data collection | Cons Disc | — | Largest deployed embodied data collector |
| AMZN | Warehouse manipulation data | Cons Disc | — | Large-scale structured manipulation data |
| QCOM | Edge inference | IT | — | Edge compute for on-robot models |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `secular-trends` | equity-research-core | deep | NVDA, TSLA, QCOM | none | Data-curve and capability timing |
| `business-model` | equity-research-core | standard | NVDA, AMZN | none | Data moat economics |
| `operational-kpi` | business-intelligence | standard | TSLA, AMZN | none | Fleet and data-collection metrics |
| `risk × default` | equity-research-core | standard | NVDA, TSLA | none | Data-scarcity risk |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
Feeds T-008 and T-009. Tests whether data ownership is a genuine moat or a cost centre.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/005-embodied-data-model-layer_synthesis.md`
- Snapshot: `snapshots/005-embodied-data-model-layer/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Data taxonomy | Enumerate embodied data modalities and costs | Week 1 | T-001 complete |
| 2 — Moat assessment | Who aggregates, who can defend it | Week 2 | Phase 1 |
| 3 — Timing | When the data wall is plausibly breached | Week 3 | Phase 2 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Embodied data is the scarcest input in physical AI; egocentric human video
  at roughly one-third the cost of teleoperation is the most likely escape route from
  the data wall, and it favours whoever aggregates the largest human-video corpus.
pillars:
- id: PIL-1
  priority: P1
  title: The data wall is real and quantified
  wrong_if:
    metric: embodied_to_llm_pretraining_data_gap_orders_of_magnitude
    threshold: <2
    source: technical_publication
    op: <
  subscriptions:
  - secular-trends × deep
  - risk × default
- id: PIL-2
  priority: P2
  title: Egocentric video displaces teleoperation on cost
  wrong_if:
    metric: teleop_cost_per_hour_ratio_to_egocentric
    threshold: '>1.0'
    source: industry_cost_disclosure
    op: <
  subscriptions:
  - unit-economics × default
  - operational-kpi × default
- id: PIL-3
  priority: P3
  title: A model-ossification threshold constrains scaling
  wrong_if:
    metric: generalisation_ossification_parameter_threshold_billions
    threshold: <7
    source: technical_replication
    op: <
  subscriptions:
  - technical-execution × default
  - secular-trends × default
budget:
  max_tasks: 80
  max_retries_per_task: 2
expiry_triggers:
- earnings_release
- constitution_bump
- skill_version_mix
macro_sensitivity: medium
constitution_pin: 1.2.0
```
