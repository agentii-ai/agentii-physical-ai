# Research Thesis: Value Chain Profit Pool Map

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 1 — Industry Structure (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
Where does economic profit accrue across the physical AI value chain, and which layer captures it durably?

**Claim**: The dominant profit pool sits in actuation, transmission, and force sensing; the model and compute layers are necessary but commoditising.

## 1b. Pillars

### Pillar 1 — Profit concentrates in motion and sensing (Priority: P1) 🎯 Minimum Defensible View
Actuation and sensing together exceed 55% of BOM and carry the highest barriers to substitution.

**Why this priority**: Identifies where to look for durable margin rather than transient revenue.

**Independently falsifiable**: Evidence that model-layer vendors capture more gross profit per unit than motion vendors falsifies it.

**wrong_if**: `metric=actuation_plus_sensing_share_of_bom_pct threshold=<55 source=filed_teardown_or_segment_disclosure op=<`

**Subscribed**: `supply-chain × deep`, `unit-economics × default`

### Pillar 2 — China holds a ~3x structural cost advantage (Priority: P2)
Domestic Chinese component supply yields roughly $46K BOM versus ~$131K for non-Chinese supply.

**Why this priority**: Determines which layer is defensible and which is exposed to import substitution.

**Independently falsifiable**: A non-Chinese BOM within 2x of the Chinese equivalent falsifies it.

**wrong_if**: `metric=nonchina_to_china_humanoid_bom_cost_ratio threshold=<2.0 source=public_teardown op=<`

**Subscribed**: `supply-chain × deep`, `competitive-positioning × default`

### Pillar 3 — The model layer captures minimal value near-term (Priority: P3)
Foundation-model vendors are not yet extracting durable rent from physical AI deployments.

**Why this priority**: Prevents overpaying for 'AI exposure' in names whose economics are hardware.

**Independently falsifiable**: Any disclosed per-robot software royalty at scale falsifies it.

**wrong_if**: `metric=model_layer_revenue_per_deployed_unit_usd threshold=>5000 source=company_disclosure`

**Subscribed**: `business-model × default`, `revenue-decomp × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| NVDA | Compute layer | IT | — | Largest absolute AI profit pool — the layer to beat |
| PH | Motion layer | Industrials | — | Largest analyzable motion-control franchise |
| ISRG | Integrated system | Health Care | — | Proof that integrated robotics can hold 65%+ gross margin |
| TSLA | Vertically integrated | Cons Disc | — | Vertical integration reference case |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `supply-chain` | industry-analysis | deep | NVDA, PH, ISRG | none | Value-chain mapping and dependency |
| `unit-economics` | business-intelligence | deep | ISRG, TSLA | none | Cost stack decomposition |
| `competitive-positioning` | industry-analysis | standard | PH, NVDA | none | Layer-level competitive structure |
| `revenue-decomp` | business-intelligence | standard | PH, ISRG | none | Revenue mix and mix-shift |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
Feeds directly into T-008 (chokepoint synthesis). Each layer identified here becomes a candidate chokepoint for T-003 through T-007.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/002-value-chain-profit-pool-map_synthesis.md`
- Snapshot: `snapshots/002-value-chain-profit-pool-map/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Layer definition | Enumerate value-chain layers and assign tickers | Week 1 | T-001 complete |
| 2 — Profit quantification | Segment economics per layer | Week 2 | Phase 1 |
| 3 — Durability assessment | Barriers, substitution risk, pricing power | Week 3 | Phase 2 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: The dominant profit pool sits in actuation, transmission, and force sensing;
  the model and compute layers are necessary but commoditising.
pillars:
- id: PIL-1
  priority: P1
  title: Profit concentrates in motion and sensing
  wrong_if:
    metric: actuation_plus_sensing_share_of_bom_pct
    threshold: <55
    source: filed_teardown_or_segment_disclosure
    op: <
  subscriptions:
  - supply-chain × deep
  - unit-economics × default
- id: PIL-2
  priority: P2
  title: China holds a ~3x structural cost advantage
  wrong_if:
    metric: nonchina_to_china_humanoid_bom_cost_ratio
    threshold: <2.0
    source: public_teardown
    op: <
  subscriptions:
  - supply-chain × deep
  - competitive-positioning × default
- id: PIL-3
  priority: P3
  title: The model layer captures minimal value near-term
  wrong_if:
    metric: model_layer_revenue_per_deployed_unit_usd
    threshold: '>5000'
    source: company_disclosure
  subscriptions:
  - business-model × default
  - revenue-decomp × default
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
