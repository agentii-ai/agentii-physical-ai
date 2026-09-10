# Research Thesis: Qualcomm — Edge Robotics Compute

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 3 — Company Deep Dives (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
Can Qualcomm establish a defensible position in on-robot inference compute?

**Claim**: Edge inference is the more contestable layer, but Qualcomm's power-efficiency position and handset-derived IP give it a credible route into robotics SoCs.

## 1b. Pillars

### Pillar 1 — Edge inference is the contestable layer (Priority: P1) 🎯 Minimum Defensible View
On-robot compute is fragmented with no incumbent comparable to NVIDIA's training position.

**Why this priority**: An open layer is where a challenger can establish position.

**Independently falsifiable**: Evidence of NVIDIA locking the edge layer through software falsifies it.

**wrong_if**: `metric=edge_robotics_soc_design_win_count_nvidia_vs_qualcomm threshold=>1.0 source=design_win_disclosure op=>`

**Subscribed**: `competitive-positioning × deep`, `competitive × default`

### Pillar 2 — Power efficiency is the deciding constraint (Priority: P2)
Battery is under 1% of humanoid BOM, so the constraint is thermal and payload rather than energy capacity.

**Why this priority**: Reframes the competition from raw TOPS to performance-per-watt.

**Independently falsifiable**: A humanoid shipping with materially larger battery for compute falsifies it.

**wrong_if**: `metric=robot_soc_performance_per_watt_gap_vs_competitors threshold=parity source=technical_specification`

**Subscribed**: `secular-trends × default`, `business-model × default`

### Pillar 3 — Robotics is optionality, not a revenue driver (Priority: P3)
Robotics revenue is immaterial against handsets and automotive through the thesis horizon.

**Why this priority**: Sets the correct valuation frame — do not pay a robotics multiple.

**Independently falsifiable**: Disclosed robotics revenue above 5% of segment total falsifies it.

**wrong_if**: `metric=qualcomm_robotics_revenue_share_of_qct_pct threshold=>5 source=10K_segment_data op=>`

**Subscribed**: `revenue-decomp × default`, `segment data × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| QCOM | Subject | IT | — | Edge compute franchise under review |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `competitive` | equity-research-core | deep | QCOM | none | Edge compute competitive structure |
| `business-model` | equity-research-core | standard | QCOM | none | Licensing and silicon economics |
| `revenue-decomp` | business-intelligence | standard | QCOM | none | QCT segmentation |
| `reverse-dcf` | quantitative-analysis | standard | QCOM | none | Implied expectations |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
Counterpoint to T-009. Together they resolve whether the compute layer is monopolised or contestable.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/010-qualcomm-edge-robotics_synthesis.md`
- Snapshot: `snapshots/010-qualcomm-edge-robotics/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Position mapping | Robotics SoC design wins and roadmap | Week 1 | T-008 complete |
| 2 — Technical constraint | Performance-per-watt benchmarking | Week 2 | Phase 1 |
| 3 — Valuation | Optionality vs priced-in expectations | Week 3 | Phase 2 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Edge inference is the more contestable layer, but Qualcomm's power-efficiency
  position and handset-derived IP give it a credible route into robotics SoCs.
pillars:
- id: PIL-1
  priority: P1
  title: Edge inference is the contestable layer
  wrong_if:
    metric: edge_robotics_soc_design_win_count_nvidia_vs_qualcomm
    threshold: '>1.0'
    source: design_win_disclosure
    op: '>'
  subscriptions:
  - competitive-positioning × deep
  - competitive × default
- id: PIL-2
  priority: P2
  title: Power efficiency is the deciding constraint
  wrong_if:
    metric: robot_soc_performance_per_watt_gap_vs_competitors
    threshold: parity
    source: technical_specification
  subscriptions:
  - secular-trends × default
  - business-model × default
- id: PIL-3
  priority: P3
  title: Robotics is optionality, not a revenue driver
  wrong_if:
    metric: qualcomm_robotics_revenue_share_of_qct_pct
    threshold: '>5'
    source: 10K_segment_data
    op: '>'
  subscriptions:
  - revenue-decomp × default
  - segment data × default
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
