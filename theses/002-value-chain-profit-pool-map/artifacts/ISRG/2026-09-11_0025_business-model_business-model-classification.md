---
artifact_id: "002-ISRG-business-model-business-model-classification-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: ISRG
skill: business-model
mode: business-model-classification
affix: ""
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "9479220eef91"
as_of: 2026-09-11
entity_claims:
  - entity: ISRG
    metric: product_gross_margin_pct
    value: 66.3
    unit: pct
    period: FY2025
    source: "10-K:page79"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: recurring_revenue_share_pct
    value: 84
    unit: pct
    period: FY2025
    source: "10-K:page78"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: installed_base_units
    value: 12101
    unit: units
    period: FY2025
    source: "10-K:page69"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: revenue_per_procedure_usd
    value: 1826
    unit: USD
    period: FY2025
    source: "derived: 10-K:page69 + 10-K:page77"
    retrieved_at: 2026-09-11
citations:
  - "sec166 (FY2025 10-K, filed 2026-02-03, accession 0001035267-26-000010)"
  - "sec172 (Q2-2026 10-Q, filed 2026-07-21, accession 0001035267-26-000058)"
  - "XBRL isrg-20251231.htm (source_authority 3)"
pillars_addressed: [PIL-3]
claim_state: pinned
key_metrics:
  fy2025_revenue_usd: 10064700000
  recurring_revenue_share_pct: 84
  installed_base_units: 12101
  product_gross_margin_pct: 66.3
  consolidated_gross_margin_pct: 66.0
conclusions:
  - "Business model: premium capital-equipment product business with razor-razorblade recurring stream; 84% of FY2025 revenue is recurring (I&A + service + operating-lease)."
  - "Model layer on-device compute is enormous (da Vinci 5 >10,000x dv Xi), but the disclosed digital-subscription slice (My Intuitive+) is not material revenue — PIL-3 subscription-case input lands in mode revenue-composition-and-concentration."
facts_count: 14
deducted_count: 2
views_count: 2
citation_count: 25
---

# ISRG — Business Model & Offerings Classification (mode 1_1)

## Executive Summary

Intuitive Surgical is a premium **product** company (robotic surgical systems) whose economic engine is a **razor-razorblade recurring stream**: 84% of FY2025 revenue ($8,465.3M of $10,064.7M) recurs from instruments & accessories, service contracts, and operating leases [FACT] [https://agentii.ai/v/ISRG/sec166/page78]. The installed base of 12,101 systems (11,106 da Vinci + 995 Ion) generates per-procedure I&A revenue of ~$1,826 [DEDUCTED] [https://agentii.ai/v/ISRG/sec166/page69]. Product gross margin is 66.3% — premium, high-end positioning [FACT] [https://agentii.ai/v/ISRG/sec166/page79]. The software/digital layer (My Intuitive+, Case Insights, SimNow) is real on-device compute — da Vinci 5 has >10,000x the computing power of da Vinci Xi — but is disclosed as **not material revenue** [FACT] [https://agentii.ai/v/ISRG/sec166/page8], [https://agentii.ai/v/ISRG/sec166/page77]. Classification verdict: capital-equipment + recurring-consumables + service hybrid; subscription (software) revenue exists per-unit only inside service contracts and non-material digital offerings — the direct PIL-3 input quantified in mode 3.

## Mode 1_1 — Business Model Classification

**Business Model: Product (capital equipment) with razor-razorblade recurring overlay**

The offering stack is explicitly an "ecosystem that includes robotic-assisted systems, instruments and accessories, customer learning, and customer support services all connected by a digital portfolio" [FACT] [https://agentii.ai/v/ISRG/sec166/page7]. Revenue is recognized across three disclosed lines: Systems (up-front capital), Instruments & Accessories (consumables), Service (contracts) [FACT] [https://agentii.ai/v/ISRG/sec166/page77].

Three revenue engines [FACT]:
1. **Capital**: da Vinci systems sell for $0.7M–$3.1M each; Ion $500K–$815K [https://agentii.ai/v/ISRG/sec166/page77].
2. **Consumables (razorblades)**: I&A generates $900–$3,700 per procedure, driven by instrument expiry/wear [https://agentii.ai/v/ISRG/sec166/page77].
3. **Recurring contracts**: service contracts $95K–$225K per system per year; operating leases (fixed-payment and usage-based) place the system itself into a subscription stream [https://agentii.ai/v/ISRG/sec166/page77], [https://agentii.ai/v/ISRG/sec166/page74].

FY2025 mix: I&A 59.8%, Systems 24.6%, Service 15.6% of revenue [DEDUCTED from XBRL: Systems $2,473.7M / I&A $6,018.9M / Service $1,572.1M vs total $10,064.7M, isrg-20251231.htm source_authority 3] [https://agentii.ai/v/ISRG/sec166/page77]. Recurring revenue (I&A + service + operating-lease revenue) = $8,465.3M = 84% of total [FACT] [https://agentii.ai/v/ISRG/sec166/page78].

**Core Offering**: da Vinci multi-port/single-port robotic surgical systems (5 generations: Si → X/Xi/SP → da Vinci 5) plus the Ion endoluminal lung-biopsy platform; consumable instruments (SureForm staplers, Vessel Sealer Extend, SynchroSeal) [FACT] [https://agentii.ai/v/ISRG/sec166/page8], [https://agentii.ai/v/ISRG/sec166/page9].

**Positioning: High-end** — da Vinci 5 targets the complex-procedure segment; da Vinci X is the price-sensitive market variant [FACT] [https://agentii.ai/v/ISRG/sec166/page76]. Evidence: 66.0% consolidated gross margin FY2025 (67.5% FY2024); 66.3% product GM; 64.6% service GM [FACT] [https://agentii.ai/v/ISRG/sec166/page69], [https://agentii.ai/v/ISRG/sec166/page79]. Premium pricing power is sustained by the installed base: 3,153,000 da Vinci procedures (+18% YoY) in FY2025 [FACT] [https://agentii.ai/v/ISRG/sec166/page69].

**Platform / software layer (PIL-3 context)**: da Vinci 5 "has more than 10,000 times the computing power of da Vinci Xi," integrating My Intuitive app, SimNow, Case Insights, and Intuitive Hub (edge computing system) [FACT] [https://agentii.ai/v/ISRG/sec166/page8]. My Intuitive+ is "a digital subscription package available with the da Vinci 5 platform" [FACT] [https://agentii.ai/v/ISRG/sec166/page11]. Yet: "we provide a portfolio of learning offerings and digital solutions. We do not currently generate material revenue from these offerings" [FACT] [https://agentii.ai/v/ISRG/sec166/page77]. The classification-relevant finding: ISRG monetizes compute through hardware+service bundles, not standalone software subscription.

**Single segment**: the company operates one reportable segment [FACT] [https://agentii.ai/v/ISRG/sec166/page124]; no divisional P&L exists. Revenue is disaggregated by product line and U.S./OUS only [https://agentii.ai/v/ISRG/sec166/page108].

**[VIEW]** The model is a hybrid: product-type revenue recognition (up-front system sales, consumable purchases) dominates the P&L, but the recurring overlay (84%) behaves like a subscription business — the defining characteristic for PIL-3's subscription-case test. **[VIEW]** The "model layer" (software/AI) is embedded in hardware with zero standalone disclosed revenue; its monetization is indirect through system ASPs ($1.60M FY2025) and service contracts.

## Coverage Gaps & Citations

- **Digital/subscription revenue split**: no dollar amount disclosed for My Intuitive+ or digital solutions — only "not material" [https://agentii.ai/v/ISRG/sec166/page77]. Per-unit subscription slice is proxied via service contracts in mode 3.
- **Segment-level P&L**: single reportable segment; no product-line operating margin disclosed (only gross margins).
- **ASP composition**: da Vinci ASP $1.60M FY2025 excludes leases/Ion/trade-ins — not comparable to pure hardware price [https://agentii.ai/v/ISRG/sec166/page78].
- **Fiscal-calendar metadata**: `get_company_fiscal_calendar` returns year-end month 1, but XBRL facts and filings are calendar-year (isrg-20251231.htm, sec166) — calendar-year used throughout; metadata inconsistency flagged.

**Citations (roll-up)**: sec166 pages 7, 8, 9, 11, 14, 69, 74, 76, 77, 78, 79, 108, 124; sec172 pages 32, 40; XBRL isrg-20251231.htm. Full links inline above.

## Verification Table (number → tool call)

| Number | Value | Tool call |
|---|---|---|
| FY2025 total revenue | $10,064.7M | search_xbrl_facts (isrg-20251231.htm, authority 3) + sec166 page77 |
| FY2025 I&A / Systems / Service | $6,018.9M / $2,473.7M / $1,572.1M | sec166 page77; XBRL detailed view (ProductOrServiceAxis) |
| Recurring revenue % | 84% ($8,465.3M) | sec166 page78 |
| Installed base 12/31/25 | 11,106 dv + 995 Ion = 12,101 | sec166 page69 |
| Product / service / consolidated GM | 66.3% / 64.6% / 66.0% | sec166 page79, page69 |
| System price range | $0.7M–$3.1M (Ion $500K–$815K) | sec166 page77 |
| Service contract fee | $95K–$225K/system/year | sec166 page77 |
| I&A per procedure | $900–$3,700; implied $1,826 | sec166 page77; derived from page69 |
| da Vinci 5 compute | >10,000x dv Xi | sec166 page8 |
| Q2-2026 revenue / recurring | $2,892.3M / 85% | sec172 page32, page40 |
