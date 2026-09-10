---
artifact_id: "002-PH-supply-chain-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: PH
skill: supply-chain
mode: default
affix: supply-chain-map
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "8cb3ac1de486"
as_of: 2026-09-11
entity_claims:
  - entity: PH
    metric: motion_systems_revenue_usd
    value: 3580000000
    unit: USD
    period: 2026Q4
    source: "10-K:page44"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: motion_systems_revenue_usd
    value: 3341000000
    unit: USD
    period: 2025Q4
    source: "10-K:page44"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: motion_systems_revenue_usd
    value: 3706000000
    unit: USD
    period: 2024Q4
    source: "10-K:page44"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: diversified_industrial_segment_operating_margin_pct
    value: 23.8
    unit: pct
    period: 2026Q4
    source: "10-K:page25"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: consolidated_gross_margin_pct
    value: 37.7
    unit: pct
    period: 2026Q4
    source: "10-K:page23"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: consolidated_gross_margin_pct
    value: 36.9
    unit: pct
    period: 2025Q4
    source: "10-K:page23"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: consolidated_gross_margin_pct
    value: 35.8
    unit: pct
    period: 2024Q4
    source: "10-K:page35"
    retrieved_at: 2026-09-11
  - entity: PH
    metric: consolidated_gross_margin_pct
    value: 37.3
    unit: pct
    period: 2026Q4
    source: "10-K:page35 (ex-IEEPA)"
    retrieved_at: 2026-09-11
citations:
  - "https://agentii.ai/v/PH/sec166/3"
  - "https://agentii.ai/v/PH/sec166/4"
  - "https://agentii.ai/v/PH/sec166/5"
  - "https://agentii.ai/v/PH/sec166/6"
  - "https://agentii.ai/v/PH/sec166/10"
  - "https://agentii.ai/v/PH/sec166/11"
  - "https://agentii.ai/v/PH/sec166/19"
  - "https://agentii.ai/v/PH/sec166/23"
  - "https://agentii.ai/v/PH/sec166/25"
  - "https://agentii.ai/v/PH/sec166/26"
  - "https://agentii.ai/v/PH/sec166/35"
  - "https://agentii.ai/v/PH/sec166/44"
  - "https://agentii.ai/v/PH/sec166/51"
  - "https://agentii.ai/v/PH/sec166/52"
  - "https://agentii.ai/v/PH/sec127/11"
pillars_addressed: [PIL-1, PIL-2]
claim_state: pinned
key_metrics:
  motion_systems_revenue_usd_fy2026: 3580000000
  motion_systems_revenue_usd_fy2025: 3341000000
  motion_systems_revenue_usd_fy2024: 3706000000
  consolidated_gross_margin_pct_fy2026: 37.7
  consolidated_gross_margin_pct_fy2026_ex_iiepa: 37.3
  consolidated_gross_margin_pct_fy2025: 36.9
  consolidated_gross_margin_pct_fy2024: 35.8
  diversified_industrial_operating_margin_pct_fy2026: 23.8
  aerospace_operating_margin_pct_fy2026: 26.0
  backlog_usd_jun2026: 12800000000
  diversified_industrial_backlog_usd_jun2026: 4332000000
  aerospace_backlog_usd_jun2026: 8498000000
  manufacturing_plants_count: 323
  iiepa_tariff_refund_cost_of_sales_reduction_usd_q4fy2026: 84000000
  scf_ending_balance_usd_fy2026: 262000000
  raw_materials_inventory_usd_jun2026: 639000000
  non_us_selling_location_sales_share_pct_fy2026: 36
  asia_pacific_revenue_usd_fy2026: 2711000000
conclusions:
  - "PIL-1 supply-chain evidence holds: 323 plants, in-house manufacture of motion-control systems and components, and a highly fragmented customer base; external supplier reliance is confined to specialty inputs (rare earths, specialty electronics, aerospace super alloys, specialty chemicals, filtration media)."
  - "PIL-2 China-cost dynamics: the rare-earth 'limited suppliers' disclosure is NEW in the FY2026 10-K (absent from FY2025); China is flagged as a trade-barrier risk; no quantitative China/rare-earth cost data is disclosed — proxy-only support, as anticipated by the Deviation Register."
  - "Consolidated GM series (PIL-1b test input): 35.8% FY2024 → 36.9% FY2025 → 37.7% FY2026; FY2026 includes ~40bp of non-recurring IEEPA tariff-refund benefit (ex-IEEPA 37.3%)."
  - "Tariff/IEEPA exposure is material but two-sided: $84M refund recognized in Q4 FY2026 cost of sales; additional refund applications pending and unbooked; raw-material tariff risk and price pass-through lag disclosed."
  - "All four T-001 baselines reconciled (Motion Systems $3,580M, DI op margin 23.8%, GM 37.7%, backlog $12.8B). The get_segment_data gold-vs-filed conflict could not be re-tested (tool INTERNAL_ERROR); 10-K values are authoritative per directive."
facts_count: 34
deducted_count: 10
views_count: 5
citation_count: 15
---

# PH Supply-Chain Map — thesis 002 (PIL-1, PIL-2)

> Counting convention: the frontmatter `facts_count` / `deducted_count` /
> `views_count` reflect FACT / DEDUCTED / VIEW tags in the Analysis and Key
> Metrics sections. The Executive Summary restates headline items untagged.
> Every number below was retrieved via agentii MCP in this run; uncited
> numbers are void (P4 audit mandate).

## Executive Summary

Parker-Hannifin's motion layer is a vertically integrated supply chain: ~323
plants in 35 U.S. states and 43 countries manufacture motion-control systems
and components in-house (10-K p19, p44). Supplier dependence is confined to
specialty inputs — the FY2026 10-K newly discloses reliance on a "limited
number of suppliers" for rare earths, specialty electronics, aerospace super
alloys, specialty chemicals and filtration media; the FY2025 10-K carried no
such sentence, a fresh China-linked sourcing risk flag for PIL-2 (p11).
Customer concentration is negligible ("several hundred thousand" OEM and
distribution customer locations; no product above 1% of sales, p3–4). Tariff
exposure is real but two-sided: Q4 FY2026 recognized an $84M IEEPA tariff
refund reducing cost of sales, with further refunds applied for but unbooked
(p23). The PIL-1b GM series runs 35.8% (FY2024) → 36.9% (FY2025) → 37.7%
(FY2026); ~40bp of FY2026 is non-recurring IEEPA benefit (ex-IEEPA 37.3%).
Motion Systems revenue was $3,580M in FY2026 (p44); DI operating margin 23.8%
(p25); backlog $12.8B (p5). All four T-001 baselines reconcile.

## Data Sources

Retrieval was via agentii MCP only, three-layer protocol. Pre-flight:
`search_companies` (PH → Parker-Hannifin Corp, CIK 0000076334), 
`get_ticker_coverage`, `get_company_fiscal_calendar` (fiscal year ends June 30;
FY2026 = 2025-07-01 → 2026-06-30). Layer 1: `search_sec_filings` +
`search_documents` (10-K forms). Layer 2: `read_source_outline` on the FY2026
10-K (`sec166`, filed 2026-08-21, report date 2026-06-30), plus
`search_keyword_in_source` filters (rare earth, magnet, tariff, IEEPA,
customer, China, 10%, critical components) on `sec166` and the FY2025 10-K
(`sec127`, report date 2025-06-30). Layer 3: `read_source_pages` on `sec166`
pages 3, 4, 5, 6, 10, 11, 19, 23, 25, 26, 35, 44, 51, 52 and `sec127` page 11.
XBRL: `search_xbrl_facts` for
`RevenueFromContractWithCustomerExcludingAssessedTax` (PH, FY periods);
`get_segment_data` (product axis) was attempted twice and returned
`INTERNAL_ERROR: column "k" does not exist` both times.

## Analysis

### 1. Motion-layer supply-chain footprint (PIL-1)

- [FACT] At June 30, 2026 PH maintained approximately 323 manufacturing
  plants, situated in 35 U.S. states and 43 other countries; the majority are
  owned, none individually material — https://agentii.ai/v/PH/sec166/19
- [FACT] The Diversified Industrial Segment is "an aggregation of several
  business units, which manufacture a broad range of motion-control systems
  and components" — in-house manufacture, not contract assembly —
  https://agentii.ai/v/PH/sec166/44
- [FACT] Principal raw materials are steel, brass, copper, aluminum, nickel,
  rubber and thermoplastic materials and chemicals, "expected … to be
  available from numerous sources" — https://agentii.ai/v/PH/sec166/6
- [FACT] Headcount at June 30, 2026: ~59,850 employees, of whom ~30,830 in
  foreign subsidiaries — https://agentii.ai/v/PH/sec166/6
- [FACT] Motion Systems (the actuation-layer platform) 3-year revenue series:
  $3,580M FY2026, $3,341M FY2025, $3,706M FY2024; Flow and Process Control
  $4,810M and Filtration and Engineered Materials $6,048M in FY2026 (DI total
  $14,438M) — https://agentii.ai/v/PH/sec166/44
- [DEDUCTED] Vertical integration is high: the company manufactures its
  motion-control systems and components across its own plant network, with
  disclosed external-supplier reliance confined to specialty inputs (see §2);
  raw-materials inventory of $639M against total inventories of $3,166M is
  consistent with in-house transformation of purchased feedstock rather than
  outsourced sub-assembly — https://agentii.ai/v/PH/sec166/51
- [VIEW] Actuation-plus-sensing share of BOM (PIL-1a falsifier) cannot be
  validated from filings; no teardown or BOM data is disclosed. Per the
  entities.md falsifier table, teardown figures would be VIEW-only.

### 2. Rare-earth / supplier concentration (PIL-2 test input)

- [FACT] FY2026 10-K risk factor: "We rely on a limited number of suppliers
  for certain critical components, such as specialty electronics, rare
  earths, specialty chemicals, aerospace super alloys and filtration media,
  and recent and planned acquisitions may increase our exposure to supply
  concentration risk" — https://agentii.ai/v/PH/sec166/11
- [FACT] The FY2025 10-K contains no such limited-supplier sentence; its
  corresponding risk factor covers only raw-material price pass-through and
  supplier price increases — https://agentii.ai/v/PH/sec127/11
- [DEDUCTED] The rare-earth sourcing disclosure is NEW in the FY2026 filing
  (keyword "rare earths" returns 0 hits in `sec127`; the sentence does not
  exist there) — https://agentii.ai/v/PH/sec166/11
- [DEDUCTED] The disclosure addition coincides with the pending CIRCOR
  Aerospace acquisition and the completed FGC acquisition, which the filing
  itself links to increased supply-concentration risk ("recent and planned
  acquisitions may increase our exposure to supply concentration risk") —
  https://agentii.ai/v/PH/sec166/11
- [VIEW] The disclosure expansion is consistent with PIL-2's China-dependency
  premise but quantifies nothing (no volumes, no costs, no named suppliers).
  It is proxy-only support; the PIL-2 falsifier remains un-measurable from
  filings (Deviation Register expiry 2026-10-10).

### 3. Customer concentration

- [FACT] "We serve several hundred thousand original equipment manufacturers
  (OEMs) and distribution customer locations" —
  https://agentii.ai/v/PH/sec166/3
- [FACT] "No single product contributed more than one percent to our total
  net sales for the year ended June 30, 2026" —
  https://agentii.ai/v/PH/sec166/4
- [DEDUCTED] The FY2026 10-K discloses no numeric customer-concentration
  percentage (keyword sweep for "10%" surfaced no concentration table);
  concentration on the demand side is effectively negligible, while
  concentration on the supply side is explicitly disclosed for specialty
  inputs (§2).
- [VIEW] The concentration asymmetry — fragmented customers, concentrated
  specialty suppliers — puts the bottleneck at the specialty-input layer,
  supporting the thesis's profit-pool framing in which rare-earth/magnet and
  specialty-material suppliers hold pricing leverage over the motion layer.

### 4. Tariff / IEEPA impacts

- [FACT] In February 2026 the U.S. Supreme Court ruled IEEPA tariffs on
  imported goods unauthorized; in Q4 FY2026 PH recognized a $84M reduction to
  cost of sales from IEEPA tariff refunds received from the U.S. government —
  https://agentii.ai/v/PH/sec166/23
- [FACT] PH has applied for additional refunds under the same program "though
  for lesser amounts"; no receivable has been recorded as amount and timing
  are uncertain — https://agentii.ai/v/PH/sec166/23
- [FACT] Tariff and import/export regulation changes "have in the past and
  may in the future have a negative impact on the availability and pricing of
  raw materials"; price pass-through to customers is subject to time delays
  and contract terms — https://agentii.ai/v/PH/sec166/11
- [FACT] Risk factors cite renegotiation of the United States-Mexico-Canada
  Agreement and "possible restrictions on trade and/or obstacles to
  conducting business in China" —
  https://agentii.ai/v/PH/sec166/11, https://agentii.ai/v/PH/sec166/10
- [FACT] FY2026 gross margin increased "primarily due to higher margins in
  both segments primarily driven by sales volume, partially offset by
  unfavorable product mix and increased material costs" —
  https://agentii.ai/v/PH/sec166/23
- [VIEW] The $84M refund directly lowered FY2026 cost of sales; the
  un-booked additional refunds are upside, but the underlying ruling implies
  PH had been absorbing IEEPA tariffs on imports before the ruling — a
  China-linked cost headwind that the refund path only partially reverses.

### 5. Segment economics and backlog

- [FACT] Diversified Industrial FY2026: net sales $14,438M, segment operating
  income $3,440M, operating margin 23.8% (vs 22.8% FY2025); North America
  margin 24.3%, International 23.1% — https://agentii.ai/v/PH/sec166/25
- [FACT] DI margin drivers: favorable pricing and prior-year divestiture
  benefits, partially offset by unfavorable product mix, increased material
  costs and higher intangible amortization —
  https://agentii.ai/v/PH/sec166/25
- [FACT] Aerospace Systems FY2026: net sales $7,061M, segment operating
  income $1,833M, operating margin 26.0% (vs 23.3% FY2025) —
  https://agentii.ai/v/PH/sec166/26
- [FACT] Segment backlog at June 30, 2026: DI $4,332M (vs $3,655M) and
  Aerospace $8,498M (vs $7,389M) —
  https://agentii.ai/v/PH/sec166/25, https://agentii.ai/v/PH/sec166/26
- [FACT] Total backlog $12.8B at June 30, 2026 vs $11.0B at June 30, 2025;
  ~70% scheduled for delivery within twelve months —
  https://agentii.ai/v/PH/sec166/5
- [DEDUCTED] Segment backlogs sum to $12,830M, reconciling to the stated
  $12.8B total — https://agentii.ai/v/PH/sec166/25
- [DEDUCTED] Motion Systems is 24.8% of DI segment revenue ($3,580M ÷
  $14,438M) and 16.7% of consolidated revenue in FY2026 —
  https://agentii.ai/v/PH/sec166/44

### 6. Geography and China exposure (PIL-2 context)

- [FACT] "Our net sales attributable to selling locations outside of the
  United States were approximately 36% in each of 2026, 2025 and 2024" —
  https://agentii.ai/v/PH/sec166/10
- [FACT] Geographic revenue (selling-operation basis) FY2026: North America
  $14,386M, EMEA $4,178M, Asia Pacific $2,711M, Latin America $224M —
  https://agentii.ai/v/PH/sec166/44
- [DEDUCTED] Asia Pacific is 12.6% of FY2026 revenue ($2,711M ÷ $21,499M);
  the page-44 table implies non-US share of 33.1% ($7,113M ÷ $21,499M),
  versus the 36% stated in the risk factors — a ~2.9pp basis discrepancy
  within the same filing, flagged for the synthesis (both figures are as
  filed).
- [FACT] Non-U.S. operations are subject to "transportation delays and other
  supply chain disruptions … the imposition of duties and tariffs and other
  trade barriers … including possible restrictions on trade and/or obstacles
  to conducting business in China" — https://agentii.ai/v/PH/sec166/10

### 7. Supply-chain financing and working capital

- [FACT] SCF programs: suppliers may elect early payment from financial
  intermediaries; participation is voluntary, payment terms are consistent
  with or without participation, and PH does not reimburse supplier costs —
  https://agentii.ai/v/PH/sec166/51
- [FACT] SCF roll-forward FY2026: beginning balance $175M, invoices confirmed
  $740M, settled $651M, ending balance $262M (vs $175M FY2025) —
  https://agentii.ai/v/PH/sec166/52
- [FACT] Inventories at June 30, 2026: finished products $849M, work in
  process $1,678M, raw materials $639M, total $3,166M (vs $2,839M FY2025) —
  https://agentii.ai/v/PH/sec166/51
- [VIEW] The ~50% YoY growth in SCF balances ($175M → $262M) is consistent
  with supplier-liquidity support during tariff-driven input-cost pressure,
  though the program remains small relative to payables.

### 8. XBRL cross-check and segment-data conflict

- [FACT] XBRL `RevenueFromContractWithCustomerExcludingAssessedTax` (us-gaap,
  is_primary, source_authority 3 for FY): FY2026 $21,499M (period_end
  2026-06-30, ph-20260630.htm), FY2025 $19,850M, FY2024 $19,930M — identical
  to the Consolidated Statements of Income —
  https://agentii.ai/v/PH/sec166/35
- [FACT] `get_segment_data` (product axis, FY2026) failed on both attempts
  with `INTERNAL_ERROR: column "k" does not exist` — the gold product-axis
  dataset is currently unavailable via the MCP tool; filed FY2025 Motion
  Systems value confirmed at $3,341M — https://agentii.ai/v/PH/sec166/44
- [DEDUCTED] The T-001 conflict (gold $3,830M vs filed $3,341M for FY2025
  Motion Systems) therefore remains unresolved; per the task directive
  ("the 10-K wins"), filed values are authoritative for this artifact —
  https://agentii.ai/v/PH/sec166/44
- [FACT] "magnet" keyword search returns zero hits in the FY2026 10-K: PH
  makes no magnet-specific sourcing disclosure; magnets are subsumed under
  the "rare earths" critical-component category —
  https://agentii.ai/v/PH/sec166/11

### 9. T-001 baseline reconciliation (fresh retrieval)

| T-001 baseline | Fresh retrieval | Status | Citation |
|---|---|---|---|
| Motion Systems $3,580M FY2026 | $3,580M FY2026 | Match [FACT] | https://agentii.ai/v/PH/sec166/44 |
| DI op margin 23.8% | 23.8% (vs 22.8% FY2025) | Match [FACT] | https://agentii.ai/v/PH/sec166/25 |
| Consolidated GM 37.7% | 37.7% FY2026 (36.9% FY2025) | Match [FACT] | https://agentii.ai/v/PH/sec166/23 |
| Backlog $12.8B | $12.8B at 6/30/2026; segment sum $12,830M | Match [FACT] | https://agentii.ai/v/PH/sec166/5 |

All four rows above are FACT-tagged (retrieved this run) and included in the
frontmatter `facts_count`.

## Key Metrics

Consolidated gross-margin series (PIL-1b test input; PH fiscal year ends June
30 — periods aligned by period_end):

| Period (period_end) | Net sales $M | Cost of sales $M | Gross margin | Basis | Citation |
|---|---|---|---|---|---|
| FY2024 (2024-06-30) | 19,930 | 12,802 | 35.8% [DEDUCTED] | computed: (19,930−12,802)/19,930 = 35.76% | https://agentii.ai/v/PH/sec166/35 |
| FY2025 (2025-06-30) | 19,850 | 12,535 | 36.9% [FACT] | MD&A-stated; recompute 36.85% agrees | https://agentii.ai/v/PH/sec166/23 |
| FY2026 (2026-06-30) | 21,499 | 13,397 | 37.7% [FACT] | MD&A-stated; recompute 37.68% agrees | https://agentii.ai/v/PH/sec166/23 |
| FY2026 ex-IEEPA | 21,499 | 13,397 + 84 | 37.3% [DEDUCTED] | adds back $84M refund to cost of sales (~40bp) | https://agentii.ai/v/PH/sec166/23 |

Other headline metrics (re-statements of tagged items above; untagged to
avoid double counting):

| Metric | Value | Citation |
|---|---|---|
| Motion Systems revenue FY2026 / FY2025 / FY2024 | $3,580M / $3,341M / $3,706M | https://agentii.ai/v/PH/sec166/44 |
| DI operating margin FY2026 | 23.8% (op income $3,440M) | https://agentii.ai/v/PH/sec166/25 |
| Aerospace operating margin FY2026 | 26.0% ($7,061M sales) | https://agentii.ai/v/PH/sec166/26 |
| Backlog 6/30/2026 (DI $4,332M + Aero $8,498M) | $12.8B total | https://agentii.ai/v/PH/sec166/5 |
| Manufacturing plants | 323 (35 US states, 43 countries) | https://agentii.ai/v/PH/sec166/19 |
| IEEPA tariff refund, Q4 FY2026 | $84M reduction to cost of sales | https://agentii.ai/v/PH/sec166/23 |
| Non-US selling-location sales | ~36% (each of FY2024–FY2026) | https://agentii.ai/v/PH/sec166/10 |
| SCF ending balance FY2026 | $262M (from $175M) | https://agentii.ai/v/PH/sec166/52 |

## Coverage Gaps & Citations

Coverage gaps:

1. `get_segment_data` (product axis) returns `INTERNAL_ERROR: column "k"
   does not exist` on both attempts — the T-001 gold-vs-filed conflict
   (gold $3,830M vs filed $3,341M, FY2025 Motion Systems) cannot be
   re-tested; 10-K values used per directive and the conflict stays flagged.
2. No magnet-specific sourcing disclosure exists (keyword "magnet": 0 hits in
   the FY2026 10-K); rare-earth exposure is disclosed only qualitatively.
3. No numeric customer-concentration percentage is disclosed in the FY2026
   10-K; concentration evidence is qualitative (hundreds of thousands of
   customer locations; no product >1% of sales).
4. No quantitative China cost/rare-earth data (volumes, prices, supplier
   names) — PIL-2 remains proxy-only; consistent with the Deviation Register
   entry in entities.md (§3).
5. The FY2024 10-K MD&A was not deep-read; the FY2024 GM is computed from the
   three-year income statement in the FY2026 10-K (sec166 page 35).
6. No price data used, per mandate.

Citation index (roll-up; non-duplicative of inline links above):

- sec166 (FY2026 10-K, filed 2026-08-21): pages 3, 4, 5, 6, 10, 11, 19, 23,
  25, 26, 35, 44, 51, 52 — https://agentii.ai/v/PH/sec166/3 through
  https://agentii.ai/v/PH/sec166/52
- sec127 (FY2025 10-K, filed 2025-08-22): page 11 —
  https://agentii.ai/v/PH/sec127/11

## Verification

| # | Number | Retrieved from | Cross-check | Status |
|---|---|---|---|---|
| 1 | Motion Systems $3,580M FY2026 | sec166 p44 | T-001 baseline $3,580M | Verified |
| 2 | Motion Systems $3,341M FY2025 | sec166 p44 | T-001 gold $3,830M (conflict side "filed") | Filed confirmed; gold side untestable (tool error) — flagged |
| 3 | DI op margin 23.8% FY2026 | sec166 p25 | T-001 baseline 23.8% | Verified |
| 4 | GM 37.7% FY2026 | sec166 p23 | p35 compute 37.68% | Verified |
| 5 | GM 36.9% FY2025 | sec166 p23 | p35 compute 36.85% | Verified |
| 6 | GM 35.8% FY2024 | sec166 p35 (computed) | line-item arithmetic | Deducted, verified |
| 7 | GM ex-IEEPA 37.3% FY2026 | sec166 p23 + p35 | 84/21,499 ≈ 0.39pp | Deducted, verified |
| 8 | Backlog $12.8B 6/30/2026 | sec166 p5 | DI $4,332M + Aero $8,498M = $12,830M | Verified |
| 9 | Revenue FY2026 $21,499M | XBRL (authority 3) | sec166 p35/p44 | Verified (3 years) |
| 10 | 323 plants | sec166 p19 | T-001 claim | Verified |
| 11 | Non-US sales ~36% | sec166 p10 | p44 table implies 33.1% | Intra-filing basis discrepancy ~2.9pp — flagged |
| 12 | Rare-earth "limited suppliers" | sec166 p11 | sec127 p11: sentence absent (0 keyword hits) | New FY2026 disclosure — confirmed |
