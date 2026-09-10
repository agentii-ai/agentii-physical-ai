# Research Thesis: Uncovered Actuator Watchlist

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 1 — Industry Structure (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
What is the investment case for the actuator pure-play layer, and precisely why can we not audit it through agentii?

**Claim**: The actuator pure-play complex is the consensus picks-and-shovels trade for physical AI, yet none of it is retrievable through the agentii data plane — a structural gap that must be documented, not silently omitted.

## 1b. Pillars

### Pillar 1 — RRX, TKR and ALNT are the consensus actuator complex (Priority: P1) 🎯 Minimum Defensible View
Sell-side work names Regal Rexnord, Timken and Allient as the primary US-listed picks-and-shovels beneficiaries.

**Why this priority**: They occupy the value pool our own BOM research identifies as largest, so their absence from the universe is a material limitation.

**Independently falsifiable**: If the consensus complex turns out to be outside the actual value pool, this pillar fails.

**wrong_if**: `metric=agentii_retrievable_document_count_for_rrx_tkr_alnt threshold=>0 source=search_documents op=>`

**Subscribed**: `external screening × default`

### Pillar 2 — PH is the only analyzable motion-control proxy (Priority: P2)
Parker-Hannifin provides retrievable segment-level Motion Systems data and is the sole covered large-cap pure motion franchise.

**Why this priority**: It is the only route to auditable exposure to the largest BOM layer.

**Independently falsifiable**: Another covered motion pure-play appearing falsifies it.

**wrong_if**: `metric=covered_us_listed_motion_pureplay_count threshold=>1 source=search_documents op=>`

**Subscribed**: `business-model × deep`, `segment data × default`

### Pillar 3 — The coverage gap is structural, not incidental (Priority: P3)
Uncovered names share no retrievable filings, documents, or XBRL facts across at least two revenue concepts — this is a data-plane boundary.

**Why this priority**: Distinguishes a genuine coverage boundary from a query error, which this workspace has already made once.

**Independently falsifiable**: Retrieval succeeding on any listed name falsifies it.

**wrong_if**: `metric=uncovered_actuator_names_returning_filings_documents_or_facts threshold=>0 source=search_sec_filings AND search_documents AND search_xbrl_facts op=>`

**Subscribed**: `risk × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| PH | Analyzable proxy | Industrials | — | Only covered motion pure-play |
| EMR | Automation adjacency | Industrials | — | Motion within broader automation |
| HON | Motion and controls | Industrials | — | Adjacent motion exposure |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `business-model` | equity-research-core | deep | PH | none | Proxy franchise economics |
| `segment data` | quantitative-analysis | deep | PH, EMR | none | Motion segment isolation |
| `risk` | equity-research-core | standard | PH, EMR, HON | none | Coverage and proxy risk |
| `competitive` | equity-research-core | standard | PH | none | Motion competitive structure |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
Produces the coverage-gap register and a data-acquisition request. Escalate to agentii.ai as a coverage expansion case — the value pool is identified but unauditable.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/007-uncovered-actuator-watchlist_synthesis.md`
- Snapshot: `snapshots/007-uncovered-actuator-watchlist/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Consensus mapping | Document the sell-side picks-and-shovels complex | Week 1 | T-001 complete |
| 2 — Three-check verification | Apply the P2.1 rule to every uncovered name | Week 2 | Phase 1 |
| 3 — Proxy validation | Confirm PH's segment data actually isolates Motion Systems | Week 3 | Phase 2 |
| 4 — Escalation | File the coverage-expansion request with evidence | Week 4 | Phase 3 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: The actuator pure-play complex is the consensus picks-and-shovels trade for
  physical AI, yet none of it is retrievable through the agentii data plane — a structural
  gap that must be documented, not silently omitted.
pillars:
- id: PIL-1
  priority: P1
  title: RRX, TKR and ALNT are the consensus actuator complex
  wrong_if:
    metric: agentii_retrievable_document_count_for_rrx_tkr_alnt
    threshold: '>0'
    source: search_documents
    op: '>'
  subscriptions:
  - external screening × default
- id: PIL-2
  priority: P2
  title: PH is the only analyzable motion-control proxy
  wrong_if:
    metric: covered_us_listed_motion_pureplay_count
    threshold: '>1'
    source: search_documents
    op: '>'
  subscriptions:
  - business-model × deep
  - segment data × default
- id: PIL-3
  priority: P3
  title: The coverage gap is structural, not incidental
  wrong_if:
    metric: uncovered_actuator_names_returning_filings_documents_or_facts
    threshold: '>0'
    source: search_sec_filings AND search_documents AND search_xbrl_facts
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
