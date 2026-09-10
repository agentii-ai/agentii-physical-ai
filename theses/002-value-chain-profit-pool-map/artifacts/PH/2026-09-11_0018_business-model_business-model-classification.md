---
artifact_id: "002-PH-business-model-business-model-classification-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: PH
skill: business-model
mode: business-model-classification
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
  - "sec166:page6"
  - "sec166:page23"
  - "sec166:page25"
  - "sec166:page26"
  - "sec166:page35"
  - "sec166:page44"
  - "sec166:page66"
  - "sec127:page42"
  - "ect72:page1"
  - "ect72:page2"
pillars_addressed: [PIL-3]
claim_state: pinned
key_metrics:
  consolidated_net_sales_usd: 21499000000
  consolidated_gross_margin_pct: 37.7
  diversified_industrial_segment_operating_margin_pct: 23.8
  aerospace_segment_operating_margin_pct: 26.0
  adjusted_segment_operating_margin_pct: 27.3
  aerospace_aftermarket_share_of_aerospace_pct: 49.0
  subscription_revenue_mentions_in_10k: 0
conclusions:
  - "PH is a pure product (hardware) business model — no platform, no software/subscription revenue stream; revenue recognized at shipment."
  - "PIL-3 null case holds: model-layer revenue per deployed unit is zero — 'subscription' appears 0 times in the FY2026 10-K."
  - "Razor-blade economics exist in hardware-only form: Aerospace aftermarket is 49.0% of Aerospace revenue; FGC acquisition adds 500bps of filtration aftermarket."
  - "Positioning is premium-differentiated: 37.7% consolidated GM, 23.8% DI and 26.0% Aerospace segment margins, record 27.3% adjusted segment margin."
  - "All three T-001 PH baseline figures re-retrieved and confirmed with zero contradictions."
facts_count: 25
deducted_count: 5
views_count: 3
citation_count: 13
---

# PH — Business Model & Offerings Classification (mode 1_1)

## Executive Summary

Parker-Hannifin (PH) is a **product business** — it designs, manufactures, and provides aftermarket support for highly engineered motion-and-control hardware ([FACT] https://agentii.ai/v/PH/sec166/page3). FY2026 net sales were $21,499M across two segments, Diversified Industrial (DI) 67% and Aerospace Systems 33% ([FACT] https://agentii.ai/v/PH/sec166/page3). There is **no platform layer, no software revenue, and no subscription revenue**: the word "subscription" appears zero times in the FY2026 10-K ([FACT] keyword search, https://agentii.ai/v/PH/sec166/page4), and the majority of revenue is recognized point-in-time at product shipment ([FACT] https://agentii.ai/v/PH/sec127/page42). This is the PIL-3 **null case**: a hardware vendor with no model-layer rent. Razor-blade economics operate in hardware-only form — Aerospace aftermarket is 49.0% of Aerospace revenue ([DEDUCTED] from https://agentii.ai/v/PH/sec166/page44), and the FGC acquisition adds 500bps of filtration aftermarket ([FACT] https://agentii.ai/v/PH/ect72/page1). Positioning is premium-differentiated: consolidated gross margin 37.7%, DI segment operating margin 23.8%, Aerospace 26.0%, record 27.3% adjusted segment operating margin ([FACT] https://agentii.ai/v/PH/sec166/page23, https://agentii.ai/v/PH/sec166/page25, https://agentii.ai/v/PH/sec166/page26, https://agentii.ai/v/PH/ect72/page1). All three T-001 PH baselines re-retrieved with zero contradictions.

## 1. Business Model Classification

**Business Model: Product (pure hardware manufacturer).**

Parker is "a global leader in motion and control technologies" that designs, manufactures, and provides aftermarket support for highly engineered solutions ([FACT] https://agentii.ai/v/PH/sec166/page3). The two reportable segments both sell physical products:

- **Diversified Industrial** — "an aggregation of several business units that design, manufacture, and provide aftermarket support for highly engineered solutions" across six market verticals (aerospace & defense, in-plant & industrial equipment, transportation, off-highway, energy, HVAC & refrigeration) ([FACT] https://agentii.ai/v/PH/sec166/page66).
- **Aerospace Systems** — "designs, manufactures and provides aftermarket support for highly engineered airframe and engine solutions for both OEMs and end users" ([FACT] https://agentii.ai/v/PH/sec166/page66).

Both segments draw on eight core technologies: hydraulics, pneumatics, electromechanical, filtration, fluid & gas handling, process control, engineered materials, and climate control ([FACT] https://agentii.ai/v/PH/sec166/page66).

**Revenue mechanics confirm a pure product model.** Revenue is "derived primarily from the sale of products" ([FACT] https://agentii.ai/v/PH/sec127/page42). In the DI segment, "revenue is typically recognized at the time of product shipment"; in Aerospace, likewise at shipment with a portion over time for customer-controlled assets ([FACT] https://agentii.ai/v/PH/sec166/page44). No performance-obligation stream resembling a SaaS subscription, license, or service annuity is disclosed. The word "subscription" has **zero occurrences** in the entire FY2026 10-K, and "software" appears only in IT/cybersecurity contexts, never as a revenue stream ([FACT] keyword-search result, https://agentii.ai/v/PH/sec166/page4).

**Classification ruling:** Product business. Not a platform (no network effects, no third-party ecosystem), not a service business (aftermarket is parts, not services-led). [VIEW] The closest structural analogue is the classic industrial "razor/razor-blade" model executed entirely in hardware: OEM sell-in followed by a captive replacement-parts annuity.

## 2. Core Offering

Motion and control technologies for machines — "hundreds of thousands of individual part numbers" ([FACT] https://agentii.ai/v/PH/sec166/page4). Principal DI product families include electric & hydraulic pumps, motors, valves, actuators, drives & controllers, filtration, seals, hoses, fittings, and thermal management ([FACT] https://agentii.ai/v/PH/sec166/page4). Aerospace products include actuation, flight-control systems, fuel systems, engine components, braking systems, and avionics ([FACT] https://agentii.ai/v/PH/sec166/page4).

Notably for this thesis, "Electronics, Drives & Controllers" and "Sensors & Diagnostics" are listed as DI products ([FACT] https://agentii.ai/v/PH/sec166/page4) — embedded control electronics ship as part of the hardware, but no standalone software/subscription revenue is disclosed. [DEDUCTED] The model-layer (software) revenue pool at PH is therefore zero on any disclosed basis, making PH a clean null-case comparator for PIL-3's `model_layer_revenue_per_deployed_unit_usd` falsifier.

## 3. Positioning

**Positioning: Premium-differentiated (high-end within industrial manufacturing).**

- Consolidated gross margin 37.7% in FY2026, up from 36.9% ([FACT] https://agentii.ai/v/PH/sec166/page23).
- DI segment operating margin 23.8%; Aerospace 26.0% ([FACT] https://agentii.ai/v/PH/sec166/page25, https://agentii.ai/v/PH/sec166/page26).
- Record adjusted segment operating margin of 27.3%, +120bps, with a new FY2031 target of 30% announced on the Q4 FY2026 call ([FACT] https://agentii.ai/v/PH/ect72/page1).

Rationale for premium classification: margins are supported by "highly engineered differentiated products" sold to "several hundred thousand OEMs and distribution customer locations" ([FACT] https://agentii.ai/v/PH/sec166/page3), an aftermarket-heavy mix (Aerospace aftermarket = 49.0% of segment sales; [DEDUCTED] from https://agentii.ai/v/PH/sec166/page44), and a proprietary operating system ("The Win Strategy") that management credits for top-quartile performance ([FACT] https://agentii.ai/v/PH/sec166/page3). [VIEW] Parker occupies a premium-tier position within industrial components — above commodity parts distributors, below software-annuity players (ISRG, NVDA); its margin ceiling is manufacturing-plus-aftermarket, with no model-layer rent to stack on top.

## 4. Razor / Razor-Blade Structure (hardware-only)

PH's annuity mechanics are disclosed explicitly:

- DI products are sold "to both OEMs and distributors who serve the aftermarket replacement markets" ([FACT] https://agentii.ai/v/PH/sec166/page3) — standard/custom original products are "also used in the replacement of original products" ([FACT] https://agentii.ai/v/PH/sec166/page4).
- Aerospace aftermarket revenue (commercial $2,523M + defense $937M = $3,460M) is 49.0% of Aerospace segment revenue ([DEDUCTED] from https://agentii.ai/v/PH/sec166/page44).
- Management states the FGC acquisition "expands our offering of proprietary filtration technologies and **increases our filtration aftermarket by 500 basis points**" ([FACT] https://agentii.ai/v/PH/ect72/page1) — i.e., acquisitions are explicitly evaluated for their aftermarket-annuity contribution.

[VIEW] The absence of any subscription layer means the "blade" revenue is a parts annuity with competitive decay risk (third-party parts, OEE-driven demand), not a locked-in software annuity — the structural reason the model layer, not the motion layer, captures the profit pool in this thesis's frame.

## 5. Coverage Gaps & Citations

**Coverage gaps:**

1. No quantitative channel split (direct vs distributor %) is disclosed anywhere in filings — see distribution-channel-analysis artifact.
2. No customer-level revenue concentration percentage is disclosed in the FY2026 10-K (the T-001 "no product >1%" claim is product-level; customer-level data is absent).
3. No unit-volume disclosure: `revenue_per_deployed_unit` cannot be computed directly for PH (consistent with PIL-3 null case — the metric is zero by construction of no software revenue).
4. Market sizing (TAM/SAM/SOM) not retrieved — mode 1_4 not in scope of this chain.

**Citations roll-up (non-duplicative index of inline links):**

1. https://agentii.ai/v/PH/sec166/page3 — business overview, 67/33 segment split, OEM/distributor customers
2. https://agentii.ai/v/PH/sec166/page4 — principal products, distribution methods, no-single-product->1%
3. https://agentii.ai/v/PH/sec166/page5 — competitors, backlog $12.8B
4. https://agentii.ai/v/PH/sec166/page6 — employees 59,850, acquisitions
5. https://agentii.ai/v/PH/sec166/page23 — consolidated results, GM 37.7%
6. https://agentii.ai/v/PH/sec166/page25 — DI segment margin 23.8%
7. https://agentii.ai/v/PH/sec166/page26 — Aerospace margin 26.0%
8. https://agentii.ai/v/PH/sec166/page35 — income statement
9. https://agentii.ai/v/PH/sec166/page44 — revenue disaggregation (platforms, markets, geography)
10. https://agentii.ai/v/PH/sec166/page66 — segment note, 8 core technologies, channel language
11. https://agentii.ai/v/PH/sec127/page42 — point-in-time majority, FY2023 comparatives
12. https://agentii.ai/v/PH/ect72/page1 — record FY2026, 27.3% margin, FGC +500bps aftermarket, FY31 target
13. https://agentii.ai/v/PH/ect72/page2 — Q4 results, distribution demand signs

## 6. Verification Table

| # | Number | Source retrieval | Tool call |
|---|---|---|---|
| 1 | Net sales FY2026 $21,499M | sec166 page35; XBRL fact 2025-07-01→2026-06-30, authority 3 | read_source_pages; search_xbrl_facts (RevenueFromContractWithCustomerExcludingAssessedTax) |
| 2 | Gross margin 37.7% | sec166 page23; cross-check (21,499−13,397)/21,499=37.68% from page35 | read_source_pages |
| 3 | DI segment op margin 23.8% ($3,440M/$14,438M) | sec166 page25 | read_source_pages |
| 4 | Aerospace segment op margin 26.0% ($1,833M/$7,061M) | sec166 page26 | read_source_pages |
| 5 | Adjusted segment op margin 27.3% | ect72 page1 (non-GAAP, management-disclosed) | read_source_pages |
| 6 | Aerospace aftermarket share 49.0% | computed from sec166 page44 table (2,523+937)/7,061 | read_source_pages + arithmetic [DEDUCTED] |
| 7 | "subscription" occurrences in FY2026 10-K = 0 | keyword search over sec166 | search_keyword_in_source |
| 8 | Motion Systems FY2026 $3,580M (T-001 reconcile) | sec166 page44; XBRL detailed fact (ph:MotionSystemsMember × ph:DiversifiedIndustrialSegmentMember) | search_xbrl_facts view=detailed |
| 9 | Backlog $12.8B June 30, 2026 | sec166 page5 | read_source_pages |
| 10 | Employees ~59,850 | sec166 page6 | read_source_pages |

**T-001 reconciliation:** all three PH baselines confirmed fresh with zero contradictions — Motion Systems $3,580M FY2026 (https://agentii.ai/v/PH/sec166/page44), DI op margin 23.8% (https://agentii.ai/v/PH/sec166/page25), consolidated GM 37.7% (https://agentii.ai/v/PH/sec166/page23). No contradictions to report.
