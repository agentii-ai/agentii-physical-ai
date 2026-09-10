---
artifact_id: "001-AMZN-supply-chain-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: AMZN
skill: supply-chain
mode: default
affix: supply-chain-map
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "8cb3ac1de486"
as_of: 2026-09-10
entity_claims: []
citations:
  - "https://agentii.ai/v/AMZN/sec131/23"
  - "https://agentii.ai/v/AMZN/sec131/25"
  - "https://agentii.ai/v/AMZN/sec131/59"
  - "https://agentii.ai/v/AMZN/sec131/60"
  - "https://agentii.ai/v/AMZN/sec131/69"
  - "https://agentii.ai/v/AMZN/sec131/70"
  - "https://agentii.ai/v/AMZN/sec177/25"
  - "https://agentii.ai/v/AMZN/sec177/27"
  - "https://agentii.ai/v/AMZN/sec177/31"
  - "https://agentii.ai/v/AMZN/ect81/5"
  - "https://agentii.ai/v/AMZN/ect83/2"
pillars_addressed: [PIL-1, PIL-2, PIL-4]
claim_state: pinned
key_metrics:
  robots_deployed_fleet: ">1,000,000 robots in fulfillment network (Feb 2026)"
  robotic_arm_fleet_2026_guidance: ">2x fleet of robotic arms (Cardinal, Sparrow) expected in 2026"
  cash_capex_fy2024: 77700000000
  cash_capex_fy2025: 128300000000
  cash_capex_h1_2026: 96300000000
  cash_capex_q2_2026: 53100000000
  pe_net_additions_fy2025_consolidated: 142352000000
  pe_net_additions_fy2025_aws: 96496000000
  pe_net_additions_fy2025_north_america: 35919000000
  pe_net_additions_h1_2026_consolidated: 118648000000
  pe_net_additions_h1_2026_aws: 90120000000
  pe_net_additions_h1_2026_north_america: 23265000000
  fulfillment_expense_fy2025: 109074000000
  fulfillment_pct_net_sales_fy2025: 15.2
  shipping_costs_fy2025: 102700000000
  revenue_fy2025: 716924000000
  revenue_fy2024: 637959000000
  revenue_q2_2026: 200606000000
  aws_revenue_fy2025: 128725000000
  us_revenue_fy2025: 489657000000
  unconditional_purchase_obligations: 84772000000
  total_commitments: 439661000000
  vendor_concentration_max: "no vendor >= 10% of purchases (2025)"
  fulfillment_regions: 10
  operating_cash_flow_ttm_jun2026: 161403000000
conclusions:
  - "AMZN operates the largest disclosed fleet-scale warehouse robotics deployment (>1M robots; robotic-arm fleet doubling guided for 2026) — supports PIL-1 deployment machinery and PIL-4 timing at warehouse-automation level, NOT embodied AI (plan risk note applies)."
  - "Deployment economics are visible in filings: $128.3B FY2025 cash capex including fulfillment-network capacity; but AWS infrastructure dominates (AWS = $90.1B of $118.6B H1-2026 net P&E additions), so headline AMZN capex is no longer a clean automation-spend proxy."
  - "Robotics is framed as a cost-to-serve lever inside a $109.1B fulfillment cost base; fulfillment intensity fell from 15.4% to 15.2% of net sales in FY2025 even as network investment rose."
  - "Supply chain structurally opaque at component level: no vendor >=10% of purchases; no robotics supplier names disclosed; vertical integration implied (internal Amazon Robotics development). PIL-2 actuator/motion component chain is not retrievable from AMZN SEC disclosures."
  - "Disclosure asymmetry: the word 'robot' appears zero times in the FY2025 10-K; fleet metrics surface only on earnings calls — retrieval must triangulate transcripts with filings."
facts_count: 24
deducted_count: 7
views_count: 4
citation_count: 11
---

# AMZN Supply-Chain Map — Warehouse Robotics Deployment Machinery

## Executive Summary

Amazon is the largest disclosed deployer of warehouse robotics at fleet scale. Management stated "over a million robots" in the fulfillment network on the Q4 2025 call https://agentii.ai/v/AMZN/ect81/5 and guided to more than doubling its fleet of robotic arms (Cardinal, Sparrow) in 2026 https://agentii.ai/v/AMZN/ect83/2. The deployment machinery is visible in financials: cash capex reached $128.3B in 2025 (from $77.7B) https://agentii.ai/v/AMZN/sec131/23 and $96.3B in H1 2026 https://agentii.ai/v/AMZN/sec177/27 — but AWS infrastructure absorbed ~$90B of the $118.6B H1-2026 net P&E additions, versus ~$23B for the North America (fulfillment-heavy) segment https://agentii.ai/v/AMZN/sec177/25. Robotics is framed as a cost-to-serve lever inside a $109.1B fulfillment cost base https://agentii.ai/v/AMZN/sec131/25. Supply chain: no vendor accounted for ≥10% of purchases https://agentii.ai/v/AMZN/sec131/60; robotics appears vertically integrated with no component-supplier disclosure. **PLAN RISK NOTE:** AMZN evidence bears on warehouse deployment economics and pace, not embodied-AI/humanoid scale — treat as a deployment-machinery analogue only.

## Data Sources

| Source | citation_id | Type | Date | Pages retrieved |
|---|---|---|---|---|
| AMZN 10-K (FY ended 2025-12-31) | sec131 | 10-K | 2026-02-06 | 23, 25, 59, 60, 69, 70 |
| AMZN 10-Q (Q ended 2026-06-30) | sec177 | 10-Q | 2026-07-31 | 25, 27, 31 |
| AMZN Q4 2025 earnings call | ect81 | transcript | 2026-02-05 | 5 |
| AMZN Q2 2026 earnings call | ect83 | transcript | 2026-07-30 | 2 |
| XBRL facts store | — | structured | — | RevenueFromContractWithCustomerExcludingAssessedTax (standard + detailed views) |
| Keyword filter | — | Layer 2.5 | — | "robot" in sec131 → 0 hits |

Protocol: preflight (search_companies, get_ticker_coverage, get_company_fiscal_calendar) → Layer 1 (search_documents, list_sources) → Layer 2 (read_source_outline ×4) → Layer 2.5 (search_keyword_in_source) → Layer 3 (read_source_pages ×6). Structured numbers via search_xbrl_facts after list_xbrl_concepts.

## Analysis

### 1. Fleet scale and deployment pace (PIL-1 data-bound, PIL-4 timing)

[FACT] CEO Andrew Jassy stated on the Q4 2025 earnings call: "we have over a million robots today in our fulfillment network" https://agentii.ai/v/AMZN/ect81/5. He added that robots handle "all sorts of functions, but still a fraction of what I think we are going to be able to enable over time," and that assigning "the robotics things that are more repetitive" yields "better productivity for the business, more safe for teammates and there's real cost efficiencies in that as well" https://agentii.ai/v/AMZN/ect81/5.

[FACT] On the Q2 2026 call, CFO Brian Olsavsky gave a concrete deployment target: "We're retrofitting our facilities with our latest generation technology, and we expect to more than double our fleet of robotic arms, like Cardinal and Sparrow, in 2026" https://agentii.ai/v/AMZN/ect83/2.

[FACT] The word "robot" appears zero times in the FY2025 10-K (79 pages; keyword scan returned 0 matches) — the fleet-scale disclosures live on earnings calls, not in the annual report.

[FACT] Regionalization of the fulfillment network is a parallel physical-reconfiguration program: Jassy noted the U.S. network was regionalized from "eight" to "now 10" regions https://agentii.ai/v/AMZN/ect81/5.

[DEDUCTED] The "more than double in 2026" guidance implies a >100% one-year growth rate for the articulated-arm component of the fleet — a retrofit cycle across the installed fulfillment base rather than greenfield-only deployment.

[DEDUCTED] A >1M-unit robot fleet each generating task-level perception/manipulation data supports PIL-1's data-bound argument at warehouse scale; AMZN is the largest publicly disclosed generator of industrial embodied-robot operational data.

### 2. Automation capex and fulfillment-network investment (deployment machinery)

[FACT] Cash capital expenditures were $77.7B in 2024 and $128.3B in 2025, which "primarily reflect investments in technology infrastructure (the majority of which is to support AWS business growth) and in additional capacity to support our fulfillment network, both of which we expect to increase in 2026" https://agentii.ai/v/AMZN/sec131/23.

[FACT] H1 2026 cash capex was $96.3B versus $55.6B in H1 2025; Q2 2026 alone was $53.1B https://agentii.ai/v/AMZN/sec177/27. On the Q2 call, Olsavsky said cash capex of $53.1B "primarily relates to AWS and generative AI" https://agentii.ai/v/AMZN/ect83/2.

[FACT] Segment-level net additions to property and equipment: FY2025 North America $35.9B, International $7.6B, AWS $96.5B, consolidated $142.4B (FY2024: $85.8B; FY2023: $48.3B) https://agentii.ai/v/AMZN/sec131/70. H1 2026: North America $23.3B, AWS $90.1B, consolidated $118.6B https://agentii.ai/v/AMZN/sec177/25. AWS P&E net reached $263.8B at June 30, 2026 versus North America's $135.0B https://agentii.ai/v/AMZN/sec177/25.

[DEDUCTED] AWS data-center capex now dwarfs fulfillment-network capex ~3.9:1 on net additions (H1 2026: $90.1B vs $23.3B) https://agentii.ai/v/AMZN/sec177/25. The warehouse-robotics capex pool is the North America fulfillment slice, not the headline $128.3B.

[DEDUCTED] H1 2026 capex of $96.3B implies a >$190B annualized run-rate — roughly 1.5x the FY2025 level — confirming the "expect to increase in 2026" language https://agentii.ai/v/AMZN/sec131/23.

[FACT] Operating cash flow (TTM) reached $161.4B at June 30, 2026, funding the capex wave internally https://agentii.ai/v/AMZN/sec177/27.

### 3. Fulfillment cost structure — where robotics pays back

[FACT] FY2025 operating expenses: Fulfillment $109.1B (+11% YoY, 15.2% of net sales vs 15.4% in 2024); Technology and infrastructure $108.5B (+23%); shipping costs $102.7B (up from $95.8B) https://agentii.ai/v/AMZN/sec131/25. "Shipping costs to receive products from our suppliers are included in our inventory and recognized as cost of sales upon sale" https://agentii.ai/v/AMZN/sec131/25.

[FACT] The Q2 2026 increase in fulfillment costs was driven by "increased sales and investments in our fulfillment network, partially offset by operational efficiencies" https://agentii.ai/v/AMZN/sec177/31.

[FACT] Technology and infrastructure expense explicitly includes "autonomous vehicles for ride-hailing services" (Zoox) and the Kuiper satellite network alongside AWS — non-warehouse physical-AI programs carried in the same cost line https://agentii.ai/v/AMZN/sec177/31.

[DEDUCTED] Fulfillment intensity declined (15.4% → 15.2% of net sales FY2025) while network investment rose https://agentii.ai/v/AMZN/sec131/25 — consistent with robotics/regionalization efficiency offsetting investment; the company itself attributes Q2 cost mitigation to "optimizing inventory placement, shortening shipping distances, reducing touches per package, and improving consolidation rates" https://agentii.ai/v/AMZN/ect83/2.

### 4. Supply-chain structure and supplier dependencies (PIL-2)

[FACT] "During 2025, no vendor accounted for 10% or more of our purchases. We generally do not have long-term contracts or arrangements with our vendors to guarantee the availability of merchandise, particular payment terms, or the extension of credit limits" https://agentii.ai/v/AMZN/sec131/60.

[FACT] Principal contractual commitments as of December 31, 2025 totaled $439.7B, including $84.8B of unconditional purchase obligations covering "long-term agreements to acquire and license digital media content, procure energy, acquire property and equipment, and license software" https://agentii.ai/v/AMZN/sec131/59. Financing obligations for "fulfillment network and data center facilities" carry a weighted-average remaining term of 15.0 years https://agentii.ai/v/AMZN/sec131/59.

[FACT] Geographic concentration of the physical network: U.S. property and equipment net + operating leases were $321.9B at end-2025 versus $121.2B non-U.S.; no single non-U.S. country ≥10% https://agentii.ai/v/AMZN/sec131/70.

[FACT] FY2025 revenue geography: United States $489.7B, Germany $45.9B, United Kingdom $43.2B, Japan $30.7B, rest of world $107.5B https://agentii.ai/v/AMZN/sec131/69. AWS revenue was $128.7B (+20%) within consolidated net sales of $716.9B (+12%) https://agentii.ai/v/AMZN/sec131/69.

[FACT] Import structure shifts tariff exposure to vendors: Amazon is "not the importer of record for the large majority of items sold in our store, given suppliers typically handle imports and pay relevant tariffs" https://agentii.ai/v/AMZN/ect83/2.

[DEDUCTED] For the robotics fleet itself, no supplier names appear anywhere in the retrieved filings; Cardinal and Sparrow are Amazon-developed systems, implying vertical integration of the actuation chain through Amazon Robotics. PIL-2's actuator/motion component chain is therefore not observable from AMZN SEC disclosures — a structural blind spot of public filings.

[DEDUCTED] Energy has become a disclosed structural supply input — purchase obligations include "procure energy," and Q2 2026 results were affected by derivative-accounted energy contracts "to secure electricity supply for existing and future operations" https://agentii.ai/v/AMZN/ect83/2 — supply-chain expansion driven by the data-center buildout rather than robotics.

### 5. Disclosure asymmetry and evidence interpretation

[VIEW] Fleet-scale robotics metrics (>1M robots; arm-fleet doubling) are disclosed only on earnings calls, while the 10-K contains zero "robot" mentions — robotics is treated as a strategy/cost narrative rather than a regulated disclosure line, so supply-chain analysis must triangulate transcripts against filings.

[VIEW] With AWS absorbing ~76% of H1-2026 net P&E additions https://agentii.ai/v/AMZN/sec177/25, AMZN's headline capex is no longer a valid proxy for fulfillment-automation investment; the North America segment line item is the better (if coarse) proxy for robotics deployment spend.

[VIEW] AMZN is the strongest public proxy for fleet-scale robotics deployment economics (capex absorption, cost-to-serve payback, retrofit cadence) — but per the plan risk note, its evidence does not speak to embodied-AI/humanoid-specific supply chains and must not be read as such.

[VIEW] The combination of regionalization (8→10 regions) plus robotics retrofitting suggests logistics-labor displacement will proceed via facility-level physical reconfiguration — a deployment pattern relevant to PIL-4 timing for warehouse automation broadly.

## Key Metrics

| Metric | Value | Period | Citation |
|---|---|---|---|
| Robotics fleet size | >1,000,000 robots | Feb 2026 (Q4 2025 call) | https://agentii.ai/v/AMZN/ect81/5 |
| Robotic-arm fleet guidance | >2x in 2026 (Cardinal, Sparrow) | guidance | https://agentii.ai/v/AMZN/ect83/2 |
| Cash capex | $77.7B → $128.3B | FY2024 → FY2025 | https://agentii.ai/v/AMZN/sec131/23 |
| Cash capex | $96.3B ($53.1B in Q2) | H1 2026 | https://agentii.ai/v/AMZN/sec177/27 |
| P&E net additions, consolidated | $48.3B / $85.8B / $142.4B | FY2023/24/25 | https://agentii.ai/v/AMZN/sec131/70 |
| P&E net additions, AWS | $24.8B / $53.3B / $96.5B | FY2023/24/25 | https://agentii.ai/v/AMZN/sec131/70 |
| P&E net additions, North America | $17.5B / $24.3B / $35.9B | FY2023/24/25 | https://agentii.ai/v/AMZN/sec131/70 |
| P&E net additions H1 2026 | AWS $90.1B; NA $23.3B; consol $118.6B | H1 2026 | https://agentii.ai/v/AMZN/sec177/25 |
| Fulfillment expense | $109.1B (15.2% of net sales; 15.4% in 2024) | FY2025 | https://agentii.ai/v/AMZN/sec131/25 |
| Technology & infrastructure expense | $108.5B (+23%) | FY2025 | https://agentii.ai/v/AMZN/sec131/25 |
| Shipping costs | $102.7B | FY2025 | https://agentii.ai/v/AMZN/sec131/25 |
| Consolidated net sales | $716.9B (+12%) | FY2025 | https://agentii.ai/v/AMZN/sec131/69 |
| AWS net sales | $128.7B (+20%) | FY2025 | https://agentii.ai/v/AMZN/sec131/69 |
| U.S. revenue share | $489.7B of $716.9B (68.3%) | FY2025 | https://agentii.ai/v/AMZN/sec131/69 |
| Vendor concentration | none ≥10% of purchases | FY2025 | https://agentii.ai/v/AMZN/sec131/60 |
| Unconditional purchase obligations | $84.8B (total commitments $439.7B) | 2025-12-31 | https://agentii.ai/v/AMZN/sec131/59 |
| U.S. vs non-U.S. P&E net + operating leases | $321.9B vs $121.2B | 2025-12-31 | https://agentii.ai/v/AMZN/sec131/70 |
| Fulfillment network regions (U.S.) | 10 (from 8) | Feb 2026 | https://agentii.ai/v/AMZN/ect81/5 |
| Operating cash flow (TTM) | $161.4B | Jun 2026 | https://agentii.ai/v/AMZN/sec177/27 |

## Coverage Gaps & Citations

**Coverage gaps**

1. **No robotics fleet-size disclosure in SEC filings.** Keyword scan of the FY2025 10-K (sec131) returned zero "robot" hits; fleet metrics (>1M robots, arm-fleet doubling) exist only in earnings-call transcripts (ect81, ect83). No drive-unit counts, units-per-facility, or deployment-by-region disclosures exist in any retrieved document.
2. **No robotics supplier disclosure (PIL-2 gap).** Cardinal/Sparrow/Amazon Robotics component chain — actuators, servos, sensing, controllers — is not named in any retrieved filing. The supplier statement ("no vendor ≥10%") covers merchandise vendors only https://agentii.ai/v/AMZN/sec131/60.
3. **Fiscal-calendar mismatch in gold registry.** get_company_fiscal_calendar returns fiscal_year_end_month=2 (February) for AMZN, but the 10-K itself is for the "fiscal year ended December 31, 2025" https://agentii.ai/v/AMZN/sec131/23. Consequently, XBRL queries filtered by fiscal_year (2025/2026) returned empty for capex concepts; calendar-dated facts were used instead.
4. **Structured capex unavailable in XBRL store.** us-gaap:PaymentsToAcquirePropertyPlantAndEquipment and us-gaap:Revenues return no AMZN facts (AMZN custom taxonomy, `amzn` namespace, not loaded in store). Cash capex figures were taken from filing page text (sec131/23, sec177/27) instead of XBRL.
5. **search_sec_filings was rate-limited** on first attempt; recovered via search_documents + list_sources (no data lost).
6. **No humanoid/embodied-AI relevance:** AMZN's robotics evidence covers warehouse automation only (plan risk note); any embodied-AI-specific supply-chain question is unanswerable from this corpus.

**Citation index (roll-up)**

1. https://agentii.ai/v/AMZN/sec131/23 — cash capex $77.7B/$128.3B; expected increase 2026
2. https://agentii.ai/v/AMZN/sec131/25 — fulfillment $109.1B; T&I $108.5B; shipping $102.7B
3. https://agentii.ai/v/AMZN/sec131/59 — commitments $439.7B; purchase obligations $84.8B; fulfillment/data-center financing obligations
4. https://agentii.ai/v/AMZN/sec131/60 — suppliers: no vendor ≥10%; no long-term vendor contracts
5. https://agentii.ai/v/AMZN/sec131/69 — revenue disaggregation FY2023-25 by product group and geography
6. https://agentii.ai/v/AMZN/sec131/70 — segment P&E net additions FY2023-25; U.S./non-U.S. split
7. https://agentii.ai/v/AMZN/sec177/25 — segment P&E net additions H1 2026; AWS $263.8B P&E net
8. https://agentii.ai/v/AMZN/sec177/27 — H1 2026 cash capex $96.3B; OCF TTM $161.4B
9. https://agentii.ai/v/AMZN/sec177/31 — fulfillment cost drivers; Zoox/Kuiper in T&I line
10. https://agentii.ai/v/AMZN/ect81/5 — >1M robots; 8→10 regions; robotics efficiency framing
11. https://agentii.ai/v/AMZN/ect83/2 — robotic-arm fleet >2x in 2026; Q2 capex $53.1B; importer-of-record tariff structure

## Verification

| # | Material number/claim | Retrieval call | /v/ citation |
|---|---|---|---|
| 1 | >1,000,000 robots in fulfillment network | read_source_pages(ect81, page5) | https://agentii.ai/v/AMZN/ect81/5 |
| 2 | Robotic-arm fleet (Cardinal, Sparrow) to more than double in 2026 | read_source_pages(ect83, page2) | https://agentii.ai/v/AMZN/ect83/2 |
| 3 | Cash capex $77.7B (2024), $128.3B (2025); expect increase 2026 | read_source_pages(sec131, page23) | https://agentii.ai/v/AMZN/sec131/23 |
| 4 | Cash capex H1 2026 $96.3B; Q2 2026 $53.1B | read_source_pages(sec177, page27) | https://agentii.ai/v/AMZN/sec177/27 |
| 5 | Q2 2026 cash capex $53.1B "primarily relates to AWS and generative AI" | read_source_pages(ect83, page2) | https://agentii.ai/v/AMZN/ect83/2 |
| 6 | Segment P&E net additions FY2023-25 (NA $35.9B / AWS $96.5B FY25) | read_source_pages(sec131, page70) | https://agentii.ai/v/AMZN/sec131/70 |
| 7 | Segment P&E net additions H1 2026 (NA $23.3B / AWS $90.1B) | read_source_pages(sec177, page25) | https://agentii.ai/v/AMZN/sec177/25 |
| 8 | Fulfillment $109.1B (15.2% of net sales); T&I $108.5B; shipping $102.7B | read_source_pages(sec131, page25) | https://agentii.ai/v/AMZN/sec131/25 |
| 9 | Fulfillment cost rise = sales + network investment, offset by efficiencies | read_source_pages(sec177, page31) | https://agentii.ai/v/AMZN/sec177/31 |
| 10 | No vendor ≥10% of purchases; no long-term vendor contracts | read_source_pages(sec131, page60) | https://agentii.ai/v/AMZN/sec131/60 |
| 11 | Total commitments $439.7B; unconditional purchase obligations $84.8B | read_source_pages(sec131, page59) | https://agentii.ai/v/AMZN/sec131/59 |
| 12 | Revenue FY2025 $716.9B; AWS $128.7B; US $489.7B; DE/UK/JP | read_source_pages(sec131, page69) | https://agentii.ai/v/AMZN/sec131/69 |
| 13 | Revenue FY2025 $716.9B / FY2024 $638.0B / Q2 2026 $200.6B (XBRL) | search_xbrl_facts(RevenueFromContractWithCustomerExcludingAssessedTax) | https://agentii.ai/v/AMZN/sec131/69 |
| 14 | "robot" = 0 hits in FY2025 10-K | search_keyword_in_source(sec131, "robot") | — (negative result) |
| 15 | U.S. P&E net + op leases $321.9B vs non-U.S. $121.2B | read_source_pages(sec131, page70) | https://agentii.ai/v/AMZN/sec131/70 |
| 16 | Not importer of record for large majority of items; suppliers handle imports | read_source_pages(ect83, page2) | https://agentii.ai/v/AMZN/ect83/2 |
| 17 | 8→10 U.S. fulfillment regions | read_source_pages(ect81, page5) | https://agentii.ai/v/AMZN/ect81/5 |
| 18 | OCF TTM $161.4B (Jun 2026) | read_source_pages(sec177, page27) | https://agentii.ai/v/AMZN/sec177/27 |

All material numbers above trace to agentii MCP retrieval calls made during this run (29 calls, 11 distinct tools). No market/price data used (market_data_stage: none). No number was sourced from memory or external web.
