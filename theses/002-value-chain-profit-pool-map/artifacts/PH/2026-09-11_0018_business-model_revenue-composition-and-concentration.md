---
artifact_id: "002-PH-business-model-revenue-composition-and-concentration-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: PH
skill: business-model
mode: revenue-composition-and-concentration
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
  - "sec166:page19"
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
  aerospace_share_of_consolidated_pct: 32.8
  motion_systems_share_of_consolidated_pct: 16.6
  north_america_revenue_share_pct: 66.9
  aerospace_aftermarket_share_of_aerospace_pct: 49.0
  largest_single_product_share_pct: "<1"
  q4_fy2026_revenue_usd: 5755000000
conclusions:
  - "Top-3 product lines: Aerospace Systems 32.8%, Filtration & Engineered Materials 28.1%, Flow & Process Control 22.4%; Motion Systems 16.6% of consolidated."
  - "Concentration risk minimal: no single product >1% of net sales (verbatim 10-K, confirms T-001); no product or segment exceeds the 20% flag except the Aerospace segment itself at 32.8%."
  - "T-001 'no product >1%' verified verbatim; Motion Systems $3,580M FY2026 verified; zero contradictions vs T-001 baselines."
  - "Aerospace mix is rising (27.5% → 32.8% of revenue FY2024→FY2026); aerospace aftermarket is 49.0% of Aerospace revenue."
  - "Revenue is ~100% B2B; no software/connected-services revenue line exists — even IoT ('connected products') capabilities monetize as hardware."
facts_count: 21
deducted_count: 14
views_count: 1
citation_count: 14
---

# PH — Revenue Composition & Concentration Risk Analysis (mode 1_3)

## Executive Summary

PH's FY2026 revenue of $21,499M decomposes into four product lines: Aerospace Systems $7,061M (32.8%), Filtration & Engineered Materials $6,048M (28.1%), Flow & Process Control $4,810M (22.4%), and Motion Systems $3,580M (16.6%) ([FACT] https://agentii.ai/v/PH/sec166/page44; [DEDUCTED] shares). Concentration risk is structurally minimal: **"no single product contributed more than one percent to our total net sales for the year ended June 30, 2026"** — verbatim ([FACT] https://agentii.ai/v/PH/sec166/page4), confirming T-001's finding. Revenue is ~100% B2B (OEMs, distributors, end users; no consumer channel disclosed) ([DEDUCTED] from https://agentii.ai/v/PH/sec166/page3). Geography: North America 66.9%, EMEA 19.4%, Asia Pacific 12.6%, Latin America 1.0% ([FACT] https://agentii.ai/v/PH/sec166/page44). Temporal mix is shifting toward Aerospace (27.5% → 32.8% of sales FY2024→FY2026) ([DEDUCTED] from https://agentii.ai/v/PH/sec166/page44); Aerospace aftermarket is 49.0% of that segment ([DEDUCTED]). Q4 FY2026 revenue was $5,755M vs $5,486M in Q3 ([DEDUCTED] from XBRL). No software or connected-services revenue line exists in the composition — the null-case revenue profile for PIL-3.

## 1. Latest Annual + Trailing-Quarter Revenue Breakdown (XBRL segment data)

### 1.1 By Product Line (FY2026)

| Product line / platform | FY2026 $M | % of consolidated | FY2025 $M | FY2024 $M |
|---|---|---|---|---|
| Aerospace Systems (segment) | 7,061 | 32.8% | 6,185 | 5,472 |
| Filtration & Engineered Materials (DI) | 6,048 | 28.1% | 5,806 | 6,079 |
| Flow & Process Control (DI) | 4,810 | 22.4% | 4,518 | 4,673 |
| Motion Systems (DI) | 3,580 | 16.6% | 3,341 | 3,706 |
| **Total** | **21,499** | **100%** | **19,850** | **19,930** |

All values [FACT] https://agentii.ai/v/PH/sec166/page44; shares [DEDUCTED]. XBRL cross-check: Motion Systems fact = $3,580M (ph:MotionSystemsMember × ph:DiversifiedIndustrialSegmentMember, authority 3) via search_xbrl_facts view=detailed.

**Motion Systems within DI:** $3,580M / $14,438M = 24.8% of DI revenue ([DEDUCTED]). DI total = $14,438M (67.2% of consolidated) ([FACT] https://agentii.ai/v/PH/sec166/page44).

### 1.2 By User Type (B2B vs B2C)

**~100% B2B.** DI sells "to both OEMs and distributors who serve the aftermarket replacement markets"; Aerospace sells to "OEMs and end users" ([FACT] https://agentii.ai/v/PH/sec166/page3, https://agentii.ai/v/PH/sec166/page66). No consumer-direct business is disclosed anywhere in the FY2026 10-K. [DEDUCTED] B2C share ≈ 0%.

### 1.3 By Geography (FY2026, selling-operation location)

| Region | $M | % |
|---|---|---|
| North America | 14,386 | 66.9% |
| EMEA | 4,178 | 19.4% |
| Asia Pacific | 2,711 | 12.6% |
| Latin America | 224 | 1.0% |

[FACT] https://agentii.ai/v/PH/sec166/page44; shares [DEDUCTED]. Cross-check vs XBRL geographic facts (srt:NorthAmericaMember $14,386M; EMEA $4,178M; AsiaPacific $2,711M; LatinAmerica $224M, all authority 3) — consistent. "The majority of revenues from the Aerospace Systems Segment is generated from sales within North America" ([FACT] https://agentii.ai/v/PH/sec166/page44).

### 1.4 By End Market

Parker does **not** disclose revenue percentages by end market (coverage gap). Disclosed qualitatively: six DI market verticals — aerospace & defense, in-plant & industrial equipment, transportation, off-highway, energy, HVAC & refrigeration ([FACT] https://agentii.ai/v/PH/sec166/page3); Aerospace & Defense is "our largest vertical" per CEO Parmentier ([FACT] https://agentii.ai/v/PH/ect72/page2). Within Aerospace, the disclosed market split is: Commercial OEM $2,330M, Commercial aftermarket $2,523M, Defense OEM $1,271M, Defense aftermarket $937M ([FACT] https://agentii.ai/v/PH/sec166/page44).

## 2. Concentration Risk Matrix

| Dimension | Largest unit | Share of revenue | >20% flag |
|---|---|---|---|
| Product (part number) | any single product | <1% — verbatim "no single product contributed more than one percent" | No |
| Platform / segment | Aerospace Systems | 32.8% | Yes (segment level; 3 sub-markets, largest = Commercial aftermarket 11.7%) |
| Customer | not disclosed | n/a | Not assessable — no customer-level % disclosed |
| Geography | North America | 66.9% | Yes |
| End market | not disclosed | n/a | Not assessable |

Product-level fact: https://agentii.ai/v/PH/sec166/page4. Largest Aerospace sub-market share: $2,523M / $21,499M = 11.7% [DEDUCTED] from https://agentii.ai/v/PH/sec166/page44. Competitor-level fragmentation: "no single competitor competes with the Company with respect to all the products we manufacture and sell" ([FACT] https://agentii.ai/v/PH/sec166/page5).

**Conclusion:** The T-001 finding "no product >1% of sales" is verified verbatim. The only >20% concentration is the Aerospace Systems segment itself (32.8%) and the North America geography (66.9%). No single customer exceeds disclosure thresholds, and Parker does not report a 10% customer (absence of any Form 10-K customer-concentration disclosure).

## 3. Temporal Comparison

**Quarter-over-quarter:** Q4 FY2026 revenue $5,755M vs Q3 FY2026 $5,486M (+4.9%) [DEDUCTED] from XBRL facts (FY2026 $21,499M minus 9M $15,744M; Q3 $5,486M — both authority 2/3 via search_xbrl_facts). Q4 organic growth was +8%, the strongest quarter of FY2026 ([FACT] https://agentii.ai/v/PH/ect72/page2).

**Year-over-year (FY2026 vs FY2025):** total sales +8.3% reported, +6.6% organic ([FACT] https://agentii.ai/v/PH/sec166/page23). Mix shift: Aerospace +14.2% vs DI +5.7% ([FACT] https://agentii.ai/v/PH/sec166/page25, https://agentii.ai/v/PH/sec166/page26).

**3-year mix evolution (FY2024 → FY2026):**

- Aerospace share of consolidated: 27.5% → 31.2% → 32.8% ([DEDUCTED] from https://agentii.ai/v/PH/sec166/page44)
- Aerospace aftermarket share of Aerospace revenue: 46.9% → 50.6% → 49.0% ([DEDUCTED] from https://agentii.ai/v/PH/sec166/page44)
- Motion Systems: $3,706M → $3,341M → $3,580M (down-then-recovering; FY2026 +7.2%) ([DEDUCTED] from https://agentii.ai/v/PH/sec166/page44)
- F&E/Filtration grew FY2025→FY2026 (+4.2%) and is being scaled further: the Filtration Group Corporation (FGC) acquisition closed Aug 13, 2026 ([FACT] https://agentii.ai/v/PH/sec166/page6); combined FGC + CIRCOR Aerospace announcements total "nearly $12 billion" of acquisitions, and with FGC closed, Parker "will have more than tripled the size of our filtration business" ([FACT] https://agentii.ai/v/PH/ect72/page1)

**Order/backlog momentum:** record backlog $12.8B (+16% YoY), ~70% shippable within 12 months ([FACT] https://agentii.ai/v/PH/sec166/page5, https://agentii.ai/v/PH/ect72/page2).

## 4. PIL-3 Relevance: the Composition Contains No Software Rent

The revenue composition has **zero disclosed software, subscription, or connected-services line items** ("subscription" = 0 occurrences in FY2026 10-K). Even where embedded intelligence exists — "Electronics, Drives & Controllers", "Sensors & Diagnostics" product families ([FACT] https://agentii.ai/v/PH/sec166/page4) and the CISO's oversight of "connected products (\"IoT\")" ([FACT] https://agentii.ai/v/PH/sec166/page19) — monetization is hardware-only, recognized at shipment ([FACT] https://agentii.ai/v/PH/sec127/page42). [VIEW] PH's composition is thus the pure motion-layer revenue profile: per-unit economics end at the sale of the part; there is no per-unit software rent to aggregate — the exact null case the PIL-3 falsifier needs.

## 5. Coverage Gaps & Citations

**Coverage gaps:** (1) end-market revenue % not disclosed (qualitative only); (2) customer-level concentration % not disclosed; (3) channel-level revenue split not disclosed (see distribution-channel-analysis artifact); (4) DI aftermarket vs OEM split not disclosed (Aerospace-only aftermarket available); (5) FY2027 Q1 (quarter ended Sept 30, 2026) not yet filed — trailing-quarter analysis uses Q4 FY2026.

**Citations roll-up:**

1. https://agentii.ai/v/PH/sec166/page3 — segments, verticals, OEM/distributor customers
2. https://agentii.ai/v/PH/sec166/page4 — no-single-product->1% verbatim; product families
3. https://agentii.ai/v/PH/sec166/page5 — competitor fragmentation; backlog $12.8B
4. https://agentii.ai/v/PH/sec166/page19 — IoT/connected products reference
5. https://agentii.ai/v/PH/sec166/page23 — consolidated results, +8.3%/+6.6%
6. https://agentii.ai/v/PH/sec166/page25 — DI segment results
7. https://agentii.ai/v/PH/sec166/page26 — Aerospace segment results
8. https://agentii.ai/v/PH/sec166/page35 — income statement
9. https://agentii.ai/v/PH/sec166/page44 — 3-year disaggregation tables
10. https://agentii.ai/v/PH/sec166/page66 — segment definitions, B2B channel language
11. https://agentii.ai/v/PH/sec166/page6 — FGC acquisition closed Aug 13, 2026
12. https://agentii.ai/v/PH/sec127/page42 — point-in-time majority; FY2023 comparatives
13. https://agentii.ai/v/PH/ect72/page2 — Q4 organic +8%, largest vertical, backlog +16%
14. https://agentii.ai/v/PH/ect72/page1 — record FY2026, ~$12B FGC+CIRCOR, filtration tripled

## 6. Verification Table

| # | Number | Source retrieval | Tool call |
|---|---|---|---|
| 1 | FY2026 revenue $21,499M | sec166 page35/page44; XBRL authority-3 fact (2025-07-01→2026-06-30) | read_source_pages; search_xbrl_facts |
| 2 | Motion Systems $3,580M (entity_claim) | sec166 page44; XBRL detailed fact | read_source_pages; search_xbrl_facts view=detailed |
| 3 | F&E $6,048M / F&P $4,810M | sec166 page44; XBRL detailed facts | read_source_pages; search_xbrl_facts view=detailed |
| 4 | Aerospace $7,061M + 4 market lines | sec166 page44; XBRL detailed facts | read_source_pages; search_xbrl_facts view=detailed |
| 5 | Geography NA $14,386M / EMEA $4,178M / APAC $2,711M / LatAm $224M | sec166 page44; XBRL geographic facts | read_source_pages; search_xbrl_facts view=detailed |
| 6 | "No single product >1%" verbatim | sec166 page4 | read_source_pages |
| 7 | Q4 FY2026 $5,755M, Q3 $5,486M | XBRL facts (FY total − 9M; Q3 fact) | search_xbrl_facts |
| 8 | DI margin 23.8% / Aero 26.0% / GM 37.7% | sec166 page25/26/23 | read_source_pages |
| 9 | Backlog $12.8B, ~70% within 12 months | sec166 page5 | read_source_pages |
| 10 | "subscription" = 0 occurrences | keyword search over sec166 | search_keyword_in_source |

**T-001 reconciliation:** zero contradictions. Motion Systems $3,580M FY2026, DI op margin 23.8%, consolidated GM 37.7% all re-retrieved fresh and matching T-001 exactly (https://agentii.ai/v/PH/sec166/page44, https://agentii.ai/v/PH/sec166/page25, https://agentii.ai/v/PH/sec166/page23).
