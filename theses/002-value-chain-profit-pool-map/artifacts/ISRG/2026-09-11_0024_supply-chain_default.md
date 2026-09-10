---
artifact_id: "002-ISRG-supply-chain-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: ISRG
skill: supply-chain
mode: default
affix: supply-chain-map
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "8cb3ac1de486"
as_of: 2026-09-11
entity_claims:
  - entity: ISRG
    metric: product_gross_margin_pct
    value: 65.7
    unit: pct
    period: FY2023
    source: "10-K:sec166 page79"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: product_gross_margin_pct
    value: 67.2
    unit: pct
    period: FY2024
    source: "10-K:sec166 page79"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: product_gross_margin_pct
    value: 66.3
    unit: pct
    period: FY2025
    source: "10-K:sec166 page79"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: recurring_revenue_share_pct
    value: 84.0
    unit: pct
    period: FY2025
    source: "10-K:sec166 page78"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: installed_base_units
    value: 11106
    unit: units
    period: FY2025
    source: "10-K:sec166 page69"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: revenue_per_procedure_usd
    value: 1909
    unit: USD
    period: FY2025
    source: "derived: I&A revenue sec166 page77 / da Vinci procedures sec166 page69"
    retrieved_at: 2026-09-11
citations:
  - "ISRG sec166 page15"
  - "ISRG sec166 page25"
  - "ISRG sec166 page31"
  - "ISRG sec166 page32"
  - "ISRG sec166 page49"
  - "ISRG sec166 page60"
  - "ISRG sec166 page65"
  - "ISRG sec166 page69"
  - "ISRG sec166 page77"
  - "ISRG sec166 page78"
  - "ISRG sec166 page79"
  - "ISRG sec166 page91"
  - "ISRG sec140 page14"
  - "XBRL us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax (FY2023-FY2025)"
  - "XBRL us-gaap:GrossProfit (FY2024-FY2025)"
pillars_addressed: [PIL-1, PIL-2]
claim_state: pinned
key_metrics:
  product_gross_margin_pct_FY2023: 65.7
  product_gross_margin_pct_FY2024: 67.2
  product_gross_margin_pct_FY2025: 66.3
  service_gross_margin_pct_FY2025: 64.6
  consolidated_gross_margin_pct_FY2025: 66.0
  consolidated_gross_margin_pct_FY2024: 67.5
  revenue_usd_FY2025: 10064700000
  product_revenue_usd_FY2025: 8492600000
  instruments_accessories_revenue_usd_FY2025: 6018900000
  systems_revenue_usd_FY2025: 2473700000
  service_revenue_usd_FY2025: 1572100000
  system_asp_usd_FY2025: 1600000
  installed_base_units_FY2025: 11106
  manufacturing_headcount_share_pct_FY2025: 44.8
  tariff_cost_of_revenue_impact_usd_FY2025: 63000000
conclusions:
  - "PIL-1: ISRG keeps the actuation-heavy content of the da Vinci value chain in-house — instruments & accessories (the motion layer) are 70.9% of product revenue, manufacturing operations are 44.8% of headcount, and production spans owned US/MX/EU sites plus a China JV."
  - "PIL-2: Sourcing is a large multi-supplier base on purchase orders with sole-/single-source exceptions and minimal finished-goods inventory; China exposure runs through rare-earth/magnet inputs and the Shanghai JV, not through outsourced actuation assembly."
  - "GM series FY2023-FY2025 (product 65.7/67.2/66.3; consolidated 66.4/67.5/66.0) reconciles exactly with the T-001 baseline and XBRL; the 2025 compression is tariff/ramp-driven, not a structural BOM-cost shift."
facts_count: 24
deducted_count: 8
views_count: 4
citation_count: 15
---

# ISRG Supply-Chain Map — da Vinci Integrated System (PIL-1 / PIL-2)

## Executive Summary

Intuitive Surgical's supply chain is vertically owned for the actuation-heavy content of its value chain. Instruments and accessories — the motion-layer content — are manufactured in-house at Sunnyvale, CA and Mexicali, MX, and represent 70.9% of product revenue [DEDUCTED, https://agentii.ai/v/ISRG/sec166/page77]. Manufacturing operations are 44.8% of the 17,021-employee workforce [DEDUCTED, https://agentii.ai/v/ISRG/sec166/page25], confirming the T-001 45% claim. Components are bought from a large supplier base via purchase orders with sole-/single-source exceptions; the company holds minimal finished-goods inventory [FACT, https://agentii.ai/v/ISRG/sec166/page15]. Product gross margin held at 66.3% in FY2025 (65.7% FY2023, 67.2% FY2024) despite a $63.0M tariff hit to cost of revenues, confirming margin resilience of the integrated-system model [FACT, https://agentii.ai/v/ISRG/sec166/page79]. Key concentration nodes: Mexicali instruments (FDA-registered, never inspected), German-made endoscopes, and China-controlled rare-earth inputs [FACT, https://agentii.ai/v/ISRG/sec166/page32].

## Data Sources

| Source | Coverage | Use |
|---|---|---|
| ISRG FY2025 10-K (`sec166`, filed 2026-02-03, year ended 2025-12-31) | 130-page outline + 13 pages deep-read | Manufacturing, suppliers, headcount, GM series, ASP |
| ISRG FY2023 10-K (`sec140`, filed 2024-01-31) | keyword filter + 1 page deep-read | Footprint continuity check |
| XBRL `us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax` | FY2023/24/25, 10-K authority | Multi-period revenue verification |
| XBRL `us-gaap:GrossProfit` | FY2024/25, 10-K authority | Gross-profit verification |
| Preflight: search_companies, get_ticker_coverage, get_company_fiscal_calendar | — | Entity + calendar resolution |

Note: `get_company_fiscal_calendar` returns `fiscal_year_end_month: 1`, conflicting with the SEC-visible Dec-31 year end (`isrg-20251231.htm`); per task instruction the calendar-year convention is used (FY2025 = year ended 2025-12-31).

## Analysis

### PIL-1 — Integrated system's supplier chain (how actuation-heavy content reaches the product)

**Manufacturing footprint (FY2025)** [FACT, https://agentii.ai/v/ISRG/sec166/page15]:
- Systems: Sunnyvale, California; Peachtree Corners, Georgia; Joint-Venture facility in Shanghai, China.
- Instruments & accessories (the actuation layer — EndoWrist wristed instruments, staplers, energy devices): Sunnyvale, CA and Mexicali, Mexico.
- Ion platform: Blacksburg, Virginia. Endoscopes (the sensing layer): Parvomay, Bulgaria and multiple sites in Germany.

The FY2023 10-K shows the identical systems/instruments structure (Sunnyvale, Peachtree Corners, Shanghai JV, Mexicali, Germany sites), i.e., the vertically-owned model predates the 2024-2025 expansion cycle [FACT, https://agentii.ai/v/ISRG/sec140/page14]. The FY2025 disclosure newly specifies Blacksburg (Ion) and Parvomay, Bulgaria (endoscopes).

**Component sourcing** [FACT, https://agentii.ai/v/ISRG/sec166/page15]: custom and off-the-shelf components are purchased from "a large number of suppliers" under stringent quality specs; some components are sole-sourced (only recognized source) or single-sourced (only approved source). The majority of components and major assemblies are bought via purchase orders rather than long-term supply agreements, and the company "generally do[es] not maintain large volumes of finished goods" — a pull-style replenishment model in which customer instrument orders ship within one business day [FACT, https://agentii.ai/v/ISRG/sec166/page15]. The risk factors attribute the sole/single-source structure to quality considerations, unique IP, and regulatory constraints [FACT, https://agentii.ai/v/ISRG/sec166/page31].

**Manufacturing headcount**: 7,625 of 17,021 employees (Dec 31, 2025) are in manufacturing operations — 44.8% [DEDUCTED from FACTs at https://agentii.ai/v/ISRG/sec166/page25]. R&D 2,288; commercial/service 4,837; administrative 2,271. Headcount +1,383 in 2025; turnover 9.3% [FACT, https://agentii.ai/v/ISRG/sec166/page25]. This confirms the T-001 45%-manufacturing-headcount evidence.

**Actuation-heavy content proxy**: instruments & accessories revenue of $6,018.9M is 70.9% of product revenue and 59.8% of total revenue in FY2025 [DEDUCTED from FACT tables, https://agentii.ai/v/ISRG/sec166/page77]. Every procedure consumes a fresh instrument set at $900–$3,700 of I&A revenue per procedure [FACT, https://agentii.ai/v/ISRG/sec166/page77] — the actuation layer is the consumable profit engine, not a one-time BOM line.

**Critical-material exposure to the actuation layer**: rare-earth elements (used in magnets — i.e., actuator content) are critical to certain components, China is the predominant producer, and in 2025 China announced export controls/licensing on products containing Chinese-origin rare earths [FACT, https://agentii.ai/v/ISRG/sec166/page32]. Endoscopes are primarily manufactured in Germany and imported into the U.S. [FACT, https://agentii.ai/v/ISRG/sec166/page79].

**Cost-side pressure points (FY2025)**: new/incremental tariffs plus trade measures increased cost of revenues by approximately $63.0M, with a further increase expected in 2026 [FACT, https://agentii.ai/v/ISRG/sec166/page65]. Q4-2025 saw isolated supply stresses at specific subcontract suppliers and for component materials impacted by trade requirements, with no material impact to date [FACT, https://agentii.ai/v/ISRG/sec166/page65]. Product GM decline in 2025 was driven by tariffs, incremental fixed overhead/depreciation from expanded manufacturing capacity, and da Vinci 5 ramp costs, partially offset by lower excess-and-obsolete charges [FACT, https://agentii.ai/v/ISRG/sec166/page79].

### PIL-2 — Sourcing structure

**Vertical integration**: owned facilities total ~4.1M sq ft on 128 acres in Sunnyvale (HQ, R&D, service, some manufacturing), ~1.7M sq ft on 69 acres in Peachtree Corners, GA, plus ~1.1M sq ft leased across U.S. manufacturing/engineering/warehousing. OUS: owned/leased properties in Mexicali (MX), Germany, Bulgaria (manufacturing), Aubonne (CH, international HQ); China JV leases R&D/manufacturing/sales facilities; Israel leases R&D [FACT, https://agentii.ai/v/ISRG/sec166/page60].

**Supplier structure**: many suppliers, purchase-order-based, minimal finished-goods and component inventory, with sole-/single-source exceptions. Single-sourced components have identifiable alternative suppliers, but re-verification of a new manufacturer is time- and cost-heavy [FACT, https://agentii.ai/v/ISRG/sec166/page31] [FACT, https://agentii.ai/v/ISRG/sec166/page32]. Supplier-insolvency risk (elevated rates) is explicitly flagged for sole/single-source suppliers [FACT, https://agentii.ai/v/ISRG/sec166/page34].

**Concentration nodes** [VIEW]:
1. Mexicali, Mexico — wholly owned, makes reusable AND disposable instruments; FDA-registered but never FDA-inspected; an import hold would cut supply to "the majority of our customers" [FACT, https://agentii.ai/v/ISRG/sec166/page49].
2. Germany — primary endoscope (vision/sensing) manufacturing region [FACT, https://agentii.ai/v/ISRG/sec166/page79].
3. China-sourced rare earths/magnets — actuation-component input exposure [FACT, https://agentii.ai/v/ISRG/sec166/page32].

**China positioning**: the Shanghai JV manufactures systems for the China market; da Vinci Xi imports into China carry tariffs that adversely affect product cost there [FACT, https://agentii.ai/v/ISRG/sec166/page65]. For the PIL-2 falsifier's proxy question (non-China vs China sourcing for actuation hardware), ISRG demonstrates the integrated-OEM pattern: actuation assembly is non-China (US/MX/EU), while magnet/rare-earth inputs remain China-exposed [VIEW].

### Falsifier-threshold observations

- **PIL-1a** (`actuation_plus_sensing_share_of_bom_pct < 55 falsifies`): no BOM-cost breakdown is disclosed in SEC filings (coverage gap). Revenue-level proxy: instruments & accessories alone are 70.9% of product revenue; adding vision/endoscope content pushes the proxy above the 55% line [VIEW, https://agentii.ai/v/ISRG/sec166/page77]. Teardown figures remain [VIEW]-grade per T-001.
- **PIL-1b** (`motion_model_gm_gap_change_pp < -10 falsifies`): the ISRG (motion-layer anchor) input series is now pinned: product GM 65.7% (FY2023) → 67.2% (FY2024) → 66.3% (FY2025) [FACT, https://agentii.ai/v/ISRG/sec166/page79]. YoY deltas: +1.5pp then −0.9pp [DEDUCTED]. The FY2025 dip is tariff/ramp-driven with revenue +21%, so the motion-layer margin held within 1pp of prior-year peak despite a $63.0M tariff hit [VIEW, https://agentii.ai/v/ISRG/sec166/page65].
- **PIL-2** (humanoid BOM cost ratio): ISRG serves as the integrated-system sourcing reference; ratio computation belongs to the synthesis phase (Deviation Register entry per T-001).

## Key Metrics

| Metric | FY2023 | FY2024 | FY2025 | Source |
|---|---|---|---|---|
| Product revenue ($M) | 5,956.3 | 7,045.0 | 8,492.6 | https://agentii.ai/v/ISRG/sec166/page91 |
| Product cost of revenue ($M) | 2,041.8 | 2,313.1 | 2,866.1 | https://agentii.ai/v/ISRG/sec166/page91 |
| **Product gross margin (%)** | **65.7** | **67.2** | **66.3** | https://agentii.ai/v/ISRG/sec166/page79 |
| Service gross margin (%) | 69.8 | 69.0 | 64.6 | https://agentii.ai/v/ISRG/sec166/page79 |
| Consolidated gross margin (%) | 66.4 [DEDUCTED] | 67.5 | 66.0 | https://agentii.ai/v/ISRG/sec166/page69, page91 |
| Total revenue ($M) | 7,124.1 | 8,352.1 | 10,064.7 | https://agentii.ai/v/ISRG/sec166/page91 |
| I&A revenue ($M) | 4,276.6 | 5,079.0 | 6,018.9 | https://agentii.ai/v/ISRG/sec166/page77 |
| Recurring revenue % of total | 83 | 84 | 84 | https://agentii.ai/v/ISRG/sec166/page78 |
| System ASP ($M, excl. leases/Ion/trade-ins) | — | 1.50 | 1.60 | https://agentii.ai/v/ISRG/sec166/page78 |
| da Vinci installed base (units) | — | 9,902 | 11,106 | https://agentii.ai/v/ISRG/sec166/page69 |
| Manufacturing headcount share (%) | — | — | 44.8 [DEDUCTED] | https://agentii.ai/v/ISRG/sec166/page25 |
| Tariff impact on cost of revenues ($M) | — | — | 63.0 | https://agentii.ai/v/ISRG/sec166/page65 |

GM-series consistency check: product GM recomputed from the income statement (product revenue − product cost) yields 65.72% / 67.17% / 66.25% [DEDUCTED, https://agentii.ai/v/ISRG/sec166/page91], matching the disclosed 65.7/67.2/66.3 within rounding. T-001 baselines (66.3% product GM, 66.0% total GM, ASP ~$1.60M for FY2025) reconcile exactly.

## Coverage Gaps & Citations

**Gaps**:
1. No BOM or cost-stack decomposition (actuation vs sensing vs compute share) is disclosed — PIL-1a can only be proxied at revenue level; teardown data required.
2. Named sole-source suppliers are not disclosed (only the structural fact); no supplier-concentration percentages.
3. `RFCCExcludingAssessedTax` did not resolve in the `isrg` custom namespace via `list_xbrl_concepts` (0 rows); verification used the us-gaap equivalent `us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax`, which matched the 10-K exactly for FY2023 ($7,124.1M), FY2024 ($8,352.1M), FY2025 ($10,064.7M) at 10-K authority. `us-gaap:GrossProfit` XBRL also matched: $5,634.2M (FY2024), $6,642.3M (FY2025).
4. `get_company_fiscal_calendar` reports a January fiscal-year-end month that conflicts with the Dec-31 year-end visible in SEC filing metadata; calendar-year convention used per task instruction.
5. MX (Mexicali) production-volume share is not quantified ("majority of our customers" is qualitative).
6. China JV financials not separable (minority interest $20.6M FY2025 net income attribution at https://agentii.ai/v/ISRG/sec166/page91).

**Citation index** (roll-up; inline links above):
- https://agentii.ai/v/ISRG/sec166/page15 — Manufacturing, suppliers, replenishment model
- https://agentii.ai/v/ISRG/sec166/page25 — Human capital / headcount
- https://agentii.ai/v/ISRG/sec166/page31 — Sole/single-source risk factor
- https://agentii.ai/v/ISRG/sec166/page32 — Rare earths, China export controls
- https://agentii.ai/v/ISRG/sec166/page34 — Macro/supplier insolvency
- https://agentii.ai/v/ISRG/sec166/page49 — Mexicali facility
- https://agentii.ai/v/ISRG/sec166/page60 — Properties (Item 2)
- https://agentii.ai/v/ISRG/sec166/page65 — Tariffs, Q4-2025 supply stresses, China imports
- https://agentii.ai/v/ISRG/sec166/page69 — FY2025 highlights
- https://agentii.ai/v/ISRG/sec166/page77 — Revenue tables, pricing ranges
- https://agentii.ai/v/ISRG/sec166/page78 — ASP, recurring revenue
- https://agentii.ai/v/ISRG/sec166/page79 — Product/service gross-profit tables and drivers
- https://agentii.ai/v/ISRG/sec166/page91 — Consolidated income statements
- https://agentii.ai/v/ISRG/sec140/page14 — FY2023 manufacturing footprint

## Verification

| # | Claim | Check | Result |
|---|---|---|---|
| V1 | Product GM FY2025 = 66.3% | 10-K table (sec166 page79) vs income-statement recompute 66.25% | PASS (rounding) |
| V2 | Consolidated GM FY2025 = 66.0% | 6,642.3/10,064.7 = 65.99% (page91) vs highlight (page69) | PASS |
| V3 | Revenue FY2023/24/25 | 10-K page91 vs XBRL RFCC-ExcludingAssessedTax ($7,124.1M / $8,352.1M / $10,064.7M, authority 3) | PASS (exact) |
| V4 | Gross profit FY2024/25 | 10-K page91 vs XBRL GrossProfit ($5,634.2M / $6,642.3M, authority 3) | PASS (exact) |
| V5 | ASP FY2025 ~$1.60M | page78 discloses $1.60M (2025) vs $1.50M (2024) | PASS |
| V6 | 45% manufacturing headcount (T-001) | 7,625 / 17,021 = 44.8% (page25) | PASS |
| V7 | I&A share of product revenue 70.9% | 6,018.9 / 8,492.6 (page77/page91) | PASS (arithmetic) |
| V8 | Product GM series YoY deltas | +1.5pp (FY2024), −0.9pp (FY2025) | PASS (arithmetic) |
