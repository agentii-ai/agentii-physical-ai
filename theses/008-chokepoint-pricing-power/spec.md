# Research Thesis: Chokepoint Pricing Power Synthesis

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 2 — Synthesis (GATES PHASE 3)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
Which of the identified chokepoints actually convert into durable pricing power, and which merely look scarce?

**Claim**: Chokepoint position alone does not confer pricing power; only chokepoints combining high switching cost with genuine capacity constraint will produce durable margin expansion.

## 1b. Pillars

### Pillar 1 — Chokepoint and profit are not the same thing (Priority: P1) 🎯 Minimum Defensible View
Several scarce components are scarce because volume is low, not because substitution is impossible — scarcity without switching cost is transient.

**Why this priority**: Prevents the portfolio from paying chokepoint multiples for commodity economics.

**Independently falsifiable**: If every identified chokepoint shows expanding gross margin, the distinction is empty and this pillar fails.

**wrong_if**: `metric=chokepoints_with_expanding_gross_margin_share_pct threshold=>90 source=10K_segment_gross_margin_trend op=>`

**Subscribed**: `competitive × deep`, `business-model × deep`, `unit-economics × default`

### Pillar 2 — Pricing power requires switching cost plus capacity constraint (Priority: P2)
Both conditions must hold simultaneously; either alone produces cyclical rather than structural returns.

**Why this priority**: Gives the portfolio a two-factor test rather than a narrative.

**Independently falsifiable**: A chokepoint with only one condition demonstrating durable pricing falsifies it.

**wrong_if**: `metric=qualified_chokepoint_count_meeting_both_criteria threshold=<2 source=composite_of_T003_to_T007 op=<`

**Subscribed**: `competitive-positioning × deep`, `segment data × default`

### Pillar 3 — Only a small number of chokepoints are investable (Priority: P3)
Applying the two-factor test plus the P2 coverage constraint leaves a very short list of actionable names.

**Why this priority**: Sets realistic expectations for portfolio construction in T-015.

**Independently falsifiable**: More than five chokepoints surviving both filters falsifies it.

**wrong_if**: `metric=investable_chokepoint_count_after_coverage_filter threshold=>5 source=composite_analysis op=>`

**Subscribed**: `valuation-methods × default`, `risk × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| PH | Motion chokepoint candidate | Industrials | — | Primary candidate — capacity and switching cost |
| ISRG | System-level moat | Health Care | — | Integrated chokepoint benchmark |
| NVDA | Compute chokepoint | IT | — | The strongest existing chokepoint as reference |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `competitive × deep` | equity-research-core | deep | PH, ISRG, NVDA | none | Moat and switching-cost assessment |
| `business-model × deep` | equity-research-core | deep | PH, ISRG, NVDA | none | Pricing-power mechanics |
| `unit-economics × default` | business-intelligence | deep | PH, ISRG | none | Margin structure |
| `competitive-positioning × standard` | industry-analysis | standard | PH, NVDA | none | Structural positioning |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
This is the decision gate for Phase 3. Company deep dives should only be dispatched on names that survive this synthesis.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/008-chokepoint-pricing-power_synthesis.md`
- Snapshot: `snapshots/008-chokepoint-pricing-power/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Chokepoint inventory | Consolidate findings from T-003 through T-007 | Week 1 | T-002…T-007 complete |
| 2 — Two-factor test | Apply switching-cost and capacity filters | Week 2 | Phase 1 |
| 3 — Investability filter | Apply the P2 coverage constraint | Week 3 | Phase 2 |
| 4 — Gate 4 review | Budget confirmation before Phase 3 dispatch | Week 4 | Phase 3 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Chokepoint position alone does not confer pricing power; only chokepoints combining
  high switching cost with genuine capacity constraint will produce durable margin
  expansion.
pillars:
- id: PIL-1
  priority: P1
  title: Chokepoint and profit are not the same thing
  wrong_if:
    metric: chokepoints_with_expanding_gross_margin_share_pct
    threshold: '>90'
    source: 10K_segment_gross_margin_trend
    op: '>'
  subscriptions:
  - competitive × deep
  - business-model × deep
  - unit-economics × default
- id: PIL-2
  priority: P2
  title: Pricing power requires switching cost plus capacity constraint
  wrong_if:
    metric: qualified_chokepoint_count_meeting_both_criteria
    threshold: <2
    source: composite_of_T003_to_T007
    op: <
  subscriptions:
  - competitive-positioning × deep
  - segment data × default
- id: PIL-3
  priority: P3
  title: Only a small number of chokepoints are investable
  wrong_if:
    metric: investable_chokepoint_count_after_coverage_filter
    threshold: '>5'
    source: composite_analysis
    op: '>'
  subscriptions:
  - valuation-methods × default
  - risk × default
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
