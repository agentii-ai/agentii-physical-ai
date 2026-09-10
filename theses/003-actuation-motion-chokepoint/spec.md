# Research Thesis: Actuation and Motion Chokepoint

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 1 — Industry Structure (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
Is actuation the binding chokepoint of humanoid production, and who captures the rent?

**Claim**: Planetary roller screws and harmonic reducers are the tightest chokepoints in the actuator stack, and capacity — not design — sets the ceiling on humanoid output through 2028.

## 1b. Pillars

### Pillar 1 — Roller screws are the single largest BOM line (Priority: P1) 🎯 Minimum Defensible View
Planetary roller screws represent 19-35% of humanoid BOM — more than any other component.

**Why this priority**: Single highest-value component is where pricing power is most likely to reside.

**Independently falsifiable**: A teardown placing screw content below 15% of BOM falsifies it.

**wrong_if**: `metric=planetary_roller_screw_share_of_bom_pct threshold=<15 source=public_teardown op=<`

**Subscribed**: `supply-chain × deep`, `unit-economics × default`

### Pillar 2 — Harmonic reducers are a near-duopoly (Priority: P2)
Precision strain-wave gearing is concentrated in a very small number of suppliers.

**Why this priority**: Duopoly structure is the classic precondition for sustained pricing power.

**Independently falsifiable**: Evidence of three or more qualified suppliers at scale falsifies it.

**wrong_if**: `metric=qualified_strain_wave_reducer_supplier_count threshold=>2 source=industry_technical_disclosure op=>`

**Subscribed**: `competitive × default`, `competitive-positioning × default`

### Pillar 3 — US-listed pure-plays are structurally unanalyzable (Priority: P3)
The actuator pure-play complex (RRX, TKR, ALNT, NOVT, MOG.A, VPG) has no retrievable agentii data, so the layer must be researched by proxy.

**Why this priority**: This is the coverage constraint in action — it forces a documented proxy methodology rather than silent omission.

**Independently falsifiable**: Retrieval of filings or XBRL facts for any of these names falsifies it.

**wrong_if**: `metric=agentii_retrievable_document_count_for_rrx_tkr_alnt threshold=>0 source=search_documents op=>`

**Subscribed**: `risk × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| PH | Motion-control proxy | Industrials | — | Only analyzable large-cap pure motion franchise |
| HON | Automation and sensing | Industrials | — | Adjacent motion and control exposure |
| EMR | Process automation | Industrials | — | Motion and control within automation portfolio |
| ETN | Motion and power | Industrials | — | Electrical and motion content |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `supply-chain` | industry-analysis | deep | PH, HON, EMR, ETN | none | Chokepoint mapping |
| `competitive` | equity-research-core | deep | PH, HON | none | Structure and moat assessment |
| `unit-economics` | business-intelligence | standard | PH | none | Component cost stack |
| `risk` | equity-research-core | standard | PH, EMR | none | Substitution and capacity risk |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
Primary input to T-008. Combined with T-002 to test whether chokepoint position actually converts to margin.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/003-actuation-motion-chokepoint_synthesis.md`
- Snapshot: `snapshots/003-actuation-motion-chokepoint/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Chokepoint inventory | Enumerate actuator components and suppliers | Week 1 | T-001 complete |
| 2 — Capacity analysis | Global capacity vs projected humanoid demand | Week 2 | Phase 1 |
| 3 — Proxy construction | Build the analyzable-proxy methodology | Week 3 | Phase 2 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Planetary roller screws and harmonic reducers are the tightest chokepoints
  in the actuator stack, and capacity — not design — sets the ceiling on humanoid
  output through 2028.
pillars:
- id: PIL-1
  priority: P1
  title: Roller screws are the single largest BOM line
  wrong_if:
    metric: planetary_roller_screw_share_of_bom_pct
    threshold: <15
    source: public_teardown
    op: <
  subscriptions:
  - supply-chain × deep
  - unit-economics × default
- id: PIL-2
  priority: P2
  title: Harmonic reducers are a near-duopoly
  wrong_if:
    metric: qualified_strain_wave_reducer_supplier_count
    threshold: '>2'
    source: industry_technical_disclosure
    op: '>'
  subscriptions:
  - competitive × default
  - competitive-positioning × default
- id: PIL-3
  priority: P3
  title: US-listed pure-plays are structurally unanalyzable
  wrong_if:
    metric: agentii_retrievable_document_count_for_rrx_tkr_alnt
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
