# Research Thesis: Critical Materials and Rare Earths

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 1 — Industry Structure (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
Does rare-earth supply gate actuator scaling, and does current pricing support or contradict the materials thesis?

**Claim**: Current NdPr pricing is below the US DoD support floor, which is bearish for rare-earth miners and simultaneously removes a feared cost headwind from actuator economics.

## 1b. Pillars

### Pillar 1 — NdPr is priced below the DoD floor (Priority: P1) 🎯 Minimum Defensible View
Ex-China NdPr oxide traded at roughly $95-110/kg in August 2026, beneath the $110/kg floor underpinning US producer agreements.

**Why this priority**: Inverts the intuitive 'own the materials' trade and is a direct P3 first-principles test.

**Independently falsifiable**: Sustained NdPr pricing above $130/kg falsifies it.

**wrong_if**: `metric=ndpr_oxide_price_usd_per_kg threshold=>130 source=benchmark_price_assessment op=>`

**Subscribed**: `sector-overview × default`, `supply-chain × default`

### Pillar 2 — Chinese magnet export controls are the real tail risk (Priority: P2)
The binding supply risk is policy-driven export restriction of rare-earth magnets, not geological scarcity.

**Why this priority**: Reframes the risk from commodity price to geopolitical access.

**Independently falsifiable**: Formal relaxation of export controls without price impact falsifies it.

**wrong_if**: `metric=magnet_export_control_events_per_year threshold=>0 source=trade_policy_disclosure`

**Subscribed**: `risk × deep`, `supply-chain × default`

### Pillar 3 — The materials layer is effectively uninvestable via agentii (Priority: P3)
MP Materials and peer rare-earth names lack retrievable agentii coverage, so the layer cannot be audited.

**Why this priority**: Documents the boundary of the data plane honestly rather than implying false precision.

**Independently falsifiable**: Retrievable coverage for MP or a peer falsifies it.

**wrong_if**: `metric=agentii_retrievable_document_count_for_mp threshold=>0 source=search_documents op=>`

**Subscribed**: `risk × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| PH | Rare-earth cost exposure | Industrials | — | Actuator and motor magnet consumption |
| ETN | Electrical materials | Industrials | — | Magnet and conductor content |
| HON | Materials and controls | Industrials | — | Supply-chain materials exposure |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `supply-chain` | industry-analysis | deep | PH, ETN, HON | none | Materials dependency mapping |
| `risk` | equity-research-core | deep | PH, ETN | none | Supply and policy risk |
| `sector-overview` | industry-analysis | standard | PH | none | Materials sector structure |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
Feeds T-008. The pricing inversion here is the clearest example of the P3 method producing a contrarian read.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/006-critical-materials-rare-earth_synthesis.md`
- Snapshot: `snapshots/006-critical-materials-rare-earth/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Price baseline | Establish current NdPr and magnet pricing | Week 1 | T-001 complete |
| 2 — Policy mapping | Export-control regime and DoD floor terms | Week 2 | Phase 1 |
| 3 — Pass-through | How materials cost reaches actuator economics | Week 3 | Phase 2 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Current NdPr pricing is below the US DoD support floor, which is bearish for
  rare-earth miners and simultaneously removes a feared cost headwind from actuator
  economics.
pillars:
- id: PIL-1
  priority: P1
  title: NdPr is priced below the DoD floor
  wrong_if:
    metric: ndpr_oxide_price_usd_per_kg
    threshold: '>130'
    source: benchmark_price_assessment
    op: '>'
  subscriptions:
  - sector-overview × default
  - supply-chain × default
- id: PIL-2
  priority: P2
  title: Chinese magnet export controls are the real tail risk
  wrong_if:
    metric: magnet_export_control_events_per_year
    threshold: '>0'
    source: trade_policy_disclosure
  subscriptions:
  - risk × deep
  - supply-chain × default
- id: PIL-3
  priority: P3
  title: The materials layer is effectively uninvestable via agentii
  wrong_if:
    metric: agentii_retrievable_document_count_for_mp
    threshold: '>0'
    source: search_documents
    op: '>'
  subscriptions:
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
