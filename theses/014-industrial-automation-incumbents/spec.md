# Research Thesis: Industrial Automation Incumbents

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 3 — Company Deep Dives (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
Do automation incumbents offer lower-beta, better-audited exposure to physical AI than the pure-play complex?

**Claim**: Automation incumbents monetise physical AI through existing channels with better data quality and lower drawdown risk, at the cost of diluted thematic exposure.

## 1b. Pillars

### Pillar 1 — Incumbents have distribution, not technology leadership (Priority: P1) 🎯 Minimum Defensible View
Established automation vendors reach industrial buyers that pure-plays cannot, but do not lead on humanoid-specific technology.

**Why this priority**: Defines the trade-off explicitly: distribution versus purity.

**Independently falsifiable**: Evidence of incumbents leading humanoid-specific design wins falsifies it.

**wrong_if**: `metric=humanoid_design_wins_by_incumbents_vs_specialists threshold=>1.0 source=design_win_disclosure op=>`

**Subscribed**: `competitive × deep`, `business-model × standard`

### Pillar 2 — Data quality is materially better than pure-plays (Priority: P2)
Incumbents file full segment disclosures with retrievable XBRL facts, unlike the actuator pure-play layer.

**Why this priority**: This is the practical reason to hold them — auditability under P2.

**Independently falsifiable**: Coverage parity for pure-plays falsifies it.

**wrong_if**: `metric=automation_incumbent_agentii_document_count_vs_actuator_pureplays threshold=>1.0 source=search_documents op=>`

**Subscribed**: `segment data × deep`, `business-model × default`

### Pillar 3 — Thematic contribution is diluted below index significance (Priority: P3)
Physical-AI revenue is immaterial to consolidated results for every incumbent in the universe.

**Why this priority**: Prevents the thesis from becoming a low-conviction index proxy.

**Independently falsifiable**: Any incumbent disclosing >5% thematic revenue falsifies it.

**wrong_if**: `metric=incumbent_physical_ai_revenue_share_pct threshold=>5 source=10K_segment_data op=>`

**Subscribed**: `revenue-decomp × deep`, `segment data × deep`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| EMR | Subject | Industrials | — | Process automation incumbent |
| ETN | Subject | Industrials | — | Electrical and motion incumbent |
| HON | Subject | Industrials | — | Controls and automation incumbent |
| DE | Subject | Industrials | — | Precision agriculture autonomy |
| CAT | Subject | Industrials | — | Heavy equipment autonomy |
| GE | Adjacent | Industrials | — | Industrial technology |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `business-model` | equity-research-core | deep | EMR, ETN, HON | none | Incumbent franchise economics |
| `segment data` | quantitative-analysis | deep | EMR, ETN, HON, DE, CAT | none | Thematic revenue isolation |
| `comps` | models-and-pitches | deep | EMR, ETN, HON, DE, CAT | none | Cross-incumbent multiples |
| `ratio-analysis` | quantitative-analysis | standard | EMR, ETN, HON | none | Return and margin profile |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
The diversification counterweight to the pure-play theses. Feeds T-015 as the lower-volatility sleeve.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/014-industrial-automation-incumbents_synthesis.md`
- Snapshot: `snapshots/014-industrial-automation-incumbents/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Thematic isolation | Quantify disclosed physical-AI revenue per name | Week 1 | T-008 complete |
| 2 — Cross-comparison | Rank incumbents on exposure and quality | Week 2 | Phase 1 |
| 3 — Role assignment | Determine portfolio role per name | Week 3 | Phase 2 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Automation incumbents monetise physical AI through existing channels with better
  data quality and lower drawdown risk, at the cost of diluted thematic exposure.
pillars:
- id: PIL-1
  priority: P1
  title: Incumbents have distribution, not technology leadership
  wrong_if:
    metric: humanoid_design_wins_by_incumbents_vs_specialists
    threshold: '>1.0'
    source: design_win_disclosure
    op: '>'
  subscriptions:
  - competitive × deep
  - business-model × standard
- id: PIL-2
  priority: P2
  title: Data quality is materially better than pure-plays
  wrong_if:
    metric: automation_incumbent_agentii_document_count_vs_actuator_pureplays
    threshold: '>1.0'
    source: search_documents
    op: '>'
  subscriptions:
  - segment data × deep
  - business-model × default
- id: PIL-3
  priority: P3
  title: Thematic contribution is diluted below index significance
  wrong_if:
    metric: incumbent_physical_ai_revenue_share_pct
    threshold: '>5'
    source: 10K_segment_data
    op: '>'
  subscriptions:
  - revenue-decomp × deep
  - segment data × deep
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
