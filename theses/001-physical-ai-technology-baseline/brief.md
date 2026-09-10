# Context Brief — Physical AI Technology Baseline (stage-0)

> Q3/Q18: this brief carries **Tier-1 Block-A slices only**. Downstream work keeps
> Tier-2 depth via `get_investment_case(depth=full)`, which returns equally
> `<ref:*>` framed blocks. Q19 framing rules: closed tags share the name of their
> opening tag, `<` is escaped inside blocks, and the tag set is a closed enum.

**corpus_version**: `agentii-2026-09-10` (workspace snapshot at thesis scaffold)
**Retrieved**: 2026-09-10
**Retrieval method**: `retrieve_and_contextualize(ticker=NVDA, domain=fundamental, modes=[frameworks, cases, strategies])`

---

## Reference blocks

<ref:analogue_case id="baillie_gifford__us_equity_growth__nvidia_corporation" entity="NVDA" period="2016-2026" as_of="2026-09-10" retrieved_at="2026-09-10">
Baillie Gifford held NVDA in its US Equity Growth strategy through the AI platform
shift, then **significantly reduced exposure immediately before the 2023-2024 rally** —
the largest absolute advance in the company's history. The position still contributed
meaningfully, but not maximally.

This is the single most instructive analogue for T-001. The firm's research on the
technology was not wrong; its *holding discipline* converted a correct thesis into a
capped outcome. Directly relevant to P5 (horizon discipline) and the T-001 pillar that
the capability inflection arrives 2027-2028 — an investor who de-risks before the
inflection forfeits the thesis.
</ref:analogue_case>

<ref:analogue_case id="kayne_anderson_rudnick__large_cap_core_equity__nvidia_corporation" entity="NVDA" period="2016-2026" as_of="2026-09-10" retrieved_at="2026-09-10">
KARR achieved >900% gross return (~10x MOIC, ~30%+ IRR) but experienced a **-66%
peak-to-trough drawdown in 2022** and began systematically trimming from Q3 2024.

The drawdown figure is the operative datum for T-001's downstream portfolio work: a
thesis with a 10x outcome still imposed a two-thirds drawdown on the way. Reinforces
P7.1 (no leverage) — at 4x, a -66% drawdown is total loss of equity.
</ref:analogue_case>

<ref:analogue_case id="baron_capital__baron_fifth_avenue_growth_strategy__nvidia_corporation" entity="NVDA" period="2016-2024" as_of="2026-09-10" retrieved_at="2026-09-10">
Baron Capital realised **~9,000-10,000% (~100x)** on cost basis from 2016 to mid-2024,
the largest single contributor to strategy performance. Illustrates the payoff
asymmetry available to a holder who correctly identifies a platform shift early and
tolerates the volatility — the outcome P5's 20+ day horizon is designed to permit.
</ref:analogue_case>

<ref:strategy id="med_bio-red-dividend__platform-technology-monetization-via-licensing__s0" fund="bio_red_dividend" era="enduring" as_of="2026-09-10">
**Platform Technology Monetization via Licensing.** Core belief: the highest value in
a novel enabling technology accrues to the *platform owner who solves the fundamental
bottleneck*, not the end-product developer. Licensing foundational IP yields recurring
revenue at lower execution risk than single-product development.

**Relevance to T-001 is structural, not sectoral.** Physical AI has its own candidate
bottlenecks — embodied data, force sensing, actuator transmission. The strategy
supplies the test to apply: does the bottleneck-owner capture the rent, or does the
end-product integrator? T-002, T-003 and T-005 each apply this test to a different
bottleneck.
</ref:strategy>

<ref:strategy id="med_bio-red-dividend__infrastructure-led-health-equity-arbitrage__s1" fund="bio_red_dividend" era="enduring" as_of="2026-09-10">
**Infrastructure-Led Equity Arbitrage.** Core belief: outcomes in a technology wave
are gated by enabling infrastructure (cold chain, logistics, purification) rather than
by the headline product. Value accrues to whoever removes the infrastructure
constraint.

**Direct structural analogue for T-001.** The thesis claim is precisely that embodied
AI is gated by a data-and-motion *infrastructure* constraint, not by model
capability. This strategy is the template for that argument.
</ref:strategy>

---

## Method selection (Q7 — one verdict per strategy candidate)

| strategy id | adopted/rejected | rationale |
|---|---|---|
| `med_bio-red-dividend__platform-technology-monetization-via-licensing__s0` | **adopted** | Supplies the bottleneck-owner test applied in T-002/T-003/T-005. Transfers cleanly: it is a structural claim about where rent accrues, independent of sector. |
| `med_bio-red-dividend__infrastructure-led-health-equity-arbitrage__s1` | **adopted** | Direct template for the claim that an enabling-infrastructure constraint gates the wave. Used to frame T-001 Pillar 1. |
| `med_bio-red-dividend__health-economics-arbitrage-via-qaly-valuation__s0` | **rejected** | Requires regulatory willingness-to-pay thresholds (QALY/ICER). No physical-AI equivalent exists; forcing the analogy would manufacture a false precision. |
| `med_bio-red-dividend__psychoneuroimmunology-psychedelic-revaluation__s0` | **rejected** | Sector-specific regulatory-stigma revaluation. No transferable mechanism to hardware. |
| `med_bio-red-dividend__microbiome-centric-metabolic-lifestyle-intervent__s0` | **rejected** | Domain-specific causal claim; no structural analogue. |
| `<ref:technical_setup>` | **not applicable** | T-001 is `market_data_stage: none`; no price-based entry setup is in scope. Any Phase 5 setup will be sourced then. |

---

## Retrieval keys (Q18)

Mechanical prefilter → pillar FTS → cold-start fallback.

| pillar | retrieval keys | source class |
|---|---|---|
| PIL-1 (data vs compute) | `embodied dataset hours`, `teleoperation cost per hour`, `robot training compute` | industry technical disclosure, company transcripts |
| PIL-2 (actuator BOM share) | `humanoid bill of materials`, `actuator cost share`, `planetary roller screw cost` | teardown, 10-K segment disclosure |
| PIL-3 (manipulation reliability) | `mean time between failures`, `task success rate`, `deployment reliability` | 10-K, earnings transcripts, fleet-operator disclosure |
| PIL-4 (capability timing) | `general purpose humanoid`, `units deployed`, `commercial deployment` | company disclosure, trade press |

**Coverage caveat carried forward from P2.1**: the actuator pure-play complex
(RRX, TKR, ALNT, NOVT, MOG.A, VPG) returns no retrievable filings, documents or XBRL
facts. PIL-2 evidence must therefore come from teardowns and from covered names'
segment disclosures (PH, EMR, ETN, HON). Evidence from uncovered names may inform
context but cannot carry a pillar.

---

## Framing note

The `frameworks` and top-level `strategies` stores returned **empty** for this
domain/ticker combination on 2026-09-10. Case analogues and the two adopted strategies
above were retrieved successfully. This is recorded rather than smoothed over: the
brief's strategy coverage is thinner than the template contemplates, and downstream
converge should re-query rather than assume the store is exhausted.
