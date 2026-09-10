---
artifact_id: "001-PH-unit-economics-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: PH
skill: unit-economics
mode: default
affix: unit-economics
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "e87ee63269a2"
as_of: 2026-09-10
entity_claims:
  - "PH FY2026 net sales $21,499M; Diversified Industrial $14,438M (67%), Aerospace Systems $7,061M (33%)"
  - "Motion Systems platform revenue FY2026 $3,580M, 16.7% of PH consolidated sales; +7.2% YoY after -9.8% in FY2025"
  - "Motion Systems has no disclosed platform-level operating income; DI segment margin 23.8%, Aerospace 26.0%"
  - "PH discloses no humanoid/robotics content-per-platform economics; BOM split remains industry estimate"
  - "PH FY2026 adj segment operating margin 27.3%; new FY2031 target 30%; FY2027 guide 27.7%"
citations:
  - "https://agentii.ai/v/PH/sec166/23"
  - "https://agentii.ai/v/PH/sec166/24"
  - "https://agentii.ai/v/PH/sec166/25"
  - "https://agentii.ai/v/PH/sec166/26"
  - "https://agentii.ai/v/PH/sec166/44"
  - "https://agentii.ai/v/PH/sec166/45"
  - "https://agentii.ai/v/PH/sec166/67"
  - "https://agentii.ai/v/PH/sec166/68"
  - "https://agentii.ai/v/PH/sec166/3"
  - "https://agentii.ai/v/PH/sec166/4"
  - "https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/1"
  - "https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/2"
  - "https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/3"
  - "https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/4"
  - "https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/5"
  - "https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/6"
pillars_addressed: [PIL-2, PIL-4]
claim_state: pinned
key_metrics:
  net_sales_fy2026: 21499
  diversified_industrial_sales_fy2026: 14438
  aerospace_systems_sales_fy2026: 7061
  motion_systems_sales_fy2026: 3580
  motion_systems_share_of_sales_pct: 16.7
  di_segment_operating_margin_fy2026_pct: 23.8
  aerospace_segment_operating_margin_fy2026_pct: 26.0
  consolidated_gross_margin_fy2026_pct: 37.7
  di_other_segment_items_pct_of_sales: 76.2
  total_backlog_jun2026: 12800
  adj_segment_operating_margin_fy2026_pct: 27.3
  fy2031_margin_target_pct: 30.0
  fy2027_organic_growth_guide_midpoint_pct: 7.0
conclusions:
  - "PH is a defensible public-market proxy for the actuator/drive cost pool, but its filings contain zero humanoid BOM data; the 40-70% actuator vs 10-15% compute split remains an external industry estimate that PH data can neither confirm nor falsify"
  - "The motion/actuation business carries premium economics: 23.8-26.0% segment operating margins and 37.7% consolidated gross margin imply actuators are high-value engineered content, consistent with a large share of any robot BOM, but no dollar content per platform is disclosed"
  - "Motion Systems is a mid-size, cyclical platform (FY2026 $3.58B, -9.8% FY2025, +7.2% FY2026) inside a segment whose growth is being driven elsewhere; PH's motion capability spans DI (hydraulic/electric actuators, drives) and Aerospace (flight controls, electromechanical actuators)"
facts_count: 34
deducted_count: 7
views_count: 3
citation_count: 16
---

# PH — Unit Economics (default): The Actuator/Dollar Evidence Base for PIL-2

## 1. Executive Summary

Parker-Hannifin (PH) is the best available public-market proxy for "who earns the actuator/drive dollar," the cost-stack evidence behind PIL-2. FY2026 net sales were $21,499M ([FACT] https://agentii.ai/v/PH/sec166/23). The motion-relevant revenue pools are large and disclosable: Motion Systems platform $3,580M, 16.7% of consolidated sales ([FACT] https://agentii.ai/v/PH/sec166/44); Diversified Industrial (DI) segment $14,438M at 23.8% segment operating margin; Aerospace Systems $7,061M at 26.0% ([FACT] https://agentii.ai/v/PH/sec166/24). Consolidated gross margin is 37.7% ([FACT] https://agentii.ai/v/PH/sec166/23). The actuation cost stack at the segment level equals 76.2% of DI sales once segment profit is stripped out ([DEDUCTED] from https://agentii.ai/v/PH/sec166/67). Critically, PH's corpus contains zero humanoid or robotics disclosures ([FACT] keyword sweep, 0 hits in FY2026 10-K) — so the humanoid BOM split (40–70% actuator+drive vs 10–15% compute) remains an industry estimate that PH data can characterize but not verify. PH's premium margins and product breadth (electromechanical/hydraulic actuators, pumps/motors, drives/controllers) are consistent with actuators being high-value BOM content, but no content-per-platform dollar is disclosed.

## 2. Core Analysis

### 2.1 Segment and Platform Structure of the Motion Dollar

PH operates two reportable segments: of FY2026 net sales of $21.5B, DI products were 67% and Aerospace Systems 33% ([FACT] https://agentii.ai/v/PH/sec166/3). Within DI, the 10-K disaggregates revenue by technology platform:

| Platform (FY, $M) | 2026 | 2025 | 2024 |
|---|---|---|---|
| Motion Systems | 3,580 | 3,341 | 3,706 |
| Flow and Process Control | 4,810 | 4,518 | 4,673 |
| Filtration and Engineered Materials | 6,048 | 5,806 | 6,079 |
| DI total | 14,438 | 13,665 | 14,458 |

([FACT] https://agentii.ai/v/PH/sec166/44)

Motion Systems therefore contributes 16.7% of consolidated FY2026 sales and 24.8% of DI sales ([DEDUCTED] from https://agentii.ai/v/PH/sec166/44 and https://agentii.ai/v/PH/sec166/23). Its trajectory is cyclical: −9.8% in FY2025 (from $3,706M to $3,341M) followed by +7.2% in FY2026 ([DEDUCTED] from the same table, https://agentii.ai/v/PH/sec166/44). Motion Systems is the closest disclosed analog to humanoid actuation content; Flow and Process Control ($4,810M) and Filtration ($6,048M) are not actuation pools.

Aerospace Systems adds a second, higher-margin motion pool: $7,061M split into Commercial OEM $2,330M, Commercial aftermarket $2,523M, Defense OEM $1,271M, and Defense aftermarket $937M ([FACT] https://agentii.ai/v/PH/sec166/44). Aerospace products include electromechanical actuators, flight control systems, hydraulic pumps/motors, and valves/actuators ([FACT] https://agentii.ai/v/PH/sec166/4) — i.e., the same actuator+drive categories PIL-2 identifies in the humanoid BOM, but at aerospace price points and with no dollar split by product line (coverage gap).

### 2.2 Margin Structure of the Motion/Actuation Business (BOM cost-stack evidence)

- DI segment operating income $3,440M on $14,438M = 23.8% margin, up 100bps YoY from 22.8% ([FACT] https://agentii.ai/v/PH/sec166/25). North America DI: $2,041M on $8,392M = 24.3%; International: $1,399M on $6,046M = 23.1% ([FACT] https://agentii.ai/v/PH/sec166/25).
- Aerospace Systems segment operating income $1,833M on $7,061M = 26.0%, up 270bps from 23.3% ([FACT] https://agentii.ai/v/PH/sec166/26). Combined segment operating income $5,273M ([FACT] https://agentii.ai/v/PH/sec166/24).
- Consolidated gross margin 37.7% vs 36.9% in FY2025 ([FACT] https://agentii.ai/v/PH/sec166/23); XBRL cost-of-goods fact of $13,397M against $21,499M revenue independently reproduces 37.7% ([FACT] XBRL `CostOfGoodsAndServicesSold`, source_authority 3, filing ph-20260630.htm — call trace §4).
- Implied segment cost stack: DI "Other Segment Items" (net sales minus segment operating income — i.e., all segment-level costs: COGS, SG&A, R&D, D&A) were $10,998M = 76.2% of DI sales in FY2026, versus 77.2% in FY2025 ([DEDUCTED] from https://agentii.ai/v/PH/sec166/67). Aerospace's equivalent is $5,228M = 74.0% of sales ([DEDUCTED] from https://agentii.ai/v/PH/sec166/67).
- Segment D&A: DI depreciation $240M + amortization $280M = $520M in FY2026 ([FACT] https://agentii.ai/v/PH/sec166/67); segment assets: DI $17,001M, Aerospace $12,180M ([FACT] https://agentii.ai/v/PH/sec166/67).
- Cost-stack noise: an $84M IEEPA tariff refund reduced cost of sales in Q4 FY2026 ([FACT] https://agentii.ai/v/PH/sec166/23) — a reminder that even the disclosed cost stack is tariff-sensitive.

Interpretation for PIL-2: at 23.8–26.0% segment operating margins and 37.7% gross margin, actuation/motion hardware is engineered, differentiated content — not commodity metal ([VIEW], anchored on https://agentii.ai/v/PH/sec166/24 and https://agentii.ai/v/PH/sec166/23). This is directionally consistent with actuators commanding a large share of a robot BOM. But nothing in the filings quantifies content per end platform: PH states no single product contributes more than 1% of total net sales ([FACT] https://agentii.ai/v/PH/sec166/4), i.e., no actuator platform is individually dominant — the business is fragmentation and breadth, which is precisely why a humanoid-specific dollar cannot be extracted.

### 2.3 Orders, Backlog and the Near-Term Motion Demand Signal

- Total backlog reached a record $12.8B, up 16% YoY ([FACT] transcript https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/2). DI backlog $4,332M vs $3,655M ([FACT] https://agentii.ai/v/PH/sec166/25); Aerospace backlog $8,498M vs $7,389M ([FACT] https://agentii.ai/v/PH/sec166/26).
- Q4 FY2026 orders: total +19% on the 3-month comparison, +12% on rolling 12-month; North America industrial +16% (3-month), International +24% (3-month), Aerospace +18% ([FACT] https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/2).
- From FY2027 PH switches Industrial order reporting to rolling 12-month rates; management's rationale: Aerospace, Engineered Materials and Filtration have grown from 35% to ~65% of pro forma sales, lengthening cycle exposure ([FACT] https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/1, https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/4). Implication: the pure industrial/motion order signal (closest to robotics-adjacent demand) becomes harder to isolate going forward ([DEDUCTED]).

### 2.4 Electrification and Motion-Capability Acquisitions (the humanoid-adjacent build-out)

- Curtis Instruments (~$1.0B, completed September 2025) was framed by the CEO as enhancing "electrification capabilities" ([FACT] https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/1; 10-K acquisition note https://agentii.ai/v/PH/sec166/45 via page map). Curtis supplies motor-speed controllers and instrumentation — the drive-electronics layer of an actuator stack.
- Pending CIRCOR commercial aerospace & defense (~$2.55B, per 10-K note https://agentii.ai/v/PH/sec166/45 via page map): described as "flight-critical motion and flow control capabilities," CY2026E sales ~$270M at >40% adjusted EBITDA margin, 80% OEM mix, with ~$26M of cost synergies modeled ([FACT] https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/6).
- Pending Filtration Group Corporation ($9.25B) — filtration, not actuation ([FACT] https://agentii.ai/v/PH/sec166/68 via page map / https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/1).
- Data-center liquid cooling exposure (hoses, couplings, manifolds, thermal management) is ~1.5% of sales and growing ([FACT] https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/6) — adjacent "physical AI infrastructure" content, not robot actuation.

### 2.5 The Humanoid BOM Question — What PH Can and Cannot Establish

What PH data supports: the actuator/drive value pool exists at scale and at premium margins; PH manufactures every actuator+drive category named in PIL-2 — "Electromechanical & Hydraulic Actuators," "Electric & Hydraulic Pumps & Motors," "Electronics, Drives & Controllers," "Pneumatic Actuators" ([FACT] https://agentii.ai/v/PH/sec166/4).

What PH data cannot establish: a keyword sweep for "robot" across the FY2026 10-K returns zero pages ([FACT] keyword search, sec166, call trace §4); the Q4 FY2026 earnings call contains no humanoid or robotics discussion ([FACT] full transcript read, https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/1 through /6). There is no content-per-platform disclosure, no unit pricing, and no Motion Systems operating-income disclosure. Consequently: (a) the 40–70% actuator+drive vs 10–15% compute split of a humanoid BOM is an industry estimate that this corpus neither confirms nor falsifies ([VIEW]); (b) the most defensible PIL-2 contribution from PH is the marginal-cost signature: with segment operating margins of 23.8–26.0% and gross margin 37.7%, actuators are among the highest value-added components in any machine that uses them, supporting the top of the BOM-share range but not proving it ([DEDUCTED] anchored on https://agentii.ai/v/PH/sec166/24, https://agentii.ai/v/PH/sec166/23); (c) if humanoid OEMs buy actuation at industrial motion price points, actuator content would plausibly dominate BOM, but PH's disclosed economics (76.2% segment-level cost ratio) are those of a component supplier, not an integrator of a $30–60k robot ([DEDUCTED]).

### 2.6 PIL-4 Support — Financial Runway of the Motion Pure-Play

FY2026: record sales $21.5B, adjusted segment operating margin 27.3% (+120bps), adjusted EPS $32.31 (+18%), operating cash flow $4.4B record (20.3% of sales), free cash flow $3.9B (18.2% of sales) ([FACT] https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/2). Q4 FY2026: sales +10% reported / +8% organic; adjusted segment margin 28.0% (first quarter ever above 28%); Aerospace Q4 margin 29.8% ([FACT] https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/2). FY2027 guidance: organic growth +7% at midpoint (~$23B sales), adjusted segment margin 27.7%, adjusted EPS $34.75 midpoint, free cash flow $3.4–3.9B ([FACT] https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/3). FY2031 target: 30% adjusted segment operating margin, raised from the FY2029 27.0% target already surpassed ([FACT] https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/1). The motion/actuation pool is backed by a cash-generative, margin-expanding parent — relevant to PIL-4's question of which physical-AI suppliers can fund capacity if robot actuation demand scales ([VIEW]).

## 3. Coverage Gaps & Citations

### Coverage Gaps (unretrievable — never invented)

1. **No humanoid/robotics disclosures.** "robot" keyword in FY2026 10-K (sec166): 0 hits; Q4 FY2026 call: no robotics discussion. No humanoid content-per-platform data exists in the corpus.
2. **No platform-level profitability.** Motion Systems has revenue disclosures only; operating income is disclosed at segment level (DI 23.8%, Aerospace 26.0%).
3. **No segment-level COGS/gross margin.** Only consolidated gross margin (37.7%) and the derived "Other Segment Items" ratio (76.2% DI) are available.
4. **No unit pricing or content-per-platform dollars** (e.g., $ actuator content per aircraft/vehicle/robot) in any retrieved document.
5. **XBRL concept sparsity.** PH does not tag `Revenues`, `SalesRevenueNet`, `RevenueFromContractWithCustomerIncludingAssessedTax`, or `GrossProfit`. The single tagged revenue concept (`RevenueFromContractWithCustomerExcludingAssessedTax`) was verified across periods and dimensions instead (§4).
6. **gold segment-table data-quality flag.** `get_segment_data` product-axis values conflict with the 10-K page 44 table (e.g., gold reports Motion Systems FY2025 $3,830M vs 10-K $3,341M; Aerospace FY2025 operating income $854M vs 10-K $1,441M). The 10-K values were used throughout; gold's product-axis rows appear stale or mis-mapped.
7. **Transcript citation IDs.** Transcripts carry no sec-style citation_id; the roll-up below uses the source UUID from `list_sources` (Q4 FY2026 call, 2026-08-06, 7 pages).
8. **No price data** (market_data_stage: none) — no market cap/price-dependent unit metrics; no per-actuator market price available.

### Citation Roll-Up Index

SEC FY2026 10-K (citation_id `sec166`, filed 2026-08-21):
- https://agentii.ai/v/PH/sec166/3 — reportable segments, 67/33 split
- https://agentii.ai/v/PH/sec166/4 — principal products (actuators, pumps/motors, drives)
- https://agentii.ai/v/PH/sec166/23 — consolidated results, gross margin 37.7%
- https://agentii.ai/v/PH/sec166/24 — segment operating income $5,273M
- https://agentii.ai/v/PH/sec166/25 — DI segment detail, backlog $4,332M
- https://agentii.ai/v/PH/sec166/26 — Aerospace detail, backlog $8,498M
- https://agentii.ai/v/PH/sec166/44 — revenue disaggregation by technology platform
- https://agentii.ai/v/PH/sec166/45 — acquisitions note (CIRCOR $2.55B, FGC $9.25B, Curtis $1.0B) [via page map]
- https://agentii.ai/v/PH/sec166/67 — segment assets, D&A, Other Segment Items
- https://agentii.ai/v/PH/sec166/68 — FGC acquisition $9.25B subsequent event [via page map]

Q4 FY2026 earnings call transcript (2026-08-06, source UUID 4fd7d9a7-2082-48ed-96b8-30e70c1f514e):
- https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/1 — FY26 records, FY31 target, Curtis electrification, order-reporting change
- https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/2 — Q4 results, orders, backlog $12.8B, cash flow, FY27 guide
- https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/3 — guidance detail, Q&A
- https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/4 — Q&A: 35%→65% mix shift, aerospace guide
- https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/5 — Q&A: orders by vertical, FY31 walk
- https://agentii.ai/v/PH/4fd7d9a7-2082-48ed-96b8-30e70c1f514e/6 — Q&A: CIRCOR economics, data center ~1.5%

## 4. Verification Table (call trace)

| # | Retrieval call | Result | Used for |
|---|---|---|---|
| 1 | search_companies (PH) | Parker-Hannifin, CIK 0000076334, June FYE | entity resolution |
| 2 | get_ticker_coverage (PH) | 59 sec_filings, 20,714 xbrl_facts, 19 transcripts | routing |
| 3 | get_company_fiscal_calendar (PH) | FY2026 = 2025-07-01→2026-06-30 | period alignment |
| 4 | search_documents (10-K) | FY2026 10-K filed 2026-08-21 | Layer 1 |
| 5 | search_sec_filings (10-K) | citation_id sec166 (FY26), sec127 (FY25) | Layer 1 |
| 6 | list_xbrl_concepts ("Revenue") | PH revenue concept = RevenueFromContractWithCustomerExcludingAssessedTax | concept discovery |
| 7 | get_segment_data (FY2026, all) | segment + platform rows; product-axis values later flagged vs 10-K | segment map |
| 8 | get_segment_data (FY2025, all) | FY2025 comparatives (10-K supersedes product-axis rows) | comparatives |
| 9 | read_source_outline (sec166) | 79-page map; page targets identified | Layer 2 |
| 10 | read_source_pages (sec166 p44,p25,p26) | Motion Systems $3,580M; DI 23.8%; Aero 26.0%; backlogs | core [FACT]s |
| 11 | read_source_pages (sec166 p23,p3,p4) | $21,499M; 67/33; product list; GM 37.7% | core [FACT]s |
| 12 | read_source_pages (sec166 p24,p67) | segment op income $5,273M; Other Segment Items $10,998M; D&A | margin/cost stack |
| 13 | search_xbrl_facts (RevenueFromContractWithCustomerExcludingAssessedTax, FY2026) | $21,499M, authority 3 (10-K) | P2.1 concept A ✓ |
| 14 | search_xbrl_facts (same, FY2025) | $19,850M, authority 3 — matches 10-K table | cross-period ✓ |
| 15 | search_xbrl_facts (same, FY2026, view=detailed) | Motion Systems $3,580M; DI $14,438M; Aero $7,061M dimension facts match p44 | dimensional ✓ |
| 16 | search_xbrl_facts (Revenues, FY2026) | 0 facts — concept not tagged by PH | gap #5 |
| 17 | search_xbrl_facts (SalesRevenueNet / ...IncludingAssessedTax) | 0 facts — not tagged | gap #5 |
| 18 | search_xbrl_facts (CostOfGoodsAndServicesSold, FY2026) | $13,397M → GM 37.7% reproduces p23 | gross margin triangulation ✓ |
| 19 | search_xbrl_facts (GrossProfit) | 0 facts — not tagged | gap #5 |
| 20 | list_sources (earnings_call_transcript) | Q4 FY26 call source_id 4fd7d9a7-… (2026-08-06) | transcript routing |
| 21 | read_source_pages (transcript p1-3) | FY26 records, orders, guidance | [FACT]s |
| 22 | read_source_pages (transcript p4-7) | CIRCOR >40% EBITDA margin; data center 1.5%; no robotics | [FACT]s |
| 23 | search_keyword_in_source (sec166, "robot") | 0 hits | humanoid gap #1 |
| 24 | batch_search (8 sub-queries) | partial: endpoints unsupported; XBRL payloads malformed — results discarded, calls re-run individually | process note |

P2.1 two-concept verification: PH tags a single revenue concept; verification was instead performed on the same concept across two fiscal years and across dimensional axes, each reconciling to the 10-K tables (rows 13–15), plus COGS triangulation of gross margin (row 18). No number in this artifact is unretrieved; all [DEDUCTED] items are arithmetic on cited [FACT]s.
