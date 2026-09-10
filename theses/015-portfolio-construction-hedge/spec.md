# Research Thesis: Portfolio Construction and Hedge

**Constitution Ref**: workspace/constitution.md (pin `1.2.0`)
**Created**: 2026-09-10
**Status**: Active
**Phase**: 4 — Portfolio (final)
**Time Horizon**: 2026-Q4 → 2029, rebalanced monthly

## 1. Research Question
How should positions be sized and hedged given the macro regime, the concentration limits, and the demonstrated failure modes of the reference fund?

**Claim**: A concentrated but unlevered portfolio of the surviving chokepoint and incumbent names, tail-hedged against multiple compression, delivers the theme with survivable drawdowns.

## 1b. Pillars

### Pillar 1 — The 10Y above 5% is the dominant portfolio risk (Priority: P1) 🎯 Minimum Defensible View
Physical AI is a long-duration theme and a sustained rise in long yields compresses the multiples the portfolio pays.

**Why this priority**: This is a portfolio-level risk that no single-name thesis can mitigate.

**Independently falsifiable**: 10Y sustained below 4.5% for a quarter without multiple expansion falsifies it.

**wrong_if**: `metric=us_10y_treasury_yield_pct threshold=>5.0 source=macro_data op=>`

**Subscribed**: `macro-regime × deep`, `portfolio-hedging × deep`, `risk × deep`

### Pillar 2 — Unlevered concentration survives the reference case's failure modes (Priority: P2)
The Situational Awareness failure was leverage and illiquidity, not thesis error; the P7.1 and P7.2 rules address both mechanically.

**Why this priority**: Directly encodes the lesson of the reference fund's collapse.

**Independently falsifiable**: A drawdown exceeding the modelled maximum despite the constraints falsifies it.

**wrong_if**: `metric=modelled_max_drawdown_under_constitution_constraints_pct threshold=<-35 source=portfolio_simulation op=<`

**Subscribed**: `position-sizing × deep`, `portfolio-hedging × deep`, `risk-and-psychology × default`

### Pillar 3 — Correlation between long and short sleeves must be verified, not assumed (Priority: P3)
The reference fund's longs and shorts were not inversely correlated, so the hedge failed when needed.

**Why this priority**: Prevents repeating the specific structural error that turned a drawdown into a collapse.

**Independently falsifiable**: Measured long/short correlation above 0.3 in a stress window falsifies it.

**wrong_if**: `metric=long_short_sleeve_return_correlation threshold=<0.3 source=portfolio_analysis op=<`

**Subscribed**: `portfolio-hedging × deep`, `risk × default`

### Pillar 4 — Coverage gaps constrain the achievable portfolio (Priority: P4)
The P2 data-plane boundary excludes the largest value pool, so the portfolio is necessarily a proxy portfolio.

**Why this priority**: States the limitation honestly rather than implying full representation.

**Independently falsifiable**: Coverage expansion for actuator pure-plays falsifies it.

**wrong_if**: `metric=investable_universe_coverage_of_physical_ai_value_pool_pct threshold=>50 source=composite_analysis op=>`

**Subscribed**: `position-sizing × default`, `risk × default`


> Delivering P1 alone MUST yield a defensible partial conclusion. Research is
> frequently halted when budget runs out; pillar-ordering guarantees the halt
> point is a deliverable point.

## 2. Universe Definition
| Ticker | Company | Sector | Weight in Thesis | Rationale for Inclusion |
|---|---|---|:---:|---|
| NVDA | Core holding candidate | IT | — | Compute franchise |
| PH | Core holding candidate | Industrials | — | Motion proxy |
| ISRG | Quality anchor | Health Care | — | Proven robotics economics |
| EMR | Incumbent sleeve | Industrials | — | Lower-beta automation |
| ETN | Incumbent sleeve | Industrials | — | Electrical and motion |
| HON | Incumbent sleeve | Industrials | — | Controls |
| TSLA | Optionality sleeve | Cons Disc | — | Humanoid option |
| AMBA | Satellite | IT | — | Edge vision |

## 3. Skill Deployment Matrix
| Skill | Vertical | Depth | Tickers | Market Data Stage (Q41) | Purpose |
|---|---|:---:|---|---|---|
| `portfolio-hedging` | portfolio-strategy | deep | NVDA, PH, ISRG, EMR, ETN, HON, TSLA, AMBA | none | Hedge construction and correlation |
| `position-sizing` | portfolio-strategy | deep | NVDA, PH, ISRG, EMR, ETN, HON, TSLA, AMBA | none | Sizing under P7 constraints |
| `risk` | equity-research-core | deep | NVDA, PH, ISRG, EMR, ETN, HON, TSLA, AMBA | none | Portfolio-level risk aggregation |
| `risk-and-psychology` | risk-and-psychology | standard | NVDA, PH, ISRG, EMR, ETN, HON, TSLA, AMBA | none | Drawdown behaviour and discipline |
| `macro-regime` | macro-strategy | deep | NVDA, PH, ISRG, EMR, ETN, HON, TSLA, AMBA | none | Regime-conditional allocation |

## 4. Depth Tiers
| Tier | Skills | mode-set | Tickers | Output |
|:---:|------|---|--------|------|
| Deep | pillars at P1 | skill `essentials_modes` | as listed | full artifact set |
| Full | all pillars | all modes (Q79 expansion) | as listed | complete + cross-checks |

## 5. Cross-Cutting Analysis
Final synthesis. Consumes every prior thesis. Produces the staged order set, which hard-fails on any unratified or superseded constitution pin.

## 6. Output Contract
- Per-Ticker: `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md`
- Cross-Stock: `_cross/015-portfolio-construction-hedge_synthesis.md`
- Snapshot: `snapshots/015-portfolio-construction-hedge/YYYY-MM-DD_thesis.md`

## 7. Thesis Phases
| Phase | Tasks | Duration | Dependencies |
|:---:|------|:---:|------|
| 1 — Survivor selection | Names passing T-008 and their own deep dives | Week 1 | T-009…T-014 complete |
| 2 — Sizing | Apply P7.1, P7.2, and concentration limits | Week 2 | Phase 1 |
| 3 — Hedge design | Tail hedge against multiple compression | Week 3 | Phase 2 |
| 4 — Stress test | Model drawdowns against the reference case | Week 4 | Phase 3 |

**frontmatter** (thesis.md, machine-read):
```yaml
claim: A concentrated but unlevered portfolio of the surviving chokepoint and incumbent
  names, tail-hedged against multiple compression, delivers the theme with survivable
  drawdowns.
pillars:
- id: PIL-1
  priority: P1
  title: The 10Y above 5% is the dominant portfolio risk
  wrong_if:
    metric: us_10y_treasury_yield_pct
    threshold: '>5.0'
    source: macro_data
    op: '>'
  subscriptions:
  - macro-regime × deep
  - portfolio-hedging × deep
  - risk × deep
- id: PIL-2
  priority: P2
  title: Unlevered concentration survives the reference case's failure modes
  wrong_if:
    metric: modelled_max_drawdown_under_constitution_constraints_pct
    threshold: <-35
    source: portfolio_simulation
    op: <
  subscriptions:
  - position-sizing × deep
  - portfolio-hedging × deep
  - risk-and-psychology × default
- id: PIL-3
  priority: P3
  title: Correlation between long and short sleeves must be verified, not assumed
  wrong_if:
    metric: long_short_sleeve_return_correlation
    threshold: <0.3
    source: portfolio_analysis
    op: <
  subscriptions:
  - portfolio-hedging × deep
  - risk × default
- id: PIL-4
  priority: P4
  title: Coverage gaps constrain the achievable portfolio
  wrong_if:
    metric: investable_universe_coverage_of_physical_ai_value_pool_pct
    threshold: '>50'
    source: composite_analysis
    op: '>'
  subscriptions:
  - position-sizing × default
  - risk × default
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
