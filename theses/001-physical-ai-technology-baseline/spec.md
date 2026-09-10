# Research Thesis: Physical AI Technology Baseline

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 0 — Foundation (GATES ALL)
**Time Horizon**: 2026-Q4 → 2028 (multi-year technology curve)

## 1. Research Question
What must be physically true for embodied AI to reach economic parity, and where on that curve are we as of Q3 2026?

**Claim**: Embodied AI is data-bound, not compute-bound; the binding engineering constraint is manipulation reliability, and the value pool sits in actuation and sensing rather than the model layer.

## 1b. Pillars

### Pillar 1 — Data, not compute, is the binding constraint (Priority: P1) 🎯 Minimum Defensible View
Robotics foundation models train on a small fraction of frontier compute because there is insufficient embodied data, not because GPUs are scarce.

**Why this priority**: It reframes the entire capex thesis: if compute were the constraint, the trade would be semis; if data is, the trade is data collection and simulation.

**Independently falsifiable**: Measure the embodied-data gap directly; if robotics models demonstrably consume frontier-scale compute, the claim fails.

**wrong_if**: `metric=embodied_dataset_hours_vs_llm_pretrain_token_gap_order_of_magnitude threshold=>1000 source=industry_technical_disclosures op=>`

**Subscribed**: `secular-trends × default`, `business-model × default`

### Pillar 2 — Actuators dominate BOM; compute is marginal (Priority: P2)
Actuator + screw + reducer + motor content is 40-70% of a humanoid's bill of materials; the AI compute stack is only ~10-15%.

**Why this priority**: This is the core variant perception — the market prices physical AI as a compute story.

**Independently falsifiable**: A credible 2026 teardown putting actuator content below 35% falsifies it.

**wrong_if**: `metric=actuator_share_of_humanoid_bom_pct threshold=<35 source=public_teardown_or_10K_disclosure op=<`

**Subscribed**: `unit-economics × default`, `supply-chain × default`

### Pillar 3 — Manipulation reliability, not intelligence, gates deployment (Priority: P3)
The gating engineering problem is mean-time-between-failure and task success rate in unstructured environments — not model capability.

**Why this priority**: Determines whether 2026-2027 revenue is real or promotional.

**Independently falsifiable**: Disclosed deployment MTBF above 2,000 hours in commercial settings would falsify the constraint.

**wrong_if**: `metric=humanoid_mtbf_hours_in_commercial_deployment threshold=>2000 source=company_disclosure_or_fleet_operator op=>`

**Subscribed**: `operational-kpi × default`, `risk × default`

### Pillar 4 — The 'GPT-3.5 moment' arrives late 2027 through 2028 (Priority: P4)
Consensus timing for a step-change in general-purpose embodied capability is 2027-2028, not 2026.

**Why this priority**: Anchors the entire portfolio's time horizon and prevents underwriting a 2026 inflection.

**Independently falsifiable**: A commercially deployed, general-purpose humanoid fleet at scale before 2027-Q4 falsifies it.

**wrong_if**: `metric=general_purpose_humanoid_commercial_units_deployed threshold=>10000 source=company_and_fleet_disclosures`

**Subscribed**: `secular-trends × deep`, `recent-quarter × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| NVDA | Compute reference | IT | — | Baseline for the compute-boundness counterfactual |
| ISRG | Robotic reliability benchmark | Health Care | — | Only US-listed company with a decade of surgical-robot MTBF disclosure |
| TSLA | Integrated humanoid programme | Cons Disc | — | Only US-listed large-cap with a disclosed humanoid programme |
| AMZN | Warehouse automation deployer | Cons Disc | — | Largest disclosed fleet-scale robotics deployer |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `secular-trends` | equity-research-core | deep | NVDA, ISRG, TSLA | none | Technology adoption curve and disruption timing |
| `unit-economics` | business-intelligence | standard | TSLA, ISRG | none | Per-unit cost structure |
| `supply-chain` | industry-analysis | deep | NVDA, AMZN | none | Physical dependency mapping |
| `operational-kpi` | business-intelligence | standard | ISRG, AMZN | none | Reliability and utilisation metrics |
| `risk` | equity-research-core | standard | NVDA, TSLA | none | Technology and execution risk |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
This thesis is the workspace's technology primitive. Every downstream thesis (T-002…T-015) inherits its assumptions. Its falsification triggers a MAJOR constitution re-examination.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/001-physical-ai-technology-baseline_synthesis.md`
- Snapshot: `snapshots/001-physical-ai-technology-baseline/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Literature and physics baseline | T-001 tasks: torque density, energy density, BOM physics | Week 1 | Constitution v1.2.0 |
| 2 — Data-economics quantification | Cost per hour of teleop vs egocentric vs synthetic | Week 2 | Phase 1 |
| 3 — Reliability evidence | MTBF, task success rates from filings and transcripts | Week 3 | Phase 2 |
| 4 — Timing synthesis | Publish the capability timeline with falsifiers | Week 4 | Phase 3 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Embodied AI is data-bound, not compute-bound; the binding engineering constraint
  is manipulation reliability, and the value pool sits in actuation and sensing rather
  than the model layer.
pillars:
- id: PIL-1
  priority: P1
  title: Data, not compute, is the binding constraint
  wrong_if:
    metric: embodied_dataset_hours_vs_llm_pretrain_token_gap_order_of_magnitude
    threshold: '>1000'
    source: industry_technical_disclosures
    op: '>'
  subscriptions:
  - secular-trends × default
  - business-model × default
- id: PIL-2
  priority: P2
  title: Actuators dominate BOM; compute is marginal
  wrong_if:
    metric: actuator_share_of_humanoid_bom_pct
    threshold: <35
    source: public_teardown_or_10K_disclosure
    op: <
  subscriptions:
  - unit-economics × default
  - supply-chain × default
- id: PIL-3
  priority: P3
  title: Manipulation reliability, not intelligence, gates deployment
  wrong_if:
    metric: humanoid_mtbf_hours_in_commercial_deployment
    threshold: '>2000'
    source: company_disclosure_or_fleet_operator
    op: '>'
  subscriptions:
  - operational-kpi × default
  - risk × default
- id: PIL-4
  priority: P4
  title: The 'GPT-3.5 moment' arrives late 2027 through 2028
  wrong_if:
    metric: general_purpose_humanoid_commercial_units_deployed
    threshold: '>10000'
    source: company_and_fleet_disclosures
  subscriptions:
  - secular-trends × deep
  - recent-quarter × default
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
