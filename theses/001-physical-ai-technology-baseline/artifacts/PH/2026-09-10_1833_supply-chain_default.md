---
artifact_id: "001-PH-supply-chain-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: PH
skill: supply-chain
mode: default
affix: supply-chain-map
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "8cb3ac1de486"
as_of: 2026-09-10
entity_claims:
  - "PH Motion Systems platform is the company's actuator/motor/controls revenue line: $3,580M FY2026, $3,341M FY2025, $3,706M FY2024 (10-K disaggregation)"
  - "PH discloses rare earths among 'a limited number of suppliers for certain critical components' in FY2026 10-K risk factors"
  - "PH has no robotics/humanoid commentary in FY2026 10-K, Q4 FY2026 or Q3 FY2026 earnings transcripts (keyword retrieval: zero hits)"
citations:
  - "https://agentii.ai/v/PH/sec166/3"
  - "https://agentii.ai/v/PH/sec166/4"
  - "https://agentii.ai/v/PH/sec166/5"
  - "https://agentii.ai/v/PH/sec166/6"
  - "https://agentii.ai/v/PH/sec166/11"
  - "https://agentii.ai/v/PH/sec166/19"
  - "https://agentii.ai/v/PH/sec166/23"
  - "https://agentii.ai/v/PH/sec166/25"
  - "https://agentii.ai/v/PH/sec166/26"
  - "https://agentii.ai/v/PH/sec166/44"
  - "https://agentii.ai/v/PH/sec166/45"
  - "https://agentii.ai/v/PH/sec166/51"
  - "https://agentii.ai/v/PH/sec166/52"
  - "https://agentii.ai/v/PH/ect72/2"
  - "https://agentii.ai/v/PH/ect72/5"
  - "https://agentii.ai/v/PH/ect72/6"
  - "https://agentii.ai/v/PH/ect71/3"
  - "https://agentii.ai/v/PH/ect71/4"
pillars_addressed: [PIL-1, PIL-2, PIL-4]
claim_state: pinned
key_metrics:
  motion_systems_revenue_fy2026_m: 3580
  motion_systems_revenue_fy2025_m: 3341
  motion_systems_revenue_fy2024_m: 3706
  diversified_industrial_revenue_fy2026_m: 14438
  aerospace_systems_revenue_fy2026_m: 7061
  total_revenue_fy2026_m: 21499
  total_backlog_fy2026_b: 12.8
  aerospace_backlog_fy2026_m: 8498
  di_backlog_fy2026_m: 4332
  inventory_raw_materials_fy2026_m: 639
  inventory_total_fy2026_m: 3166
  scf_payables_balance_fy2026_m: 262
  iiepa_tariff_refund_fy2026_m: 84
  manufacturing_plants: 323
  countries_of_operation: 43
  data_center_pct_of_sales: 1.5
conclusions:
  - "Motion Systems is PH's direct actuator/motion content: electric & hydraulic pumps/motors, electromechanical & hydraulic actuators, drives/controllers; $3,580M FY2026 = 16.6% of company revenue"
  - "Rare-earth magnet and motor-component sourcing is disclosed only qualitatively (supply-concentration risk factor); no NdPr volumes, supplier names, or material-cost breakdown in filings — constitution NdPr price note unverifiable from PH corpus"
  - "PH is vertically integrated in motion-control manufacturing (323 plants, 43 countries, majority owned); customer base is atomized (no single product >1% of sales); aerospace supply chain reported healthy"
  - "PH's physical-AI exposure is indirect today: data center/liquid cooling (~1.5% of sales) plus automation capex served by Motion Systems; zero robotics/humanoid mentions in the last three reporting-period sources"
facts_count: 31
deducted_count: 6
views_count: 3
citation_count: 18
---

# PH (Parker-Hannifin) — Supply-Chain Map: Actuator/Motion Component Chain

## Executive Summary

Parker-Hannifin's Motion Systems technology platform — electric and hydraulic pumps and motors, electromechanical and hydraulic actuators, pneumatics, drives and controllers — is the most direct listed-company proxy for the actuator/motion BOM that the thesis (PIL-2) places at 40–70% of humanoid cost. Motion Systems generated $3,580M of revenue in FY2026 (FY2025: $3,341M; FY2024: $3,706M) https://agentii.ai/v/PH/sec166/44. Parker discloses that it relies on "a limited number of suppliers for certain critical components, such as specialty electronics, rare earths, specialty chemicals, aerospace super alloys and filtration media" https://agentii.ai/v/PH/sec166/11 — the only quantitative-grade rare-earth disclosure is absent; material costs are not broken out. Manufacturing is deeply vertically integrated: 323 plants across 43 countries, majority owned https://agentii.ai/v/PH/sec166/19. Customers are atomized (no single product >1% of net sales) https://agentii.ai/v/PH/sec166/4. Robotics/humanoid commentary is entirely absent from the FY2026 10-K and the last two earnings transcripts. PH's physical-AI exposure today is indirect: data-center liquid cooling (~1.5% of sales) https://agentii.ai/v/PH/ect72/6 and automation-driven factory capex served by Motion Systems.

## Data Sources

- **FY2026 Form 10-K** (filed 2026-08-21, FYE 2026-06-30): PH sec166 — pages 3, 4, 5, 6, 11, 19, 23, 25, 26, 44, 45, 51, 52
- **Q4 FY2026 earnings call transcript** (2026-08-06): PH ect72 — pages 2, 5, 6
- **Q3 FY2026 earnings call transcript** (2026-04-30): PH ect71 — pages 3, 4
- **Structured XBRL**: `us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax` (view=detailed, segment/product/geographic dimensions, FY2026 10-K authority=3); `us-gaap:RevenueRemainingPerformanceObligation` (backlog, $12.8B at 2026-06-30, authority=3); `get_company_financials` consolidated highlights (FY2026: revenue $21,499M, operating income $5,068M, COGS $13,397M, R&D $267M, capex $459M, OCF $4,364M)

## Analysis

### 1. Motion Systems: the actuator/motion component chain (PIL-2)

The Diversified Industrial (DI) segment disaggregates revenue by technology platform. Motion Systems — electric and hydraulic pumps and motors, electromechanical and hydraulic actuators, pneumatic actuators, electronics/drives/controllers — is the platform containing the actuator and motor content that constitutes the humanoid motion BOM [FACT] https://agentii.ai/v/PH/sec166/44.

| Technology platform (DI) | FY2026 | FY2025 | FY2024 |
|---|---|---|---|
| Motion Systems | $3,580M | $3,341M | $3,706M |
| Flow and Process Control | $4,810M | $4,518M | $4,673M |
| Filtration and Engineered Materials | $6,048M | $5,806M | $6,079M |

Source: FY2026 10-K revenue disaggregation table [FACT] https://agentii.ai/v/PH/sec166/44.

- Motion Systems = 16.6% of total company net sales in FY2026 ($3,580M / $21,499M) [DEDUCTED] https://agentii.ai/v/PH/sec166/44.
- Motion Systems + Aerospace Systems ($7,061M) = $10,641M, or 49.5% of company revenue, sits in motion-control/actuation platforms; Aerospace products include electromechanical actuators, flight control systems, hydraulic pumps and motors [FACT; DEDUCTED] https://agentii.ai/v/PH/sec166/4 https://agentii.ai/v/PH/sec166/44.
- Motion Systems FY2026 grew 7.2% YoY but remains below the FY2024 level, consistent with the two-year industrial destocking cycle now turning [DEDUCTED] https://agentii.ai/v/PH/sec166/44.
- Quarterly trajectory: H1 FY2026 (Jul–Dec 2025) Motion Systems revenue $1,717M; Q2 FY2026 alone $893M — the platform is re-accelerating into the FY2027 guidance [FACT via XBRL, authority=2] https://agentii.ai/v/PH/sec166/44.
- No single product contributed more than 1% of total net sales — a structural atomization that caps single-BOM exposure [FACT] https://agentii.ai/v/PH/sec166/4.

### 2. Rare-earth and critical-component sourcing (PIL-2 / PIL-4)

The FY2026 10-K risk factors name rare earths explicitly among components sourced from a limited supplier base: "We rely on a limited number of suppliers for certain critical components, such as specialty electronics, rare earths, specialty chemicals, aerospace super alloys and filtration media, and recent and planned acquisitions may increase our exposure to supply concentration risk" [FACT] https://agentii.ai/v/PH/sec166/11.

- Principal raw materials disclosed: steel, brass, copper, aluminum, nickel, rubber, thermoplastic materials and chemicals, expected "available from numerous sources" [FACT] https://agentii.ai/v/PH/sec166/6. Note rare earths are classed with the *critical/limited-supplier* group, not the commodity group — an implicit admission of NdFeB-style magnet dependency [VIEW].
- Raw materials inventory at FY2026: $639M of total inventory $3,166M (20.2%) [FACT; DEDUCTED] https://agentii.ai/v/PH/sec166/51.
- No quantitative rare-earth data exists in the corpus: no supplier names, no NdPr volumes or pricing. The constitution's NdPr oxide ~$95–110/kg ex-China note cannot be verified or refuted from PH filings [VIEW] — Coverage Gap.
- Tariff context: the U.S. Supreme Court ruled in February 2026 that IEEPA tariffs were unauthorized; PH recognized an $84M reduction to cost of sales in Q4 FY2026 from IEEPA tariff refunds received, with additional refund applications pending [FACT] https://agentii.ai/v/PH/sec166/23.
- Management's tariff posture: "Price-cost management has been a core element of the Win Strategy for over 25 years… we do not expect this to have any impact" on earnings [FACT] https://agentii.ai/v/PH/ect71/3.

### 3. Customer concentration

- PH serves "several hundred thousand OEMs and distribution customer locations" across six market verticals [FACT] https://agentii.ai/v/PH/sec166/3. No customer-concentration table is presented in the 10-K, and with no single product above 1% of sales, no single customer can plausibly exceed 10% of revenue [DEDUCTED] https://agentii.ai/v/PH/sec166/4.
- Channel mix: industrial business is exactly 50% OEM / 50% aftermarket, with distribution historically 10–15 points higher-margin than OEM [FACT] https://agentii.ai/v/PH/ect71/4.
- Geographic revenue (by selling location): North America $14,386M, EMEA $4,178M, Asia Pacific $2,711M, Latin America $224M [FACT] https://agentii.ai/v/PH/sec166/44. Asia Pacific = 12.6% of revenue, concentrated in electronics/semiconductor and data-center demand [DEDUCTED] https://agentii.ai/v/PH/ect71/4.
- Backlog: total $12.8B at 2026-06-30 vs $11.0B at 2025-06-30 (record; XBRL RPO confirms $12.8B, authority=3) [FACT] https://agentii.ai/v/PH/sec166/5 https://agentii.ai/v/PH/sec166/45; Aerospace Systems backlog $8,498M, DI backlog $4,332M [FACT] https://agentii.ai/v/PH/sec166/26 https://agentii.ai/v/PH/sec166/25.

### 4. Vertical integration (PIL-1)

- Manufacturing footprint: approximately 323 manufacturing plants, in 35 U.S. states and 43 other countries; the majority of manufacturing plants are owned, not leased [FACT] https://agentii.ai/v/PH/sec166/19.
- In-house actuator/motor production is intrinsic to the product catalog — PH *manufactures* electric and hydraulic pumps and motors, electromechanical and hydraulic actuators, drives and controllers across both segments [FACT] https://agentii.ai/v/PH/sec166/4.
- Management: "We manufacture in many regions of the world, which allows us to be very competitive locally" — regionalized manufacturing as tariff/geopolitical hedge [FACT] https://agentii.ai/v/PH/ect71/4.
- Supply-chain financing: voluntary SCF programs; $262M supplier-invoice balance outstanding at FY2026 (vs $175M FY2025), $740M invoices confirmed during the year — supplier liquidity support instrument, not a purchasing obligation [FACT] https://agentii.ai/v/PH/sec166/51 https://agentii.ai/v/PH/sec166/52.
- Aerospace supply-chain health: "The aerospace supply chain is in much better shape than it has been… Over the last several years, we have invested quite a bit in our supply chain" — Parker participates in big-airframer production-rate increases [FACT] https://agentii.ai/v/PH/ect71/4.
- Capacity: capex ~2.5% of sales (management-confirmed; ~$459M FY2026 per XBRL cash-flow fact, 10-K authority 3; management cited ~$500M invested on the Q4 call), with capacity expansion built into FY2027 and lean/Kaizen output gains keeping capacity additions low [FACT] https://agentii.ai/v/PH/ect72/5 https://agentii.ai/v/PH/ect72/2.
- Workforce: ~59,850 team members, of whom ~30,830 in foreign subsidiaries [FACT] https://agentii.ai/v/PH/sec166/6.

### 5. Robotics / humanoid / physical-AI commentary (PIL-4)

- Keyword retrieval for "robot" returns zero hits in the FY2026 10-K, the Q4 FY2026 transcript, and the Q3 FY2026 transcript [FACT] — verified via `search_keyword_in_source` (sec166, ect72, ect71).
- The only adjacent language: "Customer spending on automation continues to lead the growth" in in-plant/industrial (FY2027 guidance) [FACT] https://agentii.ai/v/PH/ect72/2, and distributor-end customers "focused on automation and productivity" capital investments [FACT] https://agentii.ai/v/PH/ect71/4.
- Data-center exposure: ~1.5% of sales and growing (was "~1%" in prior commentary); products include hoses, couplings, manifolds, fittings, engineered materials for thermal management, and liquid-cooling systems and subsystem components sold to industry leaders [FACT] https://agentii.ai/v/PH/ect72/6.
- [VIEW] PH is a picks-and-shovels beneficiary of physical-AI *infrastructure* (data-center liquid cooling, factory automation capex) but has no disclosed humanoid-robot content program; Motion Systems' humanoid exposure is indirect via customer automation investment. This is the single most important PIL-4 negative evidence for the thesis: the largest listed actuator franchise does not yet claim a humanoid revenue stream.

### 6. Demand and order momentum (supply-chain leading indicators)

- Q4 FY2026: total organic growth +8%; total orders +19% on a 3-month basis and +12% on a rolling 12-month basis; backlog +16% YoY at record $12.8B [FACT] https://agentii.ai/v/PH/ect72/2.
- North America industrial orders +16% (3-month) in Q4 FY2026, broad-based across aerospace & defense, in-plant, distribution, construction, heavy-duty truck, commercial HVAC [FACT] https://agentii.ai/v/PH/ect72/5.
- International orders +24% (3-month), driven by electronics and in-plant; Asia Pacific organic growth +16% in Q4 [FACT] https://agentii.ai/v/PH/ect72/2 https://agentii.ai/v/PH/ect72/5.
- Distributors "ordering to demand for rather quick consumption" — no channel restock, no supply-chain fear-buying detected as of Q3 FY2026 [FACT] https://agentii.ai/v/PH/ect71/3.
- FY2027 guidance: 7% organic growth at midpoint, first-ever positive growth across all market verticals [FACT] https://agentii.ai/v/PH/ect72/2.

## Key Metrics

| Metric | Value | Period | Citation |
|---|---|---|---|
| Motion Systems revenue | $3,580M | FY2026 | https://agentii.ai/v/PH/sec166/44 |
| Motion Systems revenue | $3,341M / $3,706M | FY2025 / FY2024 | https://agentii.ai/v/PH/sec166/44 |
| Diversified Industrial revenue | $14,438M | FY2026 | https://agentii.ai/v/PH/sec166/44 |
| Aerospace Systems revenue | $7,061M | FY2026 | https://agentii.ai/v/PH/sec166/44 |
| Total net sales | $21,499M | FY2026 | https://agentii.ai/v/PH/sec166/23 |
| Total backlog | $12.8B | 2026-06-30 | https://agentii.ai/v/PH/sec166/5 |
| Aerospace / DI backlog | $8,498M / $4,332M | 2026-06-30 | https://agentii.ai/v/PH/sec166/26 |
| Inventories (raw materials / total) | $639M / $3,166M | 2026-06-30 | https://agentii.ai/v/PH/sec166/51 |
| SCF supplier-payable balance | $262M | FY2026 | https://agentii.ai/v/PH/sec166/52 |
| IEEPA tariff refund (cost-of-sales reduction) | $84M | Q4 FY2026 | https://agentii.ai/v/PH/sec166/23 |
| Manufacturing plants | 323 | 2026-06-30 | https://agentii.ai/v/PH/sec166/19 |
| Data-center exposure | ~1.5% of sales | FY2026 | https://agentii.ai/v/PH/ect72/6 |
| Q4 FY2026 organic growth / orders | +8% / +19% (3-mo) | Q4 FY2026 | https://agentii.ai/v/PH/ect72/2 |
| FY2027 organic growth guidance | 7% (midpoint) | FY2027 | https://agentii.ai/v/PH/ect72/2 |

## Coverage Gaps & Citations

**Coverage gaps** (unretrievable from corpus — not invented):
1. No robotics/humanoid-specific disclosure in any PH filing or transcript retrieved (zero "robot" keyword hits in sec166, ect72, ect71).
2. No quantitative rare-earth/magnet sourcing data: no supplier names, volumes, or NdPr pricing; the constitution NdPr oxide ~$95–110/kg note is unverifiable from PH filings.
3. No customer-concentration table (no >10% customer disclosed; only qualitative product-atomization evidence).
4. No platform-level COGS or gross margin for Motion Systems (`us-gaap:CostOfRevenue` and `Revenues` concepts not tagged for PH; revenue is tagged only as `RevenueFromContractWithCustomerExcludingAssessedTax`).
5. No supplier names anywhere in the corpus (SEC standard for PH; supplier concentration is qualitative only).
6. Market/price data absent by mandate (market_data_stage: none).

**Citation index** (non-duplicative roll-up):
1. https://agentii.ai/v/PH/sec166/3 — business/segments overview, 67/33 split
2. https://agentii.ai/v/PH/sec166/4 — principal products, no product >1% of sales
3. https://agentii.ai/v/PH/sec166/5 — backlog $12.8B
4. https://agentii.ai/v/PH/sec166/6 — raw materials, energy, acquisitions
5. https://agentii.ai/v/PH/sec166/11 — rare earths limited-supplier risk factor
6. https://agentii.ai/v/PH/sec166/19 — properties: 323 plants, 35 states, 43 countries
7. https://agentii.ai/v/PH/sec166/23 — consolidated results, IEEPA $84M refund
8. https://agentii.ai/v/PH/sec166/25 — DI segment results, DI backlog $4,332M
9. https://agentii.ai/v/PH/sec166/26 — Aerospace segment results, backlog $8,498M
10. https://agentii.ai/v/PH/sec166/44 — revenue disaggregation by platform/segment/geography
11. https://agentii.ai/v/PH/sec166/45 — contract balances, $12.8B backlog note
12. https://agentii.ai/v/PH/sec166/51 — inventories components, SCF program description
13. https://agentii.ai/v/PH/sec166/52 — SCF rollforward table
14. https://agentii.ai/v/PH/ect72/2 — Q4 FY2026 results, orders, FY2027 guidance
15. https://agentii.ai/v/PH/ect72/5 — capacity/capex, NA order drivers
16. https://agentii.ai/v/PH/ect72/6 — data center ~1.5%, liquid cooling
17. https://agentii.ai/v/PH/ect71/3 — tariff price-cost posture, distributor ordering behavior
18. https://agentii.ai/v/PH/ect71/4 — aerospace supply-chain health, 50/50 OEM-aftermarket, local manufacturing

## Verification

Every material number above traces to a retrieval call made in this run. Call trace:

| # | Tool call | Result used | Artifact citation |
|---|---|---|---|
| 1 | search_companies (PH) | Parker-Hannifin Corp, CIK 0000076334, NYSE, FYE June | preflight |
| 2 | get_ticker_coverage (PH) | 59 SEC filings, 20,714 XBRL facts, 19 transcripts | preflight |
| 3 | get_company_fiscal_calendar (PH) | FY2026 Q4 ends 2026-06-30 | preflight |
| 4 | search_sec_filings (10-K) | sec166 = FY2026 10-K (filed 2026-08-21) | /v/PH/sec166/* |
| 5 | search_documents (transcripts) | 19 transcripts, latest 2026-08-06 | — |
| 6 | list_sources (PH, ect) | source_id → citation_id mapping | — |
| 7 | read_source_outline (sec166) | 79-page map; selected supply-chain pages | /v/PH/sec166/* |
| 8 | read_source_outline (2026-08-06 ect) | ect72 | /v/PH/ect72/* |
| 9 | read_source_outline (2026-04-30 ect) | ect71 | /v/PH/ect71/* |
| 10 | read_source_pages (sec166, pages 3,6,11) | segments split; raw materials; rare-earth risk | /v/PH/sec166/3,6,11 |
| 11 | read_source_pages (sec166, pages 44,25) | Motion Systems $3,580M; DI segment table | /v/PH/sec166/44,25 |
| 12 | read_source_pages (sec166, pages 26,51,52) | Aerospace table; inventories; SCF table | /v/PH/sec166/26,51,52 |
| 13 | read_source_pages (sec166, page 23) | IEEPA $84M refund; consolidated results | /v/PH/sec166/23 |
| 14 | read_source_pages (sec166, pages 4,19) | product catalog; 323 plants | /v/PH/sec166/4,19 |
| 15 | read_source_pages (ect72, pages 2,5,6) | Q4 results, orders, data center 1.5% | /v/PH/ect72/2,5,6 |
| 16 | read_source_pages (ect71, pages 3,4) | tariff posture; aero supply chain | /v/PH/ect71/3,4 |
| 17 | search_keyword_in_source (sec166, "robot") | 0 hits — robotics absence | gap #1 |
| 18 | search_keyword_in_source (ect72, "robot") | 0 hits — robotics absence | gap #1 |
| 19 | search_keyword_in_source (ect72, "automation") | page 2 — automation demand | /v/PH/ect72/2 |
| 20 | search_keyword_in_source (ect71, "robot") | 0 hits — robotics absence | gap #1 |
| 21 | list_xbrl_concepts ("revenue") | concept inventory | — |
| 22 | search_xbrl_facts (RFCCExcludingAssessedTax, FY2026, detailed) | platform/segment/geographic revenue facts | /v/PH/sec166/44 |
| 23 | search_xbrl_facts ("Revenues", FY2026) | 0 facts — concept not tagged | gap #4 |
| 24 | search_xbrl_facts ("CostOfRevenue", FY2026) | 0 facts — concept not tagged | gap #4 |
| 25 | search_xbrl_facts (RFCCIncludingAssessedTax, FY2026) | 0 facts — concept not tagged | gap #4 |
| 26 | search_xbrl_facts (RPO) | backlog $12.8B @2026-06-30 (authority 3) | /v/PH/sec166/45 |
| 27 | search_xbrl_facts (RFCCExcludingAssessedTax, FY2025 partial) | H1 FY2026 Motion Systems $1,717M; Q2 $893M | /v/PH/sec166/44 |
| 28 | get_company_financials (PH) | FY2026: rev $21,499M, opInc $5,068M, COGS $13,397M, R&D $267M, capex $459M, OCF $4,364M | /v/PH/sec166/23 |

Tool diversity: 12 distinct tools used (requirement ≥8). Retrieval path: Layer 1 → Layer 2 → Layer 2.5 → Layer 3 followed per the supply-chain skill protocol; structured XBRL cross-validation on both revenue concept and backlog. No numbers were sourced from model priors; every figure carries an inline /v/ citation from an actual retrieval call.
