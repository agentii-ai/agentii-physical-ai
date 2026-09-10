# Research Thesis: Perception and Force Sensing

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 1 — Industry Structure (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
Does force/torque sensing — not vision — gate dexterous manipulation, and who supplies it?

**Claim**: Tactile and force sensing is materially less mature than visual perception and is the true bottleneck for dexterous manipulation; vision is comparatively commoditised.

## 1b. Pillars

### Pillar 1 — Force/torque sensing is 11-18% of BOM and ~80% of perception content (Priority: P1) 🎯 Minimum Defensible View
Six-axis force/torque sensors dominate perception cost rather than cameras.

**Why this priority**: If true, sensing vendors capture more value than vision vendors — inverting the common assumption.

**Independently falsifiable**: A teardown placing vision above force sensing in perception cost falsifies it.

**wrong_if**: `metric=force_torque_share_of_perception_cost_pct threshold=<50 source=public_teardown op=<`

**Subscribed**: `unit-economics × default`, `supply-chain × default`

### Pillar 2 — Vision is comparatively solved (Priority: P2)
Machine vision for manipulation is a mature, competitive market with limited differentiation remaining.

**Why this priority**: Determines whether vision exposure is a growth thesis or a value trap.

**Independently falsifiable**: Sustained above-market gross margin expansion by a pure vision vendor would falsify it.

**wrong_if**: `metric=machine_vision_vendor_gross_margin_trend threshold=expanding source=10K_segment_data`

**Subscribed**: `competitive × default`, `business-model × default`

### Pillar 3 — US-listed sensing exposure is indirect (Priority: P3)
There is no US-listed pure-play force/torque sensor vendor with retrievable agentii coverage; exposure must be obtained through diversified names.

**Why this priority**: Sets realistic expectations for portfolio purity in this layer.

**Independently falsifiable**: Discovery of a covered pure-play falsifies it.

**wrong_if**: `metric=us_listed_pureplay_force_sensor_ticker_count_with_agentii_coverage threshold=>0 source=search_documents op=>`

**Subscribed**: `segment data review × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| CGNX | Machine vision | IT | — | Vision pure-play with agentii coverage |
| AMBA | Edge vision silicon | IT | — | Vision SoC for autonomous systems |
| ADI | Sensing and signal chain | IT | — | Force and precision signal conditioning |
| ON | Sensors and power | IT | — | Sensor and analog content |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `supply-chain` | industry-analysis | deep | CGNX, AMBA, ADI, ON | none | Sensing value chain |
| `competitive` | equity-research-core | standard | CGNX, AMBA | none | Vision market structure |
| `segment data` | quantitative-analysis | standard | CGNX, ADI | none | Segment exposure quantification |
| `business-model × default` | equity-research-core | standard | CGNX | none | Vision vendor economics |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
Feeds T-008 and T-012. Tests whether the perception layer's value sits in silicon, optics, or sensing.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/004-perception-force-sensing_synthesis.md`
- Snapshot: `snapshots/004-perception-force-sensing/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Sensing taxonomy | Categorise vision vs tactile vs proprioceptive | Week 1 | T-001 complete |
| 2 — Cost attribution | Perception BOM split by sensing modality | Week 2 | Phase 1 |
| 3 — Vendor mapping | Analyzable exposure per modality | Week 3 | Phase 2 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Tactile and force sensing is materially less mature than visual perception
  and is the true bottleneck for dexterous manipulation; vision is comparatively commoditised.
pillars:
- id: PIL-1
  priority: P1
  title: Force/torque sensing is 11-18% of BOM and ~80% of perception content
  wrong_if:
    metric: force_torque_share_of_perception_cost_pct
    threshold: <50
    source: public_teardown
    op: <
  subscriptions:
  - unit-economics × default
  - supply-chain × default
- id: PIL-2
  priority: P2
  title: Vision is comparatively solved
  wrong_if:
    metric: machine_vision_vendor_gross_margin_trend
    threshold: expanding
    source: 10K_segment_data
  subscriptions:
  - competitive × default
  - business-model × default
- id: PIL-3
  priority: P3
  title: US-listed sensing exposure is indirect
  wrong_if:
    metric: us_listed_pureplay_force_sensor_ticker_count_with_agentii_coverage
    threshold: '>0'
    source: search_documents
    op: '>'
  subscriptions:
  - segment data review × default
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
