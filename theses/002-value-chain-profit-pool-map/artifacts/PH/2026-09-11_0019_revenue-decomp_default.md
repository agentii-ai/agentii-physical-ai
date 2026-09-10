---
artifact_id: "002-PH-revenue-decomp-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: PH
skill: revenue-decomp
mode: default
affix: revenue-mix
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "037b396ab004"
as_of: 2026-09-11
entity_claims:
  - entity: PH
    metric: motion_systems_revenue_usd
    value: 3580000000
    unit: USD
    period: FY2026
    source: "10-K:page44"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: diversified_industrial_segment_operating_margin_pct
    value: 23.8
    unit: pct
    period: FY2026
    source: "10-K:page25"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: consolidated_gross_margin_pct
    value: 37.7
    unit: pct
    period: FY2026
    source: "10-K:page23"
    retrieved_at: 2026-09-11
citations:
  - https://agentii.ai/v/PH/sec166/page3
  - https://agentii.ai/v/PH/sec166/page23
  - https://agentii.ai/v/PH/sec166/page25
  - https://agentii.ai/v/PH/sec166/page26
  - https://agentii.ai/v/PH/sec166/page43
  - https://agentii.ai/v/PH/sec166/page44
  - https://agentii.ai/v/PH/sec166/page67
pillars_addressed: [PIL-3]
claim_state: pinned
key_metrics:
  consolidated_net_sales_usd_fy2026: 21499000000
  motion_systems_revenue_usd_fy2026: 3580000000
  diversified_industrial_revenue_usd_fy2026: 14438000000
  aerospace_systems_revenue_usd_fy2026: 7061000000
  consolidated_gross_margin_pct_fy2026: 37.7
  di_segment_operating_margin_pct_fy2026: 23.8
  aerospace_segment_operating_margin_pct_fy2026: 26.0
  software_subscription_revenue_usd_fy2026: 0
conclusions:
  - "PIL-3 null case CONFIRMED: PH discloses zero software, subscription, or royalty revenue; its entire revenue disaggregation is hardware platforms and aerospace market segments, and 'subscription' returns 0 hits across the FY2026 10-K."
  - "PH's motion-layer revenue pool (Motion Systems) is $3.58B of $21.50B total sales in FY2026; no model-layer software rent exists in the mix."
  - "PH cannot falsify the PIL-3 threshold (model_layer_revenue_per_deployed_unit_usd > 5000): its software/subscription revenue per unit is $0."
facts_count: 27
deducted_count: 11
views_count: 2
citation_count: 7
---

# PH — Revenue Decomposition (PIL-3 null case: model-layer rent)

**Mode**: default | **Skill**: revenue-decomp | **Primary source**: FY2026 Form 10-K, citation_id `sec166`, filed 2026-08-21, report date 2026-06-30 (accession 0000076334-26-000105)

## Executive Summary

Parker-Hannifin FY2026 (ended 2026-06-30) net sales were $21,499M [FACT], split 67% Diversified Industrial ($14,438M) and 33% Aerospace Systems ($7,061M) [FACT]. Diversified Industrial disaggregates into three hardware technology platforms: Motion Systems $3,580M, Flow & Process Control $4,810M, and Filtration & Engineered Materials $6,048M [FACT]. Aerospace splits into commercial/defense OEM and aftermarket lines [FACT]. **No software, subscription, or digital-service revenue line exists anywhere in the disaggregation**: "subscription" returns zero hits in the entire FY2026 10-K, and the XBRL product/service axis contains only hardware members [FACT]. Revenue recognition is shipment-based product sales [FACT]. PIL-3 null case is therefore confirmed: PH's software/subscription royalty revenue is $0 — zero model-layer rent per deployed unit [DEDUCTED] — so PH cannot exceed the $5,000/unit falsifier threshold [VIEW]. Margin anchors for the motion layer: consolidated gross margin 37.7%, DI segment operating margin 23.8%, Aerospace Systems 26.0% [FACT].

## 1. Revenue Architecture (FY2026)

### 1.1 Segment level

| Segment | FY2026 net sales ($M) | Share | Segment op. margin | Source |
|---|---|---|---|---|
| Diversified Industrial | 14,438 [FACT] | 67.2% [DEDUCTED] | 23.8% [FACT] | page25, page44 |
| Aerospace Systems | 7,061 [FACT] | 32.8% [DEDUCTED] | 26.0% [FACT] | page26, page44 |
| **Total** | **21,499 [FACT]** | 100% | — | page23, page44 |

The company states the mix directly: "Of the Company's $21.5 billion in net sales for fiscal year 2026, Diversified Industrial Segment products accounted for 67% and Aerospace Systems Segment products accounted for 33%" [FACT] — https://agentii.ai/v/PH/sec166/page3.

Diversified Industrial sub-splits by geography in MD&A: North America net sales $8,392M at 24.3% operating margin; International $6,046M at 23.1% [FACT] — https://agentii.ai/v/PH/sec166/page25. Segment totals reconcile through the Note 18 bridge: DI $14,438M + Aerospace $7,061M = $21,499M, and total segment operating income $5,273M [FACT] — https://agentii.ai/v/PH/sec166/page67.

### 1.2 DI technology-platform decomposition (actuation-layer pool)

The revenue disaggregation note decomposes DI into exactly three technology platforms [FACT]:

| Platform | FY2026 ($M) | FY2025 ($M) | FY2024 ($M) | YoY | Source |
|---|---|---|---|---|---|
| **Motion Systems** | **3,580** | 3,341 | 3,706 | +7.2% [DEDUCTED] | page44 |
| Flow and Process Control | 4,810 | 4,518 | 4,673 | +6.5% [DEDUCTED] | page44 |
| Filtration and Engineered Materials | 6,048 | 5,806 | 6,079 | +4.2% [DEDUCTED] | page44 |
| Total DI | 14,438 | 13,665 | 14,458 | +5.7% [FACT] | page44 |

https://agentii.ai/v/PH/sec166/page44

**Motion Systems** — the actuation-layer pool anchor for this thesis — is $3,580M in FY2026 [FACT] — https://agentii.ai/v/PH/sec166/page44, i.e. 24.8% of DI revenue [DEDUCTED] and 16.7% of consolidated revenue [DEDUCTED]. This matches the entities.md anchor `motion_systems_revenue_usd` (3,580,000,000, FY2026) exactly.

### 1.3 Aerospace decomposition

| Market segment | FY2026 ($M) | FY2025 ($M) | FY2024 ($M) | Source |
|---|---|---|---|---|
| Commercial OEM | 2,330 | 1,915 | 1,779 | page44 |
| Commercial aftermarket | 2,523 | 2,214 | 1,814 | page44 |
| Defense OEM | 1,271 | 1,138 | 1,125 | page44 |
| Defense aftermarket | 937 | 918 | 754 | page44 |
| Total Aerospace | 7,061 | 6,185 | 5,472 | page44 |

https://agentii.ai/v/PH/sec166/page44. The combined aftermarket lines ($2,523M + $937M = $3,460M [DEDUCTED]) are hardware spares/repair parts, not software or subscriptions — the 10-K describes Aerospace products as "engine and airframe components and systems" sold via blanket purchase orders and long-term production contracts [FACT] — https://agentii.ai/v/PH/sec166/page44.

### 1.4 Geographic split

North America $14,386M, EMEA $4,178M, Asia Pacific $2,711M, Latin America $224M [FACT] — https://agentii.ai/v/PH/sec166/page44. No country other than the US exceeds 10% of consolidated sales [FACT] — https://agentii.ai/v/PH/sec166/page67.

## 2. Product vs Service — the PIL-3 null evidence

PIL-3 treats PH as the null case: a hardware vendor whose mix should show zero software/subscription royalty. Four independent evidence layers confirm the null:

**E1 — Revenue recognition language (product-sale model).** Note 2 states: "Revenue is derived primarily from the sale of products… A majority of the Company's revenues are recognized at a point in time" [FACT] — https://agentii.ai/v/PH/sec166/page43. For DI: "Revenue in the Diversified Industrial Segment is typically recognized at the time of product shipment, but a portion of revenue may be recognized over time for installation services or in situations where the product has no alternative use" [FACT] — https://agentii.ai/v/PH/sec166/page44. The only service element disclosed is installation services bundled with product, with no separately reported service/software revenue line.

**E2 — Disaggregation completeness.** The full revenue disaggregation (Note 2, page44) contains only: 3 DI hardware platforms, 4 aerospace market segments, and 5 geographic regions [FACT] — https://agentii.ai/v/PH/sec166/page44. No software, subscription, SaaS, digital, or royalty category exists in any dimension.

**E3 — Keyword probes.** `search_keyword_in_source(sec166, "subscription")` returns **0 hits** across the entire 79-page FY2026 10-K [FACT] (MCP call, 2026-09-11). `"software"` returns 4 hits, none revenue-related: an ASU 2025-06 internal-use software accounting standard (page43), cybersecurity governance (page18), IT-systems risk factor (page11), and an executive biography (page9) [FACT] — https://agentii.ai/v/PH/sec166/page43.

**E4 — XBRL product axis.** The `srt:ProductOrServiceAxis` for PH FY2026 contains only six members — Motion Systems, Flow and Process Control, Filtration and Engineered Materials, Commercial/Defense OEM, Commercial/Defense Aftermarket — no software or subscription member exists in the taxonomy instance [FACT] (`search_xbrl_facts`, concept `RevenueFromContractWithCustomerExcludingAssessedTax`, view=detailed, 2026-09-11).

**Null conclusion**: software/subscription/royalty revenue = $0 for FY2026 [DEDUCTED], hence software rent per deployed unit = $0 [DEDUCTED]. PH's aftermarket revenue is hardware spares, not software rent [VIEW].

## 3. Key Metrics

| Metric | FY2026 | FY2025 | Source |
|---|---|---|---|
| Consolidated net sales | $21,499M | $19,850M | https://agentii.ai/v/PH/sec166/page23 |
| Gross profit margin | 37.7% | 36.9% | https://agentii.ai/v/PH/sec166/page23 |
| Diversified Industrial revenue | $14,438M | $13,665M | https://agentii.ai/v/PH/sec166/page25 |
| DI segment operating margin | 23.8% | 22.8% | https://agentii.ai/v/PH/sec166/page25 |
| Aerospace Systems revenue | $7,061M | $6,185M | https://agentii.ai/v/PH/sec166/page26 |
| Aerospace operating margin | 26.0% | 23.3% | https://agentii.ai/v/PH/sec166/page26 |
| **Motion Systems revenue** | **$3,580M** | $3,341M | https://agentii.ai/v/PH/sec166/page44 |
| Software/subscription/royalty revenue | $0 (no line) | $0 (no line) | page44 + keyword probes |

## 4. XBRL Reconciliation (10-K wins rule)

Single revenue concept `us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax` (FY2026 consolidated = $21,499.0M, source_authority 3 = 10-K). All `view=detailed` facts reconcile **exactly** with 10-K page44, zero conflicts:

| XBRL dimension member | XBRL value ($M) | 10-K page44 ($M) | Status |
|---|---|---|---|
| Motion Systems (DI) | 3,580.0 | 3,580 | PASS |
| Flow and Process Control (DI) | 4,810.0 | 4,810 | PASS |
| Filtration and Engineered Materials (DI) | 6,048.0 | 6,048 | PASS |
| Commercial OEM / aftermarket | 2,330.0 / 2,523.0 | 2,330 / 2,523 | PASS |
| Defense OEM / aftermarket | 1,271.0 / 937.0 | 1,271 / 937 | PASS |
| DI total / Aerospace total | 14,438.0 / 7,061.0 | 14,438 / 7,061 | PASS |
| North America / EMEA / APAC / LatAm | 14,386 / 4,178 / 2,711 / 224 | 14,386 / 4,178 / 2,711 / 224 | PASS |

**No conflicts flagged; the 10-K-wins override was not invoked.**

## 5. Coverage Gaps & Citations

**Gaps**

1. No FY2027 Q1 10-Q yet (PH fiscal Q1 ends 2026-09-30; filing expected ~Nov 2026). FY2026 10-K is the latest authoritative revenue source — sufficient for the FY2026-period PIL-3 claim.
2. PH does not quantitatively disclose a product-vs-service split; only narrative ("a portion… over time for installation services") — the absence of a service/software line is itself the PIL-3 evidence.
3. **Entities-map append request (for implement dispatcher)**: new metric `software_subscription_revenue_usd` (value 0, unit USD, period FY2026, source "10-K:page44+keyword-probe") should be appended to the §2 map so the null becomes a structured claim, per the "never invented inline" rule.
4. `agentii.md` session append was skipped per task constraint ("DO NOT edit shared files; only artifacts/PH/").
5. No price data used, per audit mandate.

**Citation index** (all `sec166`, FY2026 10-K, filed 2026-08-21):

1. https://agentii.ai/v/PH/sec166/page3 — Business: segment mix 67/33, $21.5B sales
2. https://agentii.ai/v/PH/sec166/page23 — Consolidated results: $21,499M, GM 37.7%
3. https://agentii.ai/v/PH/sec166/page25 — DI segment results, margins, backlog
4. https://agentii.ai/v/PH/sec166/page26 — Aerospace segment results, margins, backlog
5. https://agentii.ai/v/PH/sec166/page43 — Note 2 revenue recognition: product sales, point-in-time
6. https://agentii.ai/v/PH/sec166/page44 — Revenue disaggregation: platforms, markets, geography
7. https://agentii.ai/v/PH/sec166/page67 — Note 18 segment reconciliation and geographic net sales

## 6. Verification Table

| # | Claim | Retrieved value | Source | Verifier | Status |
|---|---|---|---|---|---|
| 1 | Consolidated net sales FY2026 | $21,499M | page23 + page44 | XBRL consolidated 21,499,000,000 (10-K instance) | PASS |
| 2 | Motion Systems revenue FY2026 | $3,580M | page44 | XBRL MotionSystemsMember 3,580,000,000 | PASS |
| 3 | DI / Aerospace revenue FY2026 | 14,438 / 7,061 | page25/26 + page44 | XBRL segment members 14,438 / 7,061 | PASS |
| 4 | DI op margin 23.8% / Aero 26.0% | page25 / page26 | page67 op income bridge (3,440/14,438; 1,833/7,061) | PASS |
| 5 | GM 37.7% | page23 | XBRL COGS 13,397 → 1 − 13,397/21,499 = 37.7% | PASS |
| 6 | No software/subscription revenue line | 0 hits "subscription"; hardware-only axes | keyword probe + XBRL ProductOrServiceAxis + page44 | PASS |
| 7 | Revenue = product sales | Note 2, page43/page44 | E1 quotes | PASS |

**Verification outcome**: all 7 checks PASS; zero XBRL-vs-10-K conflicts; null case established on 4 independent evidence layers (E1–E4).

*Preflight: search_companies (PH = Parker-Hannifin, NYSE, industrial machinery), get_ticker_coverage (59 SEC filings; XBRL 20,714 facts through 2026-08-21), get_company_fiscal_calendar (FYE June 30). Retrieval: Layer 1 search_sec_filings → sec166; Layer 2 read_source_outline (79 pages); Layer 3 read_source_pages (pages 3, 23, 25, 26, 43, 44, 66, 67). Structured: get_company_financials, list_xbrl_concepts, search_xbrl_facts (detailed). Tool diversity: 11.*
