# Research Thesis: Vision Stack — Ambarella and Cognex

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 3 — Company Deep Dives (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
Is vision a growth layer or a commoditising one, and do AMBA and CGNX offer differentiated exposure?

**Claim**: Machine vision is comparatively mature and competitive, so vision vendors are unlikely to capture value proportional to their perceived physical-AI exposure.

## 1b. Pillars

### Pillar 1 — Vision is a mature, competitive layer (Priority: P1) 🎯 Minimum Defensible View
Machine vision has multiple qualified vendors and limited remaining differentiation.

**Why this priority**: Guards against paying a scarcity multiple for a competitive market.

**Independently falsifiable**: Sustained above-peer gross margin expansion falsifies it.

**wrong_if**: `metric=cgnx_gross_margin_trend_vs_machine_vision_peer_median threshold=expanding source=10K_segment_data`

**Subscribed**: `competitive × deep`, `competitive-positioning × standard`

### Pillar 2 — Edge vision silicon faces SoC integration risk (Priority: P2)
Vision functionality is increasingly absorbed into general-purpose edge SoCs, compressing standalone vision-silicon value.

**Why this priority**: Identifies the specific substitution risk to the AMBA thesis.

**Independently falsifiable**: Sustained design-win growth for standalone vision SoCs falsifies it.

**wrong_if**: `metric=standalone_vision_soc_design_wins_trend threshold=expanding source=design_win_disclosure`

**Subscribed**: `competitive-positioning × deep`, `business-model × default`

### Pillar 3 — Nearest-term revenue is cyclical, not thematic (Priority: P3)
Both names remain levered to industrial and automotive cycles rather than physical-AI adoption.

**Why this priority**: Prevents mis-attributing cyclical recovery to thematic demand.

**Independently falsifiable**: Revenue growth decoupling from industrial cycle would falsify it.

**wrong_if**: `metric=revenue_growth_correlation_to_industrial_production_index threshold=>0.6 source=xbrl_and_macro_data op=>`

**Subscribed**: `recent-quarter × deep`, `ratio-analysis × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| AMBA | Subject — edge vision silicon | IT | — | Vision SoC franchise |
| CGNX | Subject — machine vision | IT | — | Machine vision franchise |
| ON | Adjacent | IT | — | Sensor and imaging content |
| ADI | Adjacent | IT | — | Vision signal chain |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `competitive × deep` | equity-research-core | deep | CGNX, AMBA | none | Vision layer structure |
| `business-model × deep` | equity-research-core | deep | AMBA | full | SoC franchise economics |
| `recent-quarter × deep` | equity-research-core | deep | AMBA, CGNX | none | Cycle vs theme decomposition |
| `ratio-analysis` | quantitative-analysis | standard | CGNX, AMBA | none | Margin and return profile |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
Pairs with T-004 (perception and sensing) to test whether value sits in sensing rather than optics or silicon.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/012-vision-stack-amba-cgnx_synthesis.md`
- Snapshot: `snapshots/012-vision-stack-amba-cgnx/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Layer structure | Competitive map of vision vendors | Week 1 | T-008 complete |
| 2 — Substitution risk | SoC integration threat assessment | Week 2 | Phase 1 |
| 3 — Cycle decomposition | Separate cyclical from thematic revenue | Week 3 | Phase 2 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Machine vision is comparatively mature and competitive, so vision vendors are
  unlikely to capture value proportional to their perceived physical-AI exposure.
pillars:
- id: PIL-1
  priority: P1
  title: Vision is a mature, competitive layer
  wrong_if:
    metric: cgnx_gross_margin_trend_vs_machine_vision_peer_median
    threshold: expanding
    source: 10K_segment_data
  subscriptions:
  - competitive × deep
  - competitive-positioning × standard
- id: PIL-2
  priority: P2
  title: Edge vision silicon faces SoC integration risk
  wrong_if:
    metric: standalone_vision_soc_design_wins_trend
    threshold: expanding
    source: design_win_disclosure
  subscriptions:
  - competitive-positioning × deep
  - business-model × default
- id: PIL-3
  priority: P3
  title: Nearest-term revenue is cyclical, not thematic
  wrong_if:
    metric: revenue_growth_correlation_to_industrial_production_index
    threshold: '>0.6'
    source: xbrl_and_macro_data
    op: '>'
  subscriptions:
  - recent-quarter × deep
  - ratio-analysis × default
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
