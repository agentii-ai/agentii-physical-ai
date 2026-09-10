<!--
Sync Impact Report (spec 046 Q33 — executable input, not decoration):
  version: 0.1.0-unratified → 1.0.0 → 1.1.0 → 1.2.0
  amended: P2 Coverage-Bounded Universe — covered set corrected from 12 to 15 names
           (PH, ON, AMBA reinstated; ISRG/QCOM confirmed); P2.1 added
  amended2: P2 universe widened 15 → ~30 names after second retrieval sweep;
           P7.1 (no leverage) and P7.2 (liquidity) added from the Aschenbrenner precedent
  added: P1 Research Scope, P2 Coverage-Bounded Universe, P2.1 Coverage-verification
         rule, P3 First-Principles Technology Analysis, P4 Fact Audit Mandate,
         P5 Horizon Discipline, P6 English-First, P7 Risk Envelope
  removed: —
  deferred: (a) Sector WACC bands are provisional pending a ratified
            assumptions.yaml review; (b) an explicit rare-earth / critical-minerals
            supply-shock trigger is not yet wired into drift_triggers.
  Re-examination scope: initial ratification — no prior theses exist to re-examine.
-->

# Investment Constitution — Physical AI — US Equity Research

**CONSTITUTION_VERSION**: 1.2.0
**RATIFICATION_DATE**: 2026-09-10
**LAST_AMENDED_DATE**: 2026-09-10

> Drafted by agent from researched evidence on 2026-09-10 and ratified by the
> workspace owner on the same date. All bracketed placeholders have been replaced;
> `constitution_pin` moves from `unratified` to `1.0.0`.

## P1 — Research Scope

Physical AI: humanoid robotics, embodied AI, the AI data and foundation-model layer
that drives them, and the upstream/downstream supply chain. Scope is defined by
**function in the physical-AI value chain**, not by GICS sector.

## P2 — Coverage-Bounded Universe (binding constraint)

The investable universe is **the intersection of (a) the physical-AI value chain and
(b) the agentii.ai data plane**. A name with no agentii coverage cannot be audited and
therefore **cannot be researched, sized, or held**. Findings from other sources may
motivate a *watchlist* entry but never a position.

Verified 2026-09-10 by direct retrieval (see the methodological rule below). The
analyzable universe is **~30 names** — materially wider than the first pass suggested:

| Layer | Analyzable tickers |
|---|---|
| Compute / model | NVDA, QCOM, INTC, TSM, TER, KLAC, LRCX |
| Analog / power / memory | ADI, MPWR, TXN, NXPI, ON, MU |
| Vision / sensing / autonomy | AMBA, CGNX, MBLY |
| Motion / automation | PH, EMR, ETN, HON, APH, GE, MMM, DE, CAT |
| Robotics / medical / end-market | ISRG, SYK, AMZN, F, TSLA |

**Not retrievable** (13): RRX, TKR, ALNT, NOVT, MOG.A, VPG, ROK, SYM, MP, ZBRA, MDT,
TDY, TEL.

The uncovered set includes the **entire actuator and motion-control pure-play layer**
(RRX, TKR, ALNT, NOVT, MOG.A, VPG) — which BOM teardowns place at 40–70% of humanoid
cost, and which sell-side work most often recommends. This gap is addressed by the
dedicated watchlist thesis (`007-uncovered-actuator-watchlist`), not by relaxing P2.

> ⚠️ **Fuzzy-match hazard**: `search_xbrl_facts(ticker="ALNT")` returns **ALNY**
> (Alnylam) — a different company. Every ticker must be confirmed against
> `get_ticker_coverage` before its facts are used. Silent ticker substitution is a
> `SCHEMA_MISMATCH`-class error and voids the artifact.

### P2.1 — Coverage-verification rule (mandatory; added after a near-miss)

Absence of data must never be concluded from an indirect signal. The 2026-09-10
reconnaissance produced a **false negative on PH, ON, ISRG, QCOM, and AMBA** by
reading the bulk `list_coverage` table and probing a single XBRL concept. Both signals
were unsound:

- **`list_coverage` (bulk) is unreliable.** It omits tickers that demonstrably have
  data — `TSLA` is absent from it yet carries 63,523 XBRL facts — and it labels
  `ON`/`PH` with zero `xbrl_filings` despite both returning facts. Treat it as a hint,
  never as evidence.
- **One concept is not a coverage test.** Issuers tag revenue as
  `RevenueFromContractWithCustomerExcludingAssessedTax` (129 tickers) far more often
  than `Revenues` (89 tickers). Probing only `Revenues` returns a false zero.

Therefore, before any ticker is declared out of universe, it must satisfy **all three**:

1. `search_sec_filings` returns nothing, **and**
2. `search_documents` returns nothing, **and**
3. `search_xbrl_facts` returns nothing **for at least two revenue concepts**
   (`RevenueFromContractWithCustomerExcludingAssessedTax` and `Revenues`).

Where the three disagree, **retrieval wins over metadata**. A name is "analyzable" the
moment facts come back, regardless of what any coverage table or index reports. Record
the evidence (endpoint + count + date) in the artifact.

## P3 — First-Principles Technology Analysis

Physical AI is a disruptive innovation; trailing multiples are uninformative for the
pure-play layer. Theses must reason from **physics, materials science, and
engineering** — actuator torque density, BOM cost curves, rare-earth intensity,
battery energy density, manufacturing yield — and forecast from those primitives.
R&D progress disclosed in filings is primary evidence; sell-side narrative is not.

## P4 — Fact Audit Mandate

Every material financial claim must trace to agent-use-ready data retrieved from
agentii.ai (SEC filings, XBRL facts, earnings calendar), cited inline as
`agentii.ai/v/{ticker}/{citation_id}/{page}`. Unsourced quantitative claims are
`UNFRAMED_REFERENCE` and block artifact release.

## P5 — Horizon Discipline

Holding period is **≥ 20 trading days**. Positioning is driven by dated catalysts and
disclosed R&D facts, not price momentum. Price-based exits are limited to thesis
invalidation.

## P6 — English-First

**English is the sole working language.** Any Chinese-language input from the
workspace owner, and any Chinese arising mid-process, is translated into precise
professional English and carried forward in English. Artifacts, filenames, commits,
and citations are English-only. Translations must preserve technical precision —
term-of-art accuracy over literal rendering.

## P7 — Risk Envelope

Position limits, stop discipline, and concentration caps are declared in
`constitution.yaml` and enforced mechanically. Values are not renegotiated inside a
thesis.

### P7.1 — No leverage

**The portfolio operates unlevered.** No margin, no options-based implicit leverage,
no borrowing against positions. This is not a risk-preference statement; it is a rule
written from a specific failure.

The Situational Awareness fund (Aschenbrenner, 2024–2026) held a **directionally
correct** thesis — AI's physical infrastructure bottleneck — and was destroyed by
execution: ~4x leverage, concentrated positions, and correlated longs and shorts. It
lost **67% in July 2026** and sold its public book to Citadel at a >10% discount.
A correct thesis at 4x is still a blown-up fund.

Research quality does not protect against leverage. Our edge is analytical, not
financing — so we do not finance.

### P7.2 — Liquidity

No position may exceed **15% of 20-day average daily volume**. The reference fund's
terminal failure was $45B trapped in small/mid-cap names that could not be exited
without moving the market. A position we cannot leave is not a position we hold.

## Macro Regime (updated monthly)

- **Regime**: EXPANSION — **late-cycle and inflation-constrained**
- **Portfolio Bias**: NET_LONG, with a tail hedge against multiple compression
- **Key Leading Indicators**: ISM Manufacturing PMI **54.6** (Aug 2026, 8th month
  expansion, down from 55.6); 10Y–2Y spread **+41bp** (10Y 4.83% / 2Y 4.43%, positively
  sloped); HY credit spread **265bp OAS** (historically tight)

**Regime tension — the central risk to this theme.** Growth is expanding and credit
is priced for perfection, but inflation is above target (CPI 3.4%, PCE 3.7%) and the
Fed under Chair Warsh has held at 3.50–3.75% with markets pricing a **~60% chance of
a 25bp hike** at the 2026-09-16 FOMC. Physical AI is a long-duration, capex-heavy
theme; a hiking cycle compresses exactly the multiples this portfolio pays. **A hike
is not a thesis falsifier for any single name but is a portfolio-level de-rating
risk** — it is the primary reason the tail hedge is mandatory rather than optional.

## Sector Preferences

Sector tagging is by GICS for constraint arithmetic, but conviction is driven by
value-chain position.

| Sector | Bias | Conviction | Rationale |
|--------|------|:---:|------|
| Information Technology | OVERWEIGHT | HIGH | Compute/model layer (NVDA, QCOM) plus vision and motion silicon (CGNX, TER, ADI, MPWR) — the deepest agentii coverage and the clearest earnings linkage |
| Industrials | OVERWEIGHT | MEDIUM | Automation incumbents (DE, CAT, EMR, ETN, ISRG) monetising physical AI through existing channels; lower beta to the theme, higher data quality |
| Consumer Discretionary | NEUTRAL | LOW | TSLA is the only covered pure-play humanoid proxy but is a diversified auto/energy business |
| Materials | UNDERWEIGHT | LOW | Rare-earth economics are presently adverse (see below) and agentii coverage is near-zero |

## Research Scope Constraints

- **Market Cap**: $100M – $2T (all caps; $100M floor excludes shells and sub-scale issuers)
- **Regions**: United States, including ADRs of foreign issuers
- **Sectors Out of Scope**: None categorically — thematic scope spans GICS sectors
- **Max Concurrent Positions**: 12

## Risk Framework

- **Single Position**: 8% default, 4% binary catalyst, 12% max
- **Sector Concentration**: ≤ 40% any single GICS sector
- **Macro-Driven Exposure**: ≤ 30% total
- **Stop-Loss**: −30% thesis invalidation; −18% technical invalidation

## Methodology Foundation

- **Equity Research**: Agentii three-layer retrieval protocol (Document Discovery →
  Page Map → Deep Read), escalating to deep outline when table-level disambiguation
  is required
- **Valuation**: Scenario-weighted DCF + risk-adjusted NPV (rNPV) for pre-revenue and
  early-revenue names; comps as a cross-check, never as the primary method
- **Catalyst Requirement**: Dateable catalyst within 180 days for any trade idea

## Critical-Minerals Note (thesis input, not a constraint)

Actuators are ~40–60% of humanoid BOM and are rare-earth-magnet intensive. NdPr oxide
traded at **~$107/kg (China domestic) and ~$95–110/kg ex-China** in August 2026 —
**below the $110/kg DoD price floor** set for MP Materials and Lynas — on ex-China
oversupply. This is bearish for rare-earth miners and structurally *favourable* for
actuator cost curves. It inverts the intuitive "own the materials" trade and is a
worked example of P3 reasoning: the first-principles read contradicts the narrative.

---

*SemVer rules (Q33): MAJOR = a principle removed or incompatibly redefined; MINOR =
a principle added or substantially extended; PATCH = wording only. MAJOR/MINOR bumps
mark `constitution_pin`-older theses `stale` and dispatch re-examination after the
gate-5 budget confirm. PATCH never triggers review.*

<!--
Sync Impact Report entry
  bump: minor
  note: P2 corrected: universe expanded 12 -> 15 covered names (PH, ON, AMBA reinstated; ISRG/QCOM confirmed). Root cause of prior error: coverage was tested with a single XBRL concept 'Revenues', but issuers tagging RevenueFromContractWithCustomerExcludingAssessedTax returned false zeros. P2 now mandates querying facts, not reading the bulk list_coverage table, and never concluding absence from one concept. Tier A/B collapse into one tier; genuinely absent set reduced to 9 names.
  old → new: [record changed principles here]
  deferred: [none]
-->
