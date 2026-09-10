# Research Thesis: Parker-Hannifin — Motion Control Proxy

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 3 — Company Deep Dives (parallel)
**Time Horizon**: 2026-Q4 → 2029

## 1. Research Question
Does Parker-Hannifin provide genuine, auditable exposure to the humanoid motion-control value pool?

**Claim**: Parker's Motion Systems segment is the only auditable large-cap route into the largest humanoid BOM layer, but the humanoid revenue contribution is currently immaterial to reported results.

## 1b. Pillars

### Pillar 1 — Motion Systems is the analyzable proxy for the largest BOM layer (Priority: P1) 🎯 Minimum Defensible View
Parker's Motion Systems segment maps directly onto the actuation and motion content that teardowns identify as 40-70% of humanoid BOM.

**Why this priority**: It is the only covered name whose disclosed segments isolate this value pool.

**Independently falsifiable**: Segment reorganisation removing Motion Systems disclosure falsifies it.

**wrong_if**: `metric=parker_motion_systems_segment_disclosure_present threshold=1 source=10K_segment_data`

**Subscribed**: `business-model × deep`, `segment data × deep`

### Pillar 2 — Humanoid revenue is immaterial near-term (Priority: P2)
Parker's humanoid exposure is not yet a reportable revenue line and should not be underwritten as a 2026-2027 driver.

**Why this priority**: Prevents the classic error of paying a theme multiple for a segment that has not moved.

**Independently falsifiable**: Disclosed humanoid-attributable revenue above 3% of segment falsifies it.

**wrong_if**: `metric=parker_humanoid_attributable_revenue_share_pct threshold=>3 source=10K_or_transcript_disclosure op=>`

**Subscribed**: `revenue-decomp × deep`, `recent-quarter × default`

### Pillar 3 — Margin structure reflects industrial, not thematic, economics (Priority: P3)
Segment margins should be assessed against industrial peers, not against AI-exposed names.

**Why this priority**: Prevents mis-anchoring the valuation to the wrong comparable set.

**Independently falsifiable**: Segment margin expanding well beyond industrial peer range would falsify it.

**wrong_if**: `metric=motion_systems_segment_operating_margin_vs_industrial_peer_median threshold=parity source=10K_segment_data`

**Subscribed**: `comps × deep`, `ratio-analysis × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| PH | Subject | Industrials | — | Motion pure-play proxy under review |
| EMR | Peer | Industrials | — | Automation peer for margin comparison |
| ETN | Peer | Industrials | — | Electrical peer for margin comparison |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `business-model × deep` | equity-research-core | deep | PH | full | Franchise and segment economics |
| `segment data` | quantitative-analysis | deep | PH | none | Motion Systems isolation |
| `comps` | models-and-pitches | deep | PH, EMR, ETN | none | Industrial peer multiples |
| `recent-quarter` | equity-research-core | standard | PH | none | Latest results and guidance |
| `dcf` | models-and-pitches | full | PH | none | Scenario-weighted valuation |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
The single most important company thesis, because PH is the only auditable route into the largest value pool.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/011-parker-hannifin-motion_synthesis.md`
- Snapshot: `snapshots/011-parker-hannifin-motion/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Segment isolation | Extract Motion Systems financials | Week 1 | T-008 complete |
| 2 — Humanoid bridge | Trace disclosed humanoid-related commentary | Week 2 | Phase 1 |
| 3 — Peer benchmarking | Industrial comps and margin context | Week 3 | Phase 2 |
| 4 — Valuation | Scenario-weighted DCF | Week 4 | Phase 3 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: Parker's Motion Systems segment is the only auditable large-cap route into
  the largest humanoid BOM layer, but the humanoid revenue contribution is currently
  immaterial to reported results.
pillars:
- id: PIL-1
  priority: P1
  title: Motion Systems is the analyzable proxy for the largest BOM layer
  wrong_if:
    metric: parker_motion_systems_segment_disclosure_present
    threshold: '1'
    source: 10K_segment_data
  subscriptions:
  - business-model × deep
  - segment data × deep
- id: PIL-2
  priority: P2
  title: Humanoid revenue is immaterial near-term
  wrong_if:
    metric: parker_humanoid_attributable_revenue_share_pct
    threshold: '>3'
    source: 10K_or_transcript_disclosure
    op: '>'
  subscriptions:
  - revenue-decomp × deep
  - recent-quarter × default
- id: PIL-3
  priority: P3
  title: Margin structure reflects industrial, not thematic, economics
  wrong_if:
    metric: motion_systems_segment_operating_margin_vs_industrial_peer_median
    threshold: parity
    source: 10K_segment_data
  subscriptions:
  - comps × deep
  - ratio-analysis × default
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
