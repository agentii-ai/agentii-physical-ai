---
artifact_id: "002-PH-business-model-distribution-channel-analysis-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: PH
skill: business-model
mode: distribution-channel-analysis
affix: ""
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "9479220eef91"
as_of: 2026-09-11
entity_claims:
  - entity: PH
    metric: motion_systems_revenue_usd
    value: 3580000000
    unit: USD
    period: FY2026
    source: "10-K:page44:sec166"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: diversified_industrial_segment_operating_margin_pct
    value: 23.8
    unit: pct
    period: FY2026
    source: "10-K:page25:sec166"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: consolidated_gross_margin_pct
    value: 37.7
    unit: pct
    period: FY2026
    source: "10-K:page23:sec166"
    retrieved_at: 2026-09-11
citations:
  - "sec166:page3"
  - "sec166:page4"
  - "sec166:page5"
  - "sec166:page19"
  - "sec166:page23"
  - "sec166:page25"
  - "sec166:page26"
  - "sec166:page44"
  - "sec166:page66"
  - "ect72:page1"
  - "ect72:page2"
pillars_addressed: [PIL-3]
claim_state: pinned
key_metrics:
  manufacturing_plants: 323
  countries_with_facilities: 43
  di_north_america_net_sales_usd: 8392000000
  di_international_net_sales_usd: 6046000000
  sgna_percent_of_sales: 16.1
conclusions:
  - "Distribution model is a hybrid: DI sells direct to OEMs plus through independent distributors via field sales; Aerospace is direct-only to OEMs and end users."
  - "No quantitative direct:indirect channel split is disclosed by Parker — channel mix must be treated as qualitative-only (coverage gap)."
  - "Distribution reach is a disclosed competitive factor; channel breadth is extreme (several hundred thousand OEM/distributor locations)."
  - "Aerospace direct model correlates with higher segment margin (26.0%) vs DI's hybrid 23.8%, consistent with OEM-direct pricing power plus aftermarket control."
facts_count: 24
deducted_count: 3
views_count: 3
citation_count: 11
---

# PH — Distribution Channels & Go-to-Market Analysis (mode 1_2)

## Executive Summary

Parker's distribution model is a **hybrid**: the Diversified Industrial segment sells direct to OEMs *and* through independent distributors — "marketed direct to OEMs and independent distributors through field sales employees" ([FACT] https://agentii.ai/v/PH/sec166/page66) — while Aerospace Systems sells **direct-only** through regional sales organizations to OEMs and end users ([FACT] https://agentii.ai/v/PH/sec166/page4). Reach is extreme: "several hundred thousand OEMs and distribution customer locations" ([FACT] https://agentii.ai/v/PH/sec166/page3) served from 323 manufacturing plants across 35 US states and 43 other countries ([FACT] https://agentii.ai/v/PH/sec166/page19). Parker discloses **no quantitative direct:indirect split**, so channel mix can only be characterized qualitatively (coverage gap). The Aerospace direct model earns 26.0% segment operating margin versus DI's hybrid 23.8% ([FACT] https://agentii.ai/v/PH/sec166/page25, https://agentii.ai/v/PH/sec166/page26) — a 220bps spread [DEDUCTED] consistent with OEM-direct pricing power plus proprietary aftermarket control. Channel commentary on the Q4 FY2026 call ("signs from distribution that the industrial recovery is broadening") shows distribution remains a live demand-monitoring asset ([FACT] https://agentii.ai/v/PH/ect72/page2).

## 1. Distribution Model

**Distribution Model: Hybrid (segment-specific).**

**Diversified Industrial — direct + independent distributors.** "We market our Diversified Industrial Segment products primarily through field sales employees and independent distributors located throughout the world" ([FACT] https://agentii.ai/v/PH/sec166/page4). The segment note is explicit: DI "products are marketed direct to OEMs and independent distributors through field sales employees" ([FACT] https://agentii.ai/v/PH/sec166/page66). Distributors serve "the aftermarket replacement markets" ([FACT] https://agentii.ai/v/PH/sec166/page3).

**Aerospace Systems — direct sales.** "We market our Aerospace Systems Segment products through our regional sales organizations, which sell directly to OEMs and end users throughout the world" ([FACT] https://agentii.ai/v/PH/sec166/page4); segment-note language: "marketed by field sales employees and are sold directly to manufacturers and end users" ([FACT] https://agentii.ai/v/PH/sec166/page66).

**Physical infrastructure.** At June 30, 2026: approximately 323 manufacturing plants, plus sales/administrative offices and distribution centers worldwide, situated in 35 US states and 43 other countries ([FACT] https://agentii.ai/v/PH/sec166/page19). The DI North America businesses "have manufacturing plants and distribution networks throughout the United States, Canada and Mexico"; DI International serves 41 countries across EMEA, Asia Pacific, and Latin America ([FACT] https://agentii.ai/v/PH/sec166/page66).

## 2. Distribution Partners

Disclosed channel types and partners:

- **Independent distributors** — unnamed, but the distributor channel is structurally central to DI: distributor agreements govern blanket purchase orders ("subject to a master supply or distributor agreement") ([FACT] https://agentii.ai/v/PH/sec166/page44).
- **Field sales employees** — Parker's own direct sales force sells to OEMs in both segments ([FACT] https://agentii.ai/v/PH/sec166/page4).
- **"Channel partners"** — CEO Parmentier's language: acquisitions "giv[e] our application engineers and channel partners more ways to create value for customers" ([FACT] https://agentii.ai/v/PH/ect72/page1).
- **Distribution networks as moat input** — "Global distribution network" is listed among Parker's six competitive-differentiation factors ([FACT] https://agentii.ai/v/PH/sec166/page5).

Named channel partners are not disclosed in the 10-K (coverage gap — Parker does not publish a distributor roster or channel-partner revenue share).

## 3. Current Channel Mix

**Direct : Indirect = not disclosed (qualitative hybrid).**

Parker provides no percentage split of direct vs. distributor sales in any filing retrieved (FY2024–FY2026 10-Ks, Q4 FY2026 transcript). What can be bounded qualitatively:

- Aerospace Systems is 100% direct by disclosure (32.8% of consolidated revenue = $7,061M of $21,499M) ([DEDUCTED] from https://agentii.ai/v/PH/sec166/page44).
- DI (67.2%, $14,438M) is split between OEM-direct and distributors, proportions undisclosed ([FACT] https://agentii.ai/v/PH/sec166/page44).
- DI geographic mix is the closest structural proxy: North America $8,392M / International $6,046M ([FACT] https://agentii.ai/v/PH/sec166/page25).

## 4. Historical Channel Mix Trend (Trailing 3 Years)

| Period | Direct : Indirect | Basis |
|---|---|---|
| FY2024 | not disclosed | 10-K language identical in structure (3 platforms, same channel description lineage) |
| FY2025 | not disclosed | FY2025 10-K discloses identical channel language for both segments |
| FY2026 | not disclosed | "marketed direct to OEMs and independent distributors" / Aerospace "directly to manufacturers and end users" |

Parker's disclosed channel *architecture* is stable across the trailing 3 years (no channel-strategy change disclosed in FY2024–FY2026 filings retrieved). What did change is *channel-level demand*: Q4 FY2026 orders improved +16% in North America and +24% internationally on a 3-month basis ([FACT] https://agentii.ai/v/PH/ect72/page2), and management "see[s] signs from distribution that the industrial recovery is broadening as customers' demand gradually accelerates" ([FACT] https://agentii.ai/v/PH/ect72/page2).

## 5. Strategic Implications

1. **Hybrid = reach + pricing control.** The distributor network gives Parker access to hundreds of thousands of customer locations without carrying that customer-relationship cost internally; the direct OEM channel preserves engineering intimacy and pricing power on the highest-value accounts. [VIEW]
2. **Aerospace's direct model correlates with superior margin.** Aerospace segment operating margin (26.0%) exceeds DI's (23.8%) by 220bps [DEDUCTED] — and DI's own margin rose 100bps in FY2026 to 23.8% despite distributor-channel exposure ([FACT] https://agentii.ai/v/PH/sec166/page25). [VIEW] Direct OEM + proprietary aftermarket appears to be the higher-margin route, consistent with the profit-pool thesis: distribution distance from the customer compresses margin.
3. **Field-sales cost is material.** SG&A is 16.1% of sales ([FACT] https://agentii.ai/v/PH/sec166/page23) — a large, hybrid-channel sales organization is baked into the cost structure; unlike a software vendor, channel cost does not decline with scale. [VIEW]
4. **No disclosed channel shift.** Unlike many industrials pivoting to e-commerce/direct, Parker discloses no quantitative channel-mix evolution; the FY2027 change is to order-reporting methodology (rolling 12-month), not channel strategy ([FACT] https://agentii.ai/v/PH/ect72/page1).

## 6. Coverage Gaps & Citations

**Coverage gaps:** (1) no quantitative direct:indirect split (the mode's "1 : XX" template cannot be populated from filings — flagged, not invented); (2) no named distributor partners; (3) no channel-level margin disclosure (Parker reports segment margins, not channel margins); (4) no distributor-count disclosure in FY2026 10-K (a "13,000 distributors" figure does **not** appear — keyword search returned zero hits).

**Citations roll-up:**

1. https://agentii.ai/v/PH/sec166/page3 — several hundred thousand OEM/distribution locations; distributors serve aftermarket
2. https://agentii.ai/v/PH/sec166/page4 — distribution methods per segment
3. https://agentii.ai/v/PH/sec166/page5 — global distribution network as competitive factor
4. https://agentii.ai/v/PH/sec166/page19 — 323 plants, 35 states, 43 countries
5. https://agentii.ai/v/PH/sec166/page23 — SG&A 16.1% of sales
6. https://agentii.ai/v/PH/sec166/page25 — DI NA/Int'l sales split
7. https://agentii.ai/v/PH/sec166/page26 — Aerospace segment margin 26.0%
8. https://agentii.ai/v/PH/sec166/page44 — Aerospace 32.8% / DI 67.2% of consolidated
9. https://agentii.ai/v/PH/sec166/page66 — segment-note channel language
10. https://agentii.ai/v/PH/ect72/page1 — channel partners language
11. https://agentii.ai/v/PH/ect72/page2 — Q4 order rates, distribution demand signs

## 7. Verification Table

| # | Number | Source retrieval | Tool call |
|---|---|---|---|
| 1 | DI channel language ("direct to OEMs and independent distributors") | sec166 page66 | read_source_pages |
| 2 | Aerospace direct-only language | sec166 page4, page66 | read_source_pages |
| 3 | 323 plants / 35 states / 43 countries | sec166 page19 | read_source_pages |
| 4 | "several hundred thousand OEMs and distribution customer locations" | sec166 page3 | read_source_pages |
| 5 | NA orders +16%, Int'l +24% (Q4 FY2026, 3-month) | ect72 page2 | read_source_pages |
| 6 | SG&A 16.1% of sales | sec166 page23 | read_source_pages |
| 7 | No "13,000" distributor count exists | keyword search sec166 | search_keyword_in_source |
| 8 | DI NA $8,392M / Int'l $6,046M | sec166 page25 | read_source_pages |
