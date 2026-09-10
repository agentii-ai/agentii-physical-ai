# Research Thesis: NVIDIA — Physical AI Compute Franchise

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 3 — Company Deep Dives (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
What is NVIDIA's defensible position in physical AI specifically, as distinct from its data-centre franchise?

**Claim**: NVIDIA's physical-AI position rests on the simulation and world-model toolchain rather than on inference silicon, where edge competitors are better positioned.

## 1b. Pillars

### Pillar 1 — Simulation, not inference, is the defensible layer (Priority: P1) 🎯 Minimum Defensible View
Omniverse and world-model tooling create switching costs that edge inference silicon does not.

**Why this priority**: Separates the durable part of the franchise from the contestable part.

**Independently falsifiable**: A credible open-source simulation stack achieving comparable fidelity falsifies it.

**wrong_if**: `metric=nvidia_simulation_revenue_growth_vs_inference_growth threshold=>1.0 source=10K_segment_disclosure op=>`

**Subscribed**: `secular-trends × deep`, `business-model × deep`

### Pillar 2 — Physical AI is immaterial to consolidated revenue near-term (Priority: P2)
Robotics revenue is a rounding error against data-centre, and should not be underwritten as a near-term driver.

**Why this priority**: Prevents double-counting a thematic narrative into a valuation that data-centre already justifies.

**Independently falsifiable**: Disclosed robotics revenue above 5% of total falsifies it.

**wrong_if**: `metric=robotics_and_simulation_revenue_share_of_total_pct threshold=>5 source=10K_segment_data op=>`

**Subscribed**: `revenue-decomp × deep`, `segment data × deep`

### Pillar 3 — Valuation embeds no physical-AI optionality (Priority: P3)
At current multiples the physical-AI option is not separately priced — upside is not being paid for, but neither is it a cushion.

**Why this priority**: Determines whether the name is a value entry or a crowded momentum position.

**Independently falsifiable**: Reverse-DCF implying a physical-AI premium in the current price falsifies it.

**wrong_if**: `metric=nvda_reverse_dcf_implied_growth_vs_consensus threshold=>consensus_plus_500bps source=reverse-dcf_analysis op=>`

**Subscribed**: `reverse-dcf × deep`, `valuation-methods × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| NVDA | Subject | IT | — | Compute franchise under review |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `business-model` | equity-research-core | deep | NVDA | full | Franchise economics and moat |
| `revenue-decomp` | business-intelligence | deep | NVDA | none | Segment revenue isolation |
| `segment data` | quantitative-analysis | deep | NVDA | none | Data-centre vs robotics split |
| `reverse-dcf` | quantitative-analysis | deep | NVDA | none | Implied expectations |
| `competitive` | equity-research-core | standard | NVDA | none | Edge competitor threat |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
Reads against T-010 (Qualcomm) as the edge-inference counterpoint and T-008 as the chokepoint benchmark.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/009-nvidia-physical-ai-compute_synthesis.md`
- Snapshot: `snapshots/009-nvidia-physical-ai-compute/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Segment isolation | Separate robotics and simulation from data-centre | Week 1 | T-008 complete |
| 2 — Moat assessment | Simulation switching costs | Week 2 | Phase 1 |
| 3 — Valuation | Reverse-DCF implied expectations | Week 3 | Phase 2 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: NVIDIA's physical-AI position rests on the simulation and world-model toolchain
  rather than on inference silicon, where edge competitors are better positioned.
pillars:
- id: PIL-1
  priority: P1
  title: Simulation, not inference, is the defensible layer
  wrong_if:
    metric: nvidia_simulation_revenue_growth_vs_inference_growth
    threshold: '>1.0'
    source: 10K_segment_disclosure
    op: '>'
  subscriptions:
  - secular-trends × deep
  - business-model × deep
- id: PIL-2
  priority: P2
  title: Physical AI is immaterial to consolidated revenue near-term
  wrong_if:
    metric: robotics_and_simulation_revenue_share_of_total_pct
    threshold: '>5'
    source: 10K_segment_data
    op: '>'
  subscriptions:
  - revenue-decomp × deep
  - segment data × deep
- id: PIL-3
  priority: P3
  title: Valuation embeds no physical-AI optionality
  wrong_if:
    metric: nvda_reverse_dcf_implied_growth_vs_consensus
    threshold: '>consensus_plus_500bps'
    source: reverse-dcf_analysis
    op: '>'
  subscriptions:
  - reverse-dcf × deep
  - valuation-methods × default
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
