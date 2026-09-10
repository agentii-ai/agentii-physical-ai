# Research Thesis: Value Chain Profit Pool Map

**Constitution Ref**: workspace/constitution.md (pin `1.3.0`)
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

**wrong_if**: `metric=motion_model_gm_gap_change_pp threshold=<-10 source=segment_disclosure op=<` (durability half — re-scoped from a level ratio, clarify round 4: the motion-vs-model GM gap (motion GM minus model GM, pp) falling more than 10pp over the 3-FY corpus falsifies it — a level comparison confounds business-model economics with barriers)

**Falsifier evaluation rule (clarify round 3)**: BOM-share evidence comes from SEC-filing-derived proxies (PH Motion Systems segment economics, ISRG cost stack, TSLA COGS structure); teardown figures enter only as [VIEW] external references.

**Subscribed**: `PH × supply-chain`, `AMBA × supply-chain`, `CGNX × supply-chain`, `ISRG × supply-chain`, `NVDA × supply-chain`, `SPCX × supply-chain`, `ISRG × unit-economics`, `TSLA × unit-economics`, `PH × competitive-positioning`

### Pillar 2 — China holds a ~3x structural cost advantage (Priority: P2)
Domestic Chinese component supply yields roughly $46K BOM versus ~$131K for non-Chinese supply.

**Why this priority**: Determines which layer is defensible and which is exposed to import substitution.

**Independently falsifiable**: A non-Chinese BOM within 2x of the Chinese equivalent falsifies it.

**wrong_if**: `metric=nonchina_to_china_humanoid_bom_cost_ratio threshold=<2.0 source=public_teardown op=<`

**Falsifier evaluation rule (clarify round 3)**: China-ratio evidence comes from SEC-filing-derived proxies (disclosed supplier/cost data, TSLA COGS structure); teardown figures enter only as [VIEW] external references.

**Subscribed**: `PH × supply-chain`, `AMBA × competitive-positioning`, `NVDA × competitive-positioning`

### Pillar 3 — The model layer captures minimal value near-term (Priority: P3)
Foundation-model vendors are not yet extracting durable rent from physical AI deployments.

**Why this priority**: Prevents overpaying for 'AI exposure' in names whose economics are hardware.

**Independently falsifiable**: Any disclosed per-robot software royalty at scale falsifies it.

**wrong_if**: `metric=model_layer_revenue_per_deployed_unit_usd threshold=>5000 source=company_disclosure op=>`

**Metric definition (clarify round 3)**: model-layer revenue includes per-unit software/subscription revenue (ISRG My Intuitive+, NVDA platform software), not only explicit per-robot royalties.

**Subscribed**: `PH × revenue-decomp`, `ISRG × revenue-decomp`, `PH × business-model`, `ISRG × business-model`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| NVDA | Compute layer | IT | ~14.3% | Largest absolute AI profit pool — the layer to beat |
| PH | Motion layer | Industrials | ~14.3% | Largest analyzable motion-control franchise |
| ISRG | Integrated system | Health Care | ~14.3% | Proof that integrated robotics can hold 65%+ gross margin |
| TSLA | Vertically integrated | Cons Disc | ~14.3% | Vertical integration reference case |
| AMBA | Sensing silicon (edge AI vision) | IT | ~14.3% | Sensing-layer anchor for PIL-1: edge-AI vision silicon for robotics/autonomy (constitution P2 Vision/sensing layer) |
| CGNX | Industrial machine vision | IT | ~14.3% | Automation-side sensing incumbent — the industrial profit-pool reference for machine vision |
| SPCX | End-market compute deployer | Industrials | ~14.3% | Demand-side pool: compute-led capex ($28.5B H1-2026, 82.7% AI — T-001 SPCX artifact) pulls the upstream layers; one-quarter issuer |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `supply-chain` | industry-analysis | standard | NVDA, PH, ISRG, AMBA, CGNX, SPCX | none | Value-chain mapping and dependency |
| `unit-economics` | business-intelligence | standard | ISRG, TSLA | none | Cost stack decomposition |
| `competitive-positioning` | industry-analysis | standard | PH, NVDA, AMBA | none | Layer-level competitive structure |
| `revenue-decomp` | business-intelligence | standard | PH, ISRG | none | Revenue mix and mix-shift |
| `business-model` | equity-research-core | standard | PH, ISRG | none | Business-model classification of layer economics |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

> **Depth hazard (T-001 reproduce.md deviation #3, apply 2026-09-10)**: `deep`
> is unsafe for skills with empty `essentials_modes` — it expands to
> SKILL.md section-heading slugs as fake task names. `supply-chain` and
> `unit-economics` therefore run `standard` in §3; the Deep tier above applies
> only to skills whose `essentials_modes` are real mode slugs.

## 5. Cross-Cutting Analysis
Feeds directly into T-008 (chokepoint pricing power). Each layer identified here becomes a candidate chokepoint for T-003 through T-007.

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
  - metric: actuation_plus_sensing_share_of_bom_pct
    threshold: <55
    source: filed_teardown_or_segment_disclosure
    op: <
  - metric: motion_model_gm_gap_change_pp
    threshold: <-10
    source: segment_disclosure
    op: <
  subscriptions:
  - supply-chain × standard
  - unit-economics × standard
  - competitive-positioning × standard
- id: PIL-2
  priority: P2
  title: China holds a ~3x structural cost advantage
  wrong_if:
    metric: nonchina_to_china_humanoid_bom_cost_ratio
    threshold: <2.0
    source: public_teardown
    op: <
  subscriptions:
  - supply-chain × standard
  - competitive-positioning × standard
- id: PIL-3
  priority: P3
  title: The model layer captures minimal value near-term
  wrong_if:
    metric: model_layer_revenue_per_deployed_unit_usd
    threshold: '>5000'
    source: company_disclosure
    op: '>'
  subscriptions:
  - business-model × standard
  - revenue-decomp × standard
budget:
  max_tasks: 80
  max_retries_per_task: 2
expiry_triggers:
- earnings_release
- constitution_bump
- skill_version_mix
macro_sensitivity: medium
constitution_pin: 1.3.0
```

## Clarifications

- [2026-09-10] Q: PIL-1b (motion_layer_gross_margin_vs_model_layer_gm_ratio < 1.0) is already triggered by T-001's audited anchors: PH GM 37.7% / DI op margin 23.8%, ISRG 66.3%, TSLA 17.8% all sit below NVDA's 71.1%. A level comparison confounds business-model economics with barriers to substitution. How should the durability falsifier be handled? → A: Re-scope to a trend metric: metric=motion_model_gm_gap_change_pp threshold=<-10 source=segment_disclosure op=< — wrong_if the motion-vs-model GM gap (motion GM minus model GM, pp) falls by more than 10pp over the 3-FY corpus. Durability is how the gap moves, not its level; the model layer proving as durable as motion kills the barriers claim.

- [2026-09-10] Q: PIL-3's falsifier is model_layer_revenue_per_deployed_unit_usd > 5000 — but what counts as 'model-layer revenue'? T-001's corpus has no per-robot royalties; it has per-unit software subscriptions (ISRG My Intuitive+) and platform revenue (NVDA Edge $6.4B). The definition decides whether the falsifier can fire. → A: Include subscriptions: per-unit software/subscription revenue counts as model-layer revenue (e.g., ISRG My Intuitive+ AI subscription — first renewal wave with zero opt-outs per the T-001 artifact — and NVDA software per platform), not only explicit per-robot royalties.
- [2026-09-10] Q: PIL-1 and PIL-2 falsifiers source from teardown data (filed_teardown_or_segment_disclosure, public_teardown) — which agentii retrieval cannot reach (T-001 challenge finding #1: three of four falsifiers source outside the corpus). How should T-002's implement evaluate these falsifiers? → A: Filing proxies + tagged views: evaluate the BOM-share and China-ratio falsifiers against SEC-filing-derived proxies (PH Motion Systems segment economics, ISRG cost stack, TSLA COGS structure, disclosed supplier/cost data); teardown figures enter only as clearly-tagged [VIEW] external references. Matches how T-001 handled PIL-2.
- [2026-09-10] Q: PIL-1 claims two things — actuation+sensing >55% of BOM AND the highest barriers to substitution — but the wrong_if only measures the BOM share. The durability half has no falsifier. Add one? → A: Add a durability falsifier: metric=motion_layer_gross_margin_vs_model_layer_gm_ratio, threshold=<1.0, source=segment_disclosure, op=< — PH Motion Systems margin vs the model-layer margin (NVDA/ISRG software) is retrievable and testable.

- [2026-09-10] Q: T-002 pins constitution 1.2.0 and is marked Stale (re-examination pending gate-5). Its Phase-1 dependency 'T-001 complete' is now satisfied. How should T-002's pin and status be handled? → A: Re-pin to 1.3.0 and set Status to Active — the same treatment as T-001. The §7 Phase-1 dependency 'T-001 complete' is satisfied: T-001 has implemented (24 artifacts), converged clean, and been challenged.
- [2026-09-10] Q: PIL-1 claims 'actuation AND sensing' but the 4-name universe has no sensing-layer name, and T-001's evidence for the sensing BOM share (11-18%) was an unfiled industry estimate. Which names should join T-002's §2 universe? → A: Add all three: AMBA (edge-AI vision silicon — sensing-layer anchor for PIL-1), CGNX (industrial machine vision — automation-side sensing incumbent), and SPCX (end-market compute deployer — demand-side pool: compute-led capex $28.5B H1-2026, 82.7% AI, pulls the upstream layers; one-quarter issuer per the T-001 SPCX artifact). Universe becomes seven names.
- [2026-09-10] Q: All four §2 rows carry an em-dash in the Weight column (the T-001 round-1 question class). What should T-002 declare? → A: Equal weight: seven names at ~14.3% each, continuing the T-001 equal-weight ruling; T-015 overrides with real sizing.
- [2026-09-10] Q: §3 has Depth=deep on supply-chain and unit-economics. T-001's run documented a depth hazard: deep expands to garbage mode names for skills with empty essentials_modes. How should T-002 set Depth? → A: Deep only where safe: supply-chain and unit-economics (empty essentials_modes) go to standard; the deep tier remains available only to skills whose essentials_modes are real mode slugs. §4 note records the hazard.
- [2026-09-10] Q: All 6 subscription tokens are ticker-less (scanner-flagged), and P3 subscribes business-model which is NOT in §3 — the tasks generator reads §3, so P3 generates zero business-model tasks (the T-001 recent-quarter case). Proposed fix: ticker-prefixed subscriptions derived from the matrix, matrix extended to the 3 new names, P3 re-pointed to revenue-decomp (revenue mix shows the model/software layer's share). Adopt? → A: Proposal + business-model row. §3 gains business-model (equity-research-core, standard, PH + ISRG). Matrix rows: supply-chain standard | NVDA, PH, ISRG, AMBA, CGNX, SPCX; unit-economics standard | ISRG, TSLA; competitive-positioning standard | PH, NVDA, AMBA; revenue-decomp standard | PH, ISRG. Subscribed: P1 = PH × supply-chain, AMBA × supply-chain, CGNX × supply-chain, ISRG × unit-economics, TSLA × unit-economics; P2 = PH × supply-chain, AMBA × competitive-positioning, NVDA × competitive-positioning; P3 = PH × revenue-decomp, ISRG × revenue-decomp, PH × business-model, ISRG × business-model.
