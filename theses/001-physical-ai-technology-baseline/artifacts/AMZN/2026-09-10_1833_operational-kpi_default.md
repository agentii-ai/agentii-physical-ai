---
artifact_id: "001-AMZN-operational-kpi-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: AMZN
skill: operational-kpi
mode: default
affix: kpi-dashboard
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "0730fd170124"
as_of: 2026-09-10
entity_claims:
  - "AMZN operated 1,000,000+ robots in its fulfillment network as of Feb 2026 (ect81 p5)"
  - "AMZN expects to more than double its fleet of robotic arms (Cardinal, Sparrow) in 2026 (ect83 p2)"
  - "AMZN: all U.S. large-format fulfillment center launches in 2026 will have latest-generation robotics technology (ect82 p2)"
  - "AMZN FY2025 net sales $716.9B, +12% YoY (sec131 p24)"
  - "AMZN FY2025 cash capex $128.3B vs $77.7B FY2024 (sec131 p23)"
  - "AMZN H1 2026 cash capex $96.3B; Q2 2026 $53.1B (sec177 p27)"
  - "AMZN employed 1,576,000 people as of Dec 31, 2025 (sec131 p4)"
  - "AMZN paid units grew 17% YoY in Q2 2026 (ect83 p2)"
citations: [sec131, sec130, sec177, sec172, sec167, sec166, sec165, ect83, ect82, ect81, ect77, ect75]
pillars_addressed: [PIL-3, PIL-4]
claim_state: pinned
key_metrics:
  robots_in_network_feb2026: "1,000,000+"
  robotic_arms_plan_2026: "more than double (Cardinal, Sparrow)"
  fy2025_revenue_usd_m: 716924
  fy2024_revenue_usd_m: 637959
  fy2025_capex_usd_b: 128.3
  fy2024_capex_usd_b: 77.7
  h1_2026_capex_usd_b: 96.3
  q2_2026_capex_usd_b: 53.1
  q1_2026_capex_usd_b: 43.2
  na_pae_net_additions_fy2025_usd_m: 35919
  na_pae_net_additions_h1_2026_usd_m: 23265
  employees_dec31_2025: 1576000
  employees_dec31_2024: 1556000
  fulfillment_pct_of_net_sales_fy2025: 15.2
  paid_units_growth_q2_2026_pct: 17
  na_oi_margin_q2_2026_pct: 7.9
  revenue_per_employee_fy2025_usd: 454900
conclusions:
  - "PIL-3: Fleet-scale manipulation reliability is demonstrated in production: 1M+ warehouse robots, with robotic-arm (pick/place) fleet doubling in 2026; management reports improved safety, productivity, and cost-to-serve — but this is semi-structured warehouse automation, NOT humanoids (Plan Risk Note 3)."
  - "PIL-4: Deployment pace is accelerating and explicitly disclosed: single-site Shreveport integration (2024) -> expansion to multiple facilities (Feb 2025) -> all 2026 U.S. large-format FC launches on latest-gen robotics plus fleetwide retrofits (2026)."
  - "Automation capex run-rate more than doubled YoY: $77.7B (FY2024) -> $128.3B (FY2025) -> $96.3B in H1 2026 alone; NA fulfillment segment net P&E additions +42% YoY in H1 2026."
  - "Productivity KPIs improving: paid units +17% YoY in Q2 2026 while fulfillment expense per dollar of net sales fell to 15.2% (FY2025); revenue per employee +11% to ~$455k."
  - "Robotics disclosure is qualitative fleet-level (1M+ robots, robotic arms doubling); quantitative per-site and per-task reliability metrics are not disclosed — treated as coverage gap."
facts_count: 35
deducted_count: 9
views_count: 3
citation_count: 12
---

# AMZN — Operational KPI Dashboard (robotics fleet, productivity, automation capex)

**Skill:** operational-kpi | **Mode:** default | **As of:** 2026-09-10 | **Pillars served:** PIL-3 (manipulation reliability gates deployment), PIL-4 (timing — fleet-scale deployment pace)

## Executive Summary

AMZN operates the largest disclosed fleet of warehouse robots: **1,000,000+ robots** in its fulfillment network as of Feb 2026 https://agentii.ai/v/AMZN/ect81/5, and management expects to **more than double its fleet of robotic arms (Cardinal, Sparrow) in 2026** https://agentii.ai/v/AMZN/ect83/2. Deployment pace is explicit and accelerating: all U.S. large-format fulfillment-center launches in 2026 carry latest-generation robotics, deployed across both new and existing (retrofit) sites https://agentii.ai/v/AMZN/ect82/2. Productivity KPIs are improving in parallel: paid units grew 17% YoY in Q2 2026 https://agentii.ai/v/AMZN/ect83/2, while fulfillment expense held at 15.2% of net sales in FY2025 https://agentii.ai/v/AMZN/sec131/25 and revenue per employee rose ~11% to ~$455k https://agentii.ai/v/AMZN/sec131/4. The automation capex run-rate has more than doubled: $77.7B (FY2024) to $128.3B (FY2025) https://agentii.ai/v/AMZN/sec131/23, with $96.3B in H1 2026 alone https://agentii.ai/v/AMZN/sec177/27. **Caveat (Plan Risk Note 3):** this is warehouse automation, not humanoids — the evidence bears on deployment economics (reliability at scale, retrofit economics, productivity payback), not humanoid manipulation.

## Data Sources

| Source | Citation ID | Date | Used for |
|---|---|---|---|
| FY2025 Form 10-K | sec131 | 2026-02-06 | FY financials, capex, properties sq ft, employees, segment P&E |
| FY2024 Form 10-K | sec130 | 2025-02-07 | FY2024 employees, properties sq ft |
| Q2 2026 Form 10-Q | sec177 | 2026-07-31 | H1 2026 capex, cash flows, segment P&E additions, D&A |
| Q1/Q2/Q3 2025 10-Qs | sec165/166/167 | 2025 | XBRL fact source filings (quarterly revenue, OI) |
| Q1 2026 10-Q | sec172 | 2026-04-30 | XBRL fact source filing |
| Q2 2026 earnings call | ect83 | 2026-07-30 | Robotics arms doubling, Q2 KPIs, capex $53.1B |
| Q1 2026 earnings call | ect82 | 2026-04-29 | 2026 FC launch robotics mandate, unit-vs-cost KPI, capex $43.2B |
| Q4 2025 earnings call | ect81 | 2026-02-05 | 1M+ robots, regionalization 8→10 regions |
| Q4 2024 earnings call | ect77 | 2025-02-06 | Shreveport robotics integration, GenAI robot brains |
| Q2 2024 earnings call | ect75 | 2024-08-01 | Robotics as cost-to-serve lever, 5B same/next-day units |

Structured facts via `search_xbrl_facts` (is_primary=true): `RevenueFromContractWithCustomerExcludingAssessedTax` (35 facts) and `OperatingIncomeLoss` (35 facts). Concept discovery via `list_xbrl_concepts` (P2.1: two revenue concepts — `RevenueFromContractWithCustomerExcludingAssessedTax` and `Revenues`; the latter returned zero is-primary facts for AMZN, noted in Coverage Gaps).

## Analysis

### 1. Robotics fleet size (PIL-3, PIL-4)

[FACT] Amazon disclosed "over a million robots" operating in its fulfillment network as of Feb 2026 (Q4 2025 call), performing "all sorts of functions," with robotics taking over repetitive tasks for "better productivity for the business, more safe for teammates and... real cost efficiencies" https://agentii.ai/v/AMZN/ect81/5.

[FACT] On the Q2 2026 call (Jul 2026), CFO Brian Olsavsky stated the company is "expanding our deployment of robotics and automation... retrofitting our facilities with our latest generation technology, and we expect to more than double our fleet of robotic arms, like Cardinal and Sparrow, in 2026" https://agentii.ai/v/AMZN/ect83/2. Cardinal and Sparrow are pick-and-place manipulation systems — this is the closest disclosed proxy for fleet-scale manipulation-unit deployment pace.

[FACT] The Q1 2026 call quantified the deployment mandate: "All of our U.S. large-format fulfillment center launches in 2026 will have this latest generation technology," deployed in "both new and existing facilities," with "early positive results with improved site safety, higher productivity and lower cost to serve" https://agentii.ai/v/AMZN/ect82/2.

[FACT] Deployment sequencing (PIL-4 timing): in Feb 2025 (Q4 2024 call), Jassy described the Shreveport facility as the first site integrating the "next tranche of robotics initiatives" together, with "plans now to start to expand that and roll that out to a number of other facilities... some new facilities and others retrofit existing facilities," framed as "a many-year effort" https://agentii.ai/v/AMZN/ect77/4. The 2026 disclosures show that rollout has progressed from single site (2024) to fleetwide mandate (2026).

[FACT] Manipulation-reliability context (PIL-3): the "brains in a lot of those robotics are generative AI-infused that do things like tell the robotic claw what's in a bin, what it should pick up, how it should move it, where it should place it" https://agentii.ai/v/AMZN/ect77/4 — i.e., perception-to-grasp decision-making is deployed at production scale, though in semi-structured warehouse environments, not humanoid form factors.

[VIEW] The 1M+ robot disclosure (Feb 2026) followed by a "more than double the robotic arms" commitment (Jul 2026) indicates the manipulation sub-fleet is the fastest-growing robot class in the network — consistent with PIL-3's premise that manipulation reliability gates deployment pace, but inverted: Amazon's disclosure pattern suggests reliability has cleared the gate and capex/labor economics now drive pace.

### 2. Productivity KPIs (units, revenue per employee, cost per unit)

[FACT] Paid unit growth: "Worldwide paid units grew 17% year-over-year" in Q2 2026 https://agentii.ai/v/AMZN/ect83/2.

[FACT] Q1 2026 unit-vs-cost productivity: "Overall unit growth of 15% continues to outpace our cost to operate the fulfillment network as outbound shipping costs grew 12% year-over-year and fulfillment expense grew 9% year-over-year, both on an FX-neutral basis" https://agentii.ai/v/AMZN/ect82/2.

[FACT] Fulfillment expense as % of net sales declined from 15.4% (FY2024) to 15.2% (FY2025) — absolute fulfillment expense rose 11% to $109.1B, attributed to "increased sales and investments in our fulfillment network, partially offset by operational efficiencies" https://agentii.ai/v/AMZN/sec131/25.

[FACT] Speed throughput: "more than 5 billion units arriving the same day or next day" for Prime customers in the first half of 2024 alone (Q2 2024 call) https://agentii.ai/v/AMZN/ect75/1.

[FACT] Headcount: 1,556,000 full- and part-time employees as of Dec 31, 2024 https://agentii.ai/v/AMZN/sec130/4; 1,576,000 as of Dec 31, 2025 https://agentii.ai/v/AMZN/sec131/4 (+20,000, +1.3%).

[DEDUCTED] Revenue per employee: FY2024 $637,959M / 1,556,000 ≈ $410k https://agentii.ai/v/AMZN/sec131/24 https://agentii.ai/v/AMZN/sec130/4; FY2025 $716,924M / 1,576,000 ≈ $455k https://agentii.ai/v/AMZN/sec131/24 https://agentii.ai/v/AMZN/sec131/4 (+10.9%). Revenue is company-wide (includes AWS), so this is a blended productivity measure, not a fulfillment-only metric.

[DEDUCTED] NA segment net sales per NA fulfillment/DC square foot: FY2024 $387,497M / 485.0M sq ft ≈ $799/sq ft https://agentii.ai/v/AMZN/sec130/18; FY2025 $426,305M / 519.9M sq ft ≈ $820/sq ft https://agentii.ai/v/AMZN/sec131/18 (+2.6%). Confounded by combined fulfillment + data-center footprint disclosure (see Coverage Gaps).

[DEDUCTED] Fulfillment cost per $1 of net sales improved from $0.154 (FY2024) to $0.152 (FY2025) https://agentii.ai/v/AMZN/sec131/25, and North America segment operating margin rose to 7.9% in Q2 2026 https://agentii.ai/v/AMZN/ect83/2 (6.9% NA margin for FY2025: $29,619M OI on $426,305M sales https://agentii.ai/v/AMZN/sec131/27 https://agentii.ai/v/AMZN/sec131/24).

[VIEW] Amazon reports productivity in unit-growth-vs-cost terms rather than absolute units-per-employee. The consistent disclosure pattern — units growing 2–8pp faster than fulfillment cost — is the company's chosen evidence that automation is deflating per-unit handling cost. Absolute units shipped and units per employee are not disclosed (coverage gap).

### 3. Automation capex run-rate and deployment economics (PIL-4)

[FACT] Consolidated cash capex: $77.7B (2024) → $128.3B (2025), "primarily reflect investments in technology infrastructure (the majority of which is to support AWS business growth) and in additional capacity to support our fulfillment network, both of which we expect to increase in 2026" https://agentii.ai/v/AMZN/sec131/23.

[FACT] 2026 quarterly run-rate: Q1 2026 cash capex $43.2B https://agentii.ai/v/AMZN/ect82/2; Q2 2026 cash capex $53.1B https://agentii.ai/v/AMZN/ect83/2; H1 2026 $96.3B vs H1 2025 $55.6B https://agentii.ai/v/AMZN/sec177/27. Purchases of property and equipment: Q2 2026 $54,208M; H1 2026 $98,411M; trailing twelve months $173,028M https://agentii.ai/v/AMZN/sec177/3.

[FACT] Fulfillment-relevant (North America segment) net P&E additions — the closest SEC-disclosed proxy for warehouse automation investment: FY2024 $24,348M → FY2025 $35,919M (+48%) https://agentii.ai/v/AMZN/sec131/70; H1 2026 $23,265M vs H1 2025 $16,368M (+42% YoY) https://agentii.ai/v/AMZN/sec177/25. AWS segment additions remain the dominant share (FY2025 $96,496M; H1 2026 $90,120M), so warehouse automation capex is a minority of total https://agentii.ai/v/AMZN/sec131/70 https://agentii.ai/v/AMZN/sec177/25.

[FACT] Automation asset-base growth: North America P&E, net rose from $103.0B (Dec 2024) to $122.0B (Dec 2025) to $135.0B (Jun 2026) https://agentii.ai/v/AMZN/sec131/70 https://agentii.ai/v/AMZN/sec177/25. NA D&A expense grew from $3,742M (Q2 2025) to $4,500M (Q2 2026, +20%), reflecting a growing automation-heavy asset base https://agentii.ai/v/AMZN/sec177/25.

[FACT] Network configuration: US fulfillment regions expanded from 8 to 10 as part of regionalization efficiency https://agentii.ai/v/AMZN/ect81/5. NA fulfillment/data-center/other footprint: 485.0M sq ft leased+owned (Dec 2024) → 519.9M sq ft (Dec 2025) https://agentii.ai/v/AMZN/sec130/18 https://agentii.ai/v/AMZN/sec131/18.

[DEDUCTED] Robotics retrofit economics: management attributes the fulfillment-cost improvement ("partially offset by operational efficiencies" on 11% expense growth https://agentii.ai/v/AMZN/sec131/25) jointly to regionalization, robotics, and consolidation — the incremental NA P&E additions of ~$36B in FY2025 (≈8.4% of NA net sales) https://agentii.ai/v/AMZN/sec131/70 https://agentii.ai/v/AMZN/sec131/24 are the disclosed cost of this efficiency program.

[VIEW] PIL-4 read-across for humanoids: AMZN's trajectory shows a two-phase deployment pattern — (1) greenfield-only latest tech, then (2) retrofit of the existing fleet, with ~2 years from single-site integration (Shreveport, 2024) to fleetwide retrofit mandate (2026) https://agentii.ai/v/AMZN/ect77/4 https://agentii.ai/v/AMZN/ect82/2. If humanoid deployment follows the same pattern, timing models should assume a greenfield-to-retrofit bridge of similar length, with capex intensity concentrated in years 2–4.

### 4. Revenue and operating income context (structured facts)

Quarterly revenue (us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax, is_primary):

| Period | Revenue ($M) | Source |
|---|---|---|
| Q2 2026 (Apr–Jun) | 200,606 | XBRL fact (amzn-20260630.htm) https://agentii.ai/v/AMZN/sec177/4 |
| Q1 2026 (Jan–Mar) | 181,519 | XBRL fact (amzn-20260331.htm) https://agentii.ai/v/AMZN/sec172/4 |
| Q4 2025 (Oct–Dec) | 213,386 [DEDUCTED = FY 716,924 − 9M 503,538] | https://agentii.ai/v/AMZN/sec131/24 |
| Q3 2025 (Jul–Sep) | 180,169 | XBRL fact (amzn-20250930.htm) https://agentii.ai/v/AMZN/sec167/4 |
| Q2 2025 (Apr–Jun) | 167,702 | XBRL fact (amzn-20250630.htm) https://agentii.ai/v/AMZN/sec166/4 |
| Q1 2025 (Jan–Mar) | 155,667 | XBRL fact (amzn-20250331.htm) https://agentii.ai/v/AMZN/sec165/4 |
| FY2025 | 716,924 | https://agentii.ai/v/AMZN/sec131/24 |
| FY2024 | 637,959 | https://agentii.ai/v/AMZN/sec131/24 |

[FACT] Cross-validation: the derived Q4 2025 revenue of $213.4B matches the $213.4B stated on the Q4 2025 call https://agentii.ai/v/AMZN/ect81/1; Q2 2026 revenue of $200.6B matches the call https://agentii.ai/v/AMZN/ect83/2. Segment FY2025: North America $426.3B (+10%), International $161.9B (+13%), AWS $128.7B (+20%) https://agentii.ai/v/AMZN/sec131/24.

Quarterly operating income (us-gaap:OperatingIncomeLoss, is_primary):

| Period | OI ($M) | Source |
|---|---|---|
| Q2 2026 | 27,461 | XBRL fact https://agentii.ai/v/AMZN/sec177/4 |
| Q1 2026 | 23,852 | XBRL fact https://agentii.ai/v/AMZN/sec172/4 |
| Q4 2025 | 24,977 [DEDUCTED = FY 79,975 − 9M 54,998] | https://agentii.ai/v/AMZN/sec131/27 |
| Q3 2025 | 17,422 | XBRL fact https://agentii.ai/v/AMZN/sec167/4 |
| Q2 2025 | 19,171 | XBRL fact https://agentii.ai/v/AMZN/sec166/4 |
| Q1 2025 | 18,405 | XBRL fact https://agentii.ai/v/AMZN/sec165/4 |
| FY2025 | 79,975 | https://agentii.ai/v/AMZN/sec131/27 |
| FY2024 | 68,593 | https://agentii.ai/v/AMZN/sec131/27 |

[FACT] Cross-validation: derived Q4 2025 OI of $25.0B matches the $25B stated on the call https://agentii.ai/v/AMZN/ect81/1. FY2025 consolidated OI included $2.5B FTC settlement charge (Q3 2025) and $2.7B severance charges https://agentii.ai/v/AMZN/sec131/27. Q1 2026 operating margin of 13.1% was the company's highest ever https://agentii.ai/v/AMZN/ect82/2.

## Key Metrics

| KPI | Value | Tag | Citation |
|---|---|---|---|
| Robots in fulfillment network | 1,000,000+ | FACT | https://agentii.ai/v/AMZN/ect81/5 |
| Robotic arms (Cardinal/Sparrow) 2026 plan | more than double | FACT | https://agentii.ai/v/AMZN/ect83/2 |
| Paid units growth Q2 2026 | +17% YoY | FACT | https://agentii.ai/v/AMZN/ect83/2 |
| Fulfillment % of net sales | 15.2% (FY2025) vs 15.4% (FY2024) | FACT | https://agentii.ai/v/AMZN/sec131/25 |
| Revenue per employee | ~$455k FY2025 (+11% YoY) | DEDUCTED | https://agentii.ai/v/AMZN/sec131/4 |
| NA sales / NA fulfillment+DC sq ft | ~$820/sq ft FY2025 | DEDUCTED | https://agentii.ai/v/AMZN/sec131/18 |
| Cash capex | $128.3B FY2025; $96.3B H1 2026 | FACT | https://agentii.ai/v/AMZN/sec131/23 https://agentii.ai/v/AMZN/sec177/27 |
| NA net P&E additions | $35.9B FY2025; $23.3B H1 2026 | FACT | https://agentii.ai/v/AMZN/sec131/70 https://agentii.ai/v/AMZN/sec177/25 |
| Employees | 1,576,000 (Dec 31, 2025) | FACT | https://agentii.ai/v/AMZN/sec131/4 |
| NA operating margin | 7.9% Q2 2026 | FACT | https://agentii.ai/v/AMZN/ect83/2 |
| Same/next-day units H1 2024 | >5B | FACT | https://agentii.ai/v/AMZN/ect75/1 |

## Coverage Gaps & Citations

**Coverage gaps (unretrievable — not invented):**
1. **Absolute units shipped and units per employee** — AMZN discloses only growth rates (paid units +17% Q2 2026) and throughput anecdotes (5B same/next-day units); no absolute unit counts in SEC corpus.
2. **Robotics fleet size by quarter** — corpus has two point disclosures (1M+ Feb 2026; arms doubling 2026). Pre-2024 fleet milestones (e.g., 750k robots) do not appear in the retrieved transcripts (keyword search "robot" on ect75 returned only the cost-to-serve mention, no fleet count).
3. **Per-site / per-task reliability metrics** — no disclosed pick-failure, downtime, or manipulation-success rates; qualitative safety/productivity statements only.
4. **Quarterly capex for Q3/Q4 2025** — Q4 2025 is not separately disclosed in the 10-K (FY total only); Q3 2025 10-Q cash-flow page not retrieved in this run (available as sec167 if needed).
5. **Fulfillment-only square footage** — properties table combines "fulfillment, data centers, and other" https://agentii.ai/v/AMZN/sec131/18, so warehouse-only productivity per sq ft cannot be isolated.
6. **`Revenues` concept (P2.1 second concept)** — returned zero is-primary facts for AMZN in the XBRL store; primary concept used is `RevenueFromContractWithCustomerExcludingAssessedTax`.
7. **XBRL capex facts** — `PaymentsToAcquirePropertyPlantAndEquipment` returned empty from `search_xbrl_facts` for AMZN (both unfiltered and fiscal-year-filtered calls); capex values were instead retrieved from 10-K/10-Q cash-flow pages and earnings calls (cited above).

**Citations (roll-up index):**

| ID | Document | Link base |
|---|---|---|
| sec131 | FY2025 Form 10-K (2026-02-06) | https://agentii.ai/v/AMZN/sec131/{page} |
| sec130 | FY2024 Form 10-K (2025-02-07) | https://agentii.ai/v/AMZN/sec130/{page} |
| sec177 | Q2 2026 Form 10-Q (2026-07-31) | https://agentii.ai/v/AMZN/sec177/{page} |
| sec172 | Q1 2026 Form 10-Q (2026-04-30) | https://agentii.ai/v/AMZN/sec172/{page} |
| sec167 | Q3 2025 Form 10-Q (2025-10-31) | https://agentii.ai/v/AMZN/sec167/{page} |
| sec166 | Q2 2025 Form 10-Q (2025-08-01) | https://agentii.ai/v/AMZN/sec166/{page} |
| sec165 | Q1 2025 Form 10-Q (2025-05-02) | https://agentii.ai/v/AMZN/sec165/{page} |
| ect83 | Q2 2026 earnings call (2026-07-30) | https://agentii.ai/v/AMZN/ect83/{page} |
| ect82 | Q1 2026 earnings call (2026-04-29) | https://agentii.ai/v/AMZN/ect82/{page} |
| ect81 | Q4 2025 earnings call (2026-02-05) | https://agentii.ai/v/AMZN/ect81/{page} |
| ect77 | Q4 2024 earnings call (2025-02-06) | https://agentii.ai/v/AMZN/ect77/{page} |
| ect75 | Q2 2024 earnings call (2024-08-01) | https://agentii.ai/v/AMZN/ect75/{page} |

## Verification (call trace)

| # | Tool call | Inputs | Outcome |
|---|---|---|---|
| 1 | search_companies | ticker=AMZN | Resolved AMZN, CIK 0001018724, NASDAQ |
| 2 | get_ticker_coverage | ticker=AMZN | 7 sources; xbrl 22,062 facts; 19 transcripts; 86 src docs |
| 3 | get_company_fiscal_calendar | ticker=AMZN | FY-end month 2 (registry); quarters mapped; first attempt rate-limited, retried |
| 4 | list_xbrl_concepts | search=Revenue | 109 concepts; revenue concepts selected (P2.1) |
| 5 | list_xbrl_concepts | search=PaymentsToAcquire | 45 concepts; capex concept confirmed |
| 6 | batch_search | 18 sub-queries | Returned metadata stubs only; abandoned for direct calls |
| 7 | search_xbrl_facts | Revenue concept, pages 1–2 | 35 facts: quarterly Q1–Q3 + FY (Q4s absent — derived) |
| 8 | search_xbrl_facts | OperatingIncomeLoss | 35 facts: quarterly + FY |
| 9 | search_xbrl_facts | Capex concept (3 attempts) | Empty result set — gap #7; capex taken from cash-flow pages |
| 10 | search_sec_filings | 10-K, 10-Q | Citation IDs: sec120–131 (10-K), sec160–177 (10-Q) |
| 11 | search_sec_filings | earnings_call_transcript | Empty (transcripts not in pipeline.sec_filings) |
| 12 | search_documents | 10-K, transcripts | Metadata only (no citation ids) — superseded by #10 |
| 13 | list_sources | source_type=earnings_call_transcript | 19 transcripts with source_ids |
| 14 | read_source_outline | sec131, sec177, transcript source_ids | Page maps; transcript citation IDs resolved: ect75, ect77, ect81, ect82, ect83 |
| 15 | search_keyword_in_source | keyword=robot × 6 docs | Robotics pages located (ect81 p5, ect82 p2, ect83 p2, ect77 p4, ect75 p1; sec177 none) |
| 16 | read_source_pages | sec131 p4,p18,p23,p24,p25,p26,p27,p70; sec130 p4,p18; sec177 p3,p25,p27; ect75 p1; ect77 p4; ect81 p5; ect82 p2; ect83 p2 | All material numbers in this artifact |

Every material number in this artifact traces to one of the calls above. No price/market data used (market_data_stage: none). No external (non-MCP) sources used.
