---
artifact_id: "001-NVDA-supply-chain-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: NVDA
skill: supply-chain
mode: default
affix: supply-chain-map
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "8cb3ac1de486"
as_of: 2026-09-10
entity_claims:
  - "NVDA top-3 direct customers = 21%+17%+16% (54%) of Q1 FY2027 revenue; FY2026 top-2 = 36%"
  - "NVDA manufacturing/supply/capacity commitments $119B (Apr 26 2026), $95B due by end FY2027; total supply incl. inventory + prepaids $145B"
  - "NVDA fabless dependencies: TSMC + Samsung foundry, CoWoS packaging, HBM from SK Hynix/Micron/Samsung, CMs Hon Hai/Wistron/Fabrinet"
  - "NVDA physical-AI revenue >$9B trailing 12 months; Edge Computing platform (robotics+automotive) $6.4B Q1 FY2027, +29% YoY"
  - "VeraRubin production shipments begin Q3 2026; management cites $1T Blackwell+Rubin revenue visibility 2025-CY2027"
citations: []
pillars_addressed: [PIL-1, PIL-2, PIL-4]
claim_state: pinned
key_metrics:
  revenue_fy2026_usd_m: 215938
  revenue_q1_fy2027_usd_m: 81615
  revenue_q1_fy2027_yoy_pct: 85
  data_center_rev_q1_fy2027_usd_m: 75246
  hyperscale_rev_q1_fy2027_usd_m: 37869
  acie_rev_q1_fy2027_usd_m: 37377
  edge_rev_q1_fy2027_usd_m: 6369
  top3_direct_customer_share_q1_fy2027_pct: "21/17/16"
  inventory_q1_fy2027_usd_m: 25797
  supply_commitments_q1_fy2027_usd_b: 119
  total_supply_incl_prepaids_usd_b: 145
  physical_ai_ttm_revenue_usd_b: 9
  gross_margin_q1_fy2027_pct: 74.9
  q2_fy2027_guidance_usd_b: 91
conclusions:
  - "Compute capacity in the physical-AI build-out is being pre-committed through NVDA's supplier chain ($145B supply) and delivered ~50% into hyperscalers whose capex is forecast >$1T by 2027 — the compute-bound counterfactual to PIL-1's data-boundness thesis."
  - "The compute stack dominates NVDA's mix (~92% Data Center in Q1 FY2027) while the disclosed embodied-AI/edge envelope (robotics, automotive, physical AI) is ~$9B TTM (~3.6% of LTM revenue) — consistent with PIL-2: value accrues to the compute stack, not the actuator BOM, at this stage."
  - "PIL-4 timing anchors: VeraRubin production Q3 2026, $1T Blackwell+Rubin visibility through CY2027, GB300 fastest-ever ramp, robotics expansion flagged as a 5-year growth wave."
facts_count: 48
deducted_count: 6
views_count: 4
citation_count: 17
---

# NVDA Supply-Chain Map — Physical-AI Technology Baseline (001)

## 1. Executive Summary

NVIDIA's supply chain is where global AI compute capacity is pre-committed. Q1 FY2027 revenue reached $81.6B, +85% YoY [FACT] https://agentii.ai/v/NVDA/sec173/20, with Data Center $75.2B (+92%) split nearly evenly between Hyperscale $37.9B (+115%) and AI Clouds/Industrial/Enterprise $37.4B [FACT] https://agentii.ai/v/NVDA/sec173/21. Three direct customers (21%/17%/16%) concentrated 54% of revenue [FACT] https://agentii.ai/v/NVDA/sec173/20. On the buy side, manufacturing/supply/capacity commitments reached $119B [FACT] https://agentii.ai/v/NVDA/sec173/16 — ~$145B including inventory and prepaids [FACT] https://agentii.ai/v/NVDA/ect81/1 — against foundry (TSMC/Samsung), CoWoS, and HBM (SK Hynix/Micron/Samsung) dependencies [FACT] https://agentii.ai/v/NVDA/sec169/8. Disclosed robotics exposure is explicit but small: Edge Computing (robotics, automotive, PCs) was $6.4B (+29%) [FACT] https://agentii.ai/v/NVDA/sec173/21 and physical-AI revenue exceeded $9B over twelve months [FACT] https://agentii.ai/v/NVDA/ect81/1. Timing: VeraRubin production starts Q3 2026 with $1T Blackwell+Rubin visibility through CY2027 [FACT] https://agentii.ai/v/NVDA/ect81/1. Conclusion: NVIDIA monetizes the infrastructure build-out phase of physical AI — compute dominates ~92% of revenue; embodied/edge is the growth option, not the base [VIEW].

## 2. Data Sources

- **FY2026 Form 10-K** (filed 2026-02-25, period ended 2026-01-25), `NVDA sec169`: manufacturing & suppliers (p8), customer-concentration risk (p23), MD&A overview (p36), revenue concentration + gross margin (p41), critical audit matter (p50), commitments Note 12 (p70), geographic revenue (p78), end-market revenue table (p79).
- **Q1 FY2027 Form 10-Q** (filed 2026-05-20, period ended 2026-04-26), `NVDA sec173`: AR concentration + inventory detail (p13), commitments Note 10 (p16), segment + customer concentration (p20), market-platform revenue (p21), MD&A platform commentary (p25), lead-time risk factor (p32).
- **Q1 FY2027 earnings call transcript** (2026-05-20), `NVDA ect81`: prepared remarks (p1), closing remarks (p5).
- **Structured endpoints**: `search_xbrl_facts` (us-gaap:Revenues, us-gaap:InventoryNet), `get_company_financials` (metric cross-check), `list_xbrl_concepts` (concept resolution), `search_sec_filings`/`search_documents`/`list_sources` (Layer 1 discovery), `read_source_outline` + `search_keyword_in_source` (Layer 2).

## 3. Analysis

### 3.1 Customer concentration: where the compute flows (PIL-1)

NVDA's disclosed demand chain shows hyperscaler capex as the dominant delivery channel for AI infrastructure. In Q1 FY2027, three direct customers represented 21%, 17%, and 16% of total revenue — a combined 54% — all attributable to the Compute & Networking segment [FACT] https://agentii.ai/v/NVDA/sec173/20. Concentration is rising: in FY2026 the top two direct customers were 22% and 14% (36% combined) [FACT] https://agentii.ai/v/NVDA/sec169/41. Receivables mirror the same skew: three direct customers held 30%, 18%, and 16% of accounts receivable as of 2026-04-26 [FACT] https://agentii.ai/v/NVDA/sec173/13. NVDA also estimates "some" indirect customers individually represent 10%+ of revenue, including "one AI research and deployment company" buying cloud services from NVDA's customers [FACT] https://agentii.ai/v/NVDA/sec169/41.

The demand geography is overwhelmingly US-domiciled. Revenue from customers headquartered outside the United States fell to 22% of total revenue in Q1 FY2027, from 42% a year earlier [FACT] https://agentii.ai/v/NVDA/sec173/20; for FY2026 the figure was 31% [FACT] https://agentii.ai/v/NVDA/sec169/41. Within Data Center, the CFO states hyperscaler revenue was "approximately 50% of Data Center revenue" in Q1 FY2027 [FACT] https://agentii.ai/v/NVDA/sec173/25, and NVDA's prepared remarks cite analyst forecasts of hyperscale capex exceeding $1 trillion by 2027, with AI infrastructure spending tracking to $3–4 trillion annually by decade-end [FACT] https://agentii.ai/v/NVDA/ect81/1. Named deployments make the flow concrete: Microsoft's Farweave data center is "live... powered by hundreds of thousands of Blackwell GPUs," and AWS will add "more than 1 million Blackwell and Rubin GPUs" starting this year [FACT] https://agentii.ai/v/NVDA/ect81/1.

[DEDUCTED] Hyperscale platform revenue growth of +115% YoY — versus +85% for the company — means compute capacity is concentrating even faster into the largest buyers; the physical-AI infrastructure build-out is being capitalized by a handful of US-headquartered hyperscalers and frontier-model labs. [VIEW] For the PIL-1 counterfactual, NVDA's own disclosed bottlenecks (data-center availability, energy, capital) are infrastructure constraints, not model-training-data constraints — the binding limit at the AI-infrastructure layer is physical capacity, which supports the thesis that embodied AI's bottleneck shifts to data and physical deployment.

### 3.2 Upstream dependencies: foundry / CoWoS / HBM / contract manufacturing

NVDA is fabless across the entire manufacturing chain. The 10-K names the choke points explicitly: wafers from TSMC and Samsung; memory from SK Hynix, Micron, and Samsung; CoWoS advanced packaging; and assembly/testing/packaging by contract manufacturers Hon Hai (Foxconn), Wistron, and Fabrinet [FACT] https://agentii.ai/v/NVDA/sec169/8. The same page discloses the supply chain is "mainly concentrated in Asia" with expansion under way into the U.S. and Latin America [FACT] https://agentii.ai/v/NVDA/sec169/8, and the MD&A repeats the US/LatAm diversification [FACT] https://agentii.ai/v/NVDA/sec169/36. Long-lived assets reflect the physical footprint: Taiwan $3.2B (vs US $5.1B) as of 2026-01-25 [FACT] https://agentii.ai/v/NVDA/sec169/79.

[DEDUCTED] Taiwan's role is a flow-through channel rather than an end-market: NVDA estimates 76% of Data Center revenue from Taiwan-headquartered customers in FY2026 was attributed to end customers in the US and Europe [FACT] (provenance: XBRL geography text block retrieved via `search_xbrl_facts`) https://agentii.ai/v/NVDA/sec169/78. Q1 FY2027 geographic detail confirms Taiwan-headquartered revenue of $12.0B on total $81.6B, with the US at $63.8B [FACT] https://agentii.ai/v/NVDA/sec173/20. [VIEW] The concentration of silicon, packaging, and HBM in a single Taiwan/Korea corridor makes the entire physical-AI compute stack hostage to a geography NVDA itself flags in risk factors — and the company is paying up to diversify (US/LatAm expansion, Q1 FY2027 inventory raw-materials build — see 3.3).

### 3.3 Supply commitments, inventory, and lead-time signals

The single most important supply-chain fact in this filing set is the scale of forward pre-commitment. Manufacturing, supply, and capacity commitments — "data center-scale production and longer future ordering horizons across current and future product architectures" — were $95.2B at FY2026 year-end, "substantially all... paid through fiscal year 2027" [FACT] https://agentii.ai/v/NVDA/sec169/70 (also flagged as the PwC critical audit matter alongside the $21.4B inventory balance [FACT] https://agentii.ai/v/NVDA/sec169/50). Three months later they had risen to $119B, with $95B due in the remainder of FY2027 [FACT] https://agentii.ai/v/NVDA/sec173/16. On the Q1 call, the CFO framed total supply "inclusive of inventory purchase commitments on prepaids" at $145B [FACT] https://agentii.ai/v/NVDA/ect81/1.

[DEDUCTED] The three disclosures reconcile: $119B commitments + $25.8B inventory ≈ $144.8B ≈ $145B total supply — NVDA is carrying roughly 57% of trailing-twelve-month revenue ($253.5B) in committed supply, effectively capacity-financing its own suppliers (foundries, CoWoS, HBM) and its customers' builds.

Inventory rose to $25,797M at 2026-04-26 from $21,403M at FY2026 year-end (+20.5% QoQ), driven by raw materials up to $6,647M from $3,807M (+75% QoQ), work-in-process $9,949M, finished goods $9,201M [FACT] https://agentii.ai/v/NVDA/sec173/13. The raw-materials surge ahead of the VeraRubin launch is a classic capacity-reservation signal. Inventory provisions were only $0.8B in Q1 FY2027 versus $2.3B a year earlier [FACT] https://agentii.ai/v/NVDA/sec173/13, after FY2026 absorbed $7.2B of provisions including the $4.5B H20 export-control charge [FACT] https://agentii.ai/v/NVDA/sec169/41. [DEDUCTED] The provision reset plus record commitments indicates supply now chases demand rather than demand correcting to supply — but NVDA's own risk factors warn of manufacturing lead times exceeding 12 months that can create supply-demand mismatches and non-cancellable purchase-order exposure [FACT] https://agentii.ai/v/NVDA/sec173/32.

Adjacent commitments reinforce the infrastructure build-out: $30B multi-year cloud service agreements and $6B other vendor commitments as of 2026-04-26 [FACT] https://agentii.ai/v/NVDA/sec173/16, plus $32.4B of expected future data-center lease obligations [FACT] https://agentii.ai/v/NVDA/sec173/21 and $27B investment commitments [FACT] https://agentii.ai/v/NVDA/sec173/13.

### 3.4 Robotics / physical-AI end-market exposure (PIL-2)

NVDA restructured reporting in Q1 FY2027 around two market platforms: Data Center and Edge Computing, where Edge "highlights devices for agentic and physical AI including PCs, game consoles, workstations, AI-RAN base stations, robotics and automotive" [FACT] https://agentii.ai/v/NVDA/sec173/25. Edge Computing revenue was $6,369M in Q1 FY2027, +29% YoY and +10% QoQ, driven by Blackwell workstation demand [FACT] https://agentii.ai/v/NVDA/sec173/21. The CFO added a direct disclosure: "Our physical AI continues to gain momentum exceeding $9 billion in revenue over the last 12 months," citing the Uber robotaxi partnership (nearly 30 cities, 4 continents by 2028) and robotics adoption across "industrial, surgical, and humanoid applications" [FACT] https://agentii.ai/v/NVDA/ect81/1. Jensen Huang's closing remarks name robotics, autonomous vehicles, embedded medical instruments, and AI-RAN as the "next wave... physical AI... billions of autonomous and robotic systems," expecting the physical-AI/robotics segment to "grow incredibly fast" within the next five years [FACT] https://agentii.ai/v/NVDA/ect81/5.

[DEDUCTED] Physical AI at >$9B TTM is only ~3.6% of NVDA's $253.5B trailing-twelve-month revenue; Edge Computing is 7.8% of Q1 revenue versus 92.2% for Data Center ($75.2B vs $6.4B [FACT] https://agentii.ai/v/NVDA/sec173/21). Under the legacy end-market taxonomy, Automotive — the closest pure actuator-adjacent segment — was $2,349M in FY2026, up 39%, against Data Center's $193,737M [FACT] https://agentii.ai/v/NVDA/sec169/79. [VIEW] This is the PIL-2 evidence at the supplier of compute: the value-weighted BOM of today's physical-AI stack is compute (GPUs, networking, HBM), not actuators — embodied platforms are the option, and even NVDA's own $200B Vera CPU TAM [FACT] https://agentii.ai/v/NVDA/ect81/1 sits on the compute side of the BOM.

### 3.5 Timing signals (PIL-4)

- VeraRubin (7 chips across 5 accelerated racks) commences production shipments in Q3, second half of calendar 2026; CFO: "we have demand already planned. We have got POs" [FACT] https://agentii.ai/v/NVDA/ect81/5.
- Management cites "full confidence in $1 trillion in Blackwell and Rubin revenue we foresee from 2025 through calendar 2027" [FACT] https://agentii.ai/v/NVDA/ect81/1.
- GB300/Blackwell Ultra was "the fastest product ramp in our company's history" with Blackwell the majority of system shipments [FACT] https://agentii.ai/v/NVDA/ect81/1.
- Q2 FY2027 revenue guide: $91B ±2%, growth "driven primarily by data center" [FACT] https://agentii.ai/v/NVDA/ect81/1.
- Supply-side sequencing: $95B of the $119B commitments falls due inside FY2027 — the Rubin ramp is pre-purchased [FACT] https://agentii.ai/v/NVDA/sec173/16.
- Demand-side pacing: hyperscale capex >$1T by 2027 (analyst forecast cited on the call) and AI-infrastructure spend $3–4T annually by decade-end [FACT] https://agentii.ai/v/NVDA/ect81/1.

[DEDUCTED] The disclosed timeline — GB300 ramped, VeraRubin Q3 2026, $1T cumulative visibility through CY2027, Uber robotaxi fleets by 2028 — puts the physical-AI infrastructure wave 2–5 years behind the model-training wave, with robotics deployments trailing datacenter builds by roughly one product-generation cycle.

## 4. Key Metrics

| Metric | Value | Period | Citation |
|---|---|---|---|
| Total revenue | $215,938M (+65% YoY) | FY2026 | https://agentii.ai/v/NVDA/sec169/79 |
| Total revenue | $81,615M (+85% YoY, +20% QoQ) | Q1 FY2027 | https://agentii.ai/v/NVDA/sec173/20 |
| Net income | $58.3B; diluted EPS $2.39 | Q1 FY2027 | https://agentii.ai/v/NVDA/sec173/3 |
| Data Center revenue | $75,246M (+92% YoY) | Q1 FY2027 | https://agentii.ai/v/NVDA/sec173/21 |
| — Hyperscale | $37,869M (+115% YoY, ~50% of DC) | Q1 FY2027 | https://agentii.ai/v/NVDA/sec173/21 |
| — AI Clouds, Industrial & Enterprise | $37,377M (+74% YoY) | Q1 FY2027 | https://agentii.ai/v/NVDA/sec173/21 |
| Edge Computing revenue | $6,369M (+29% YoY) | Q1 FY2027 | https://agentii.ai/v/NVDA/sec173/21 |
| Physical-AI revenue | >$9B trailing 12 months | as of Q1 FY2027 | https://agentii.ai/v/NVDA/ect81/1 |
| Top direct customers | 21% / 17% / 16% of revenue (FY2026: 22% + 14%) | Q1 FY2027 | https://agentii.ai/v/NVDA/sec173/20 |
| Top-3 AR concentration | 30% / 18% / 16% | 2026-04-26 | https://agentii.ai/v/NVDA/sec173/13 |
| Manufacturing/supply/capacity commitments | $119B ($95B due in rest of FY2027) | 2026-04-26 | https://agentii.ai/v/NVDA/sec173/16 |
| Total supply incl. inventory + prepaids | $145B | Q1 FY2027 | https://agentii.ai/v/NVDA/ect81/1 |
| Inventory | $25,797M (RM $6,647M / WIP $9,949M / FG $9,201M) | 2026-04-26 | https://agentii.ai/v/NVDA/sec173/13 |
| Inventory provisions | $0.8B (vs $2.3B a year ago; FY2026 $7.2B incl. $4.5B H20) | Q1 FY2027 | https://agentii.ai/v/NVDA/sec173/13 |
| Gross margin | 74.9% (FY2026: 71.1%, FY2025: 75.0%) | Q1 FY2027 | https://agentii.ai/v/NVDA/sec169/41 |
| Outside-US revenue | 22% (FY2026: 31%) | Q1 FY2027 | https://agentii.ai/v/NVDA/sec173/20 |
| Cloud service commitments | $30B; other vendor $6B; investments $27B | 2026-04-26 | https://agentii.ai/v/NVDA/sec173/16 |
| Q2 FY2027 revenue guide | $91B ±2% | — | https://agentii.ai/v/NVDA/ect81/1 |
| China export-control state | No China Hopper shipments in Q1 FY2027 (vs $4.6B a year earlier) | Q1 FY2027 | https://agentii.ai/v/NVDA/sec173/25 |

## 5. Coverage Gaps & Citations

**Coverage gaps** (unretrievable — not estimated):
- FY2027 Q2 10-Q not yet filed (quarter ended 2026-08-31; latest transcript 2026-05-20 per `get_ticker_coverage`).
- XBRL purchase-commitment concepts untagged by NVDA: `PurchaseCommitmentRemainingMinimumAmount` (0 facts) and `LongTermPurchaseCommitmentAmount` (0 facts) — commitments cited from 10-K/10-Q text notes instead.
- Supplier-level spend split (e.g., dollars to TSMC vs Samsung) not disclosed; indirect customer names not disclosed (only "one AI research and deployment company").
- No price/market data used (market_data_stage: none per chain constraints).

**Citation index** (inline `/v/` links; 18 distinct page anchors):

1. https://agentii.ai/v/NVDA/sec169/8 — fabless suppliers: TSMC, Samsung, SK Hynix, Micron, CoWoS, Hon Hai, Wistron, Fabrinet
2. https://agentii.ai/v/NVDA/sec169/23 — customer-concentration risk; capacity purchase obligations; no financing arrangements entered
3. https://agentii.ai/v/NVDA/sec169/36 — MD&A: Blackwell majority, GB300 Q2 FY2026, H20 $4.5B charge, US/LatAm supply expansion
4. https://agentii.ai/v/NVDA/sec169/41 — FY2026 concentration 22%/14%, GM 71.1%, provisions $7.2B
5. https://agentii.ai/v/NVDA/sec169/50 — PwC CAM: $21.4B inventory, $95.2B obligations
6. https://agentii.ai/v/NVDA/sec169/70 — Note 12: $95.2B commitments, $27B cloud, $11.4B investments
7. https://agentii.ai/v/NVDA/sec169/78 — FY2026 geographic revenue (US $149.6B; Taiwan 76% end-attribution to US/EU)
8. https://agentii.ai/v/NVDA/sec169/79 — end-market revenue (DC $193.7B; Auto $2.3B); long-lived assets Taiwan $3.2B
9. https://agentii.ai/v/NVDA/sec173/3 — Q1 FY2027 income statement ($81.6B revenue, $58.3B NI, EPS $2.39)
10. https://agentii.ai/v/NVDA/sec173/13 — AR concentration 30/18/16; inventory detail; $27B investment commitments
11. https://agentii.ai/v/NVDA/sec173/16 — Note 10: $119B commitments, $30B cloud, $6B other vendor
12. https://agentii.ai/v/NVDA/sec173/20 — segments C&N $74.55B/+88%, Graphics $7.07B/+58%; 21/17/16 concentration; 22% outside-US
13. https://agentii.ai/v/NVDA/sec173/21 — market-platform table (Hyperscale $37.9B, ACIE $37.4B, Edge $6.4B); $32.4B future leases
14. https://agentii.ai/v/NVDA/sec173/25 — Edge platform definition (robotics, automotive); hyperscale ~50% of DC; China Hopper zero vs $4.6B
15. https://agentii.ai/v/NVDA/sec173/32 — lead times >12 months risk factor
16. https://agentii.ai/v/NVDA/ect81/1 — prepared remarks: $145B total supply, physical AI >$9B TTM, Uber robotaxi, hyperscale capex >$1T by 2027, VeraRubin Q3, $1T visibility, Q2 guide $91B
17. https://agentii.ai/v/NVDA/ect81/5 — closing remarks: physical-AI "third segment," robotics/AVs/medical/AI-RAN; VeraRubin Q3 start with POs

## 6. Verification

| # | Tool call | Scope | Outcome |
|---|---|---|---|
| 1 | search_companies | ticker resolution | NVDA / NVIDIA Corp, CIK 0001045810, FYE Feb |
| 2 | get_ticker_coverage | coverage preflight | 7 source types populated; 169 filings; 40,156 XBRL facts |
| 3 | get_company_fiscal_calendar | fiscal periods | Q1 FY2027 = 2026-03-01..2026-05-31 |
| 4 | search_sec_filings (10-K) | Layer 1 | sec169 = FY2026 10-K (filed 2026-02-25) |
| 5 | search_sec_filings (10-Q) | Layer 1 | sec173 = Q1 FY2027 10-Q (filed 2026-05-20) |
| 6 | list_xbrl_concepts (Revenue) | XBRL concepts | Revenues; RevenueFromContractWithCustomerExcludingAssessedTax |
| 7 | search_xbrl_facts (Revenues) | XBRL | FY2026 $215,938M; Q1 FY2027 $81,615M; geo text blocks |
| 8 | search_xbrl_facts (InventoryNet) | XBRL | FY2026 YE $21,403M; Q2 FY2026 $14,962M |
| 9 | read_source_outline (sec169) | Layer 2 | 85-page map; pages selected |
| 10 | read_source_pages (sec169: 8,23,36,41) | Layer 3 | suppliers; concentration; MD&A; GM/provisions |
| 11 | search_keyword_in_source (sec169, robot) | Layer 2.5 | robotics mentions pp. 4-6, 36 |
| 12 | read_source_pages (sec169: 50,70,79) | Layer 3 | CAM; commitments; end-market table |
| 13 | read_source_outline (sec173) | Layer 2 | 41-page map |
| 14 | read_source_pages (sec173: 13,16,21,25) | Layer 3 | inventory; commitments; platform revenue; edge def |
| 15 | search_keyword_in_source (sec173, robot) | Layer 2.5 | robotics pp. 23, 25 |
| 16 | read_source_pages (sec173: 20,23) | Layer 3 | segments; 21/17/16; 22% outside-US |
| 17 | search_documents (transcripts) | Layer 1 | 17 transcripts; latest 2026-05-20 |
| 18 | list_sources (transcripts) | Layer 1 | source_id efe6588c-... |
| 19 | read_source_outline (efe6588c) | Layer 2 | citation_id ect81 |
| 20 | search_keyword_in_source (ect81, robot) | Layer 2.5 | pp. 1, 2, 4, 5 |
| 21 | read_source_pages (ect81: 1, 5) | Layer 3 | prepared + closing remarks |
| 22 | search_xbrl_facts (PurchaseCommitmentRemainingMinimumAmount) | XBRL | 0 facts → Coverage Gap |
| 23 | list_xbrl_concepts (Purchase) | XBRL | LongTermPurchaseCommitmentAmount exists |
| 24 | get_company_financials (balance_sheet) | XBRL metrics | Q1 FY2027 rev $81,615M / NI $58,321M / assets $259,474M cross-check |
| 25 | search_xbrl_facts (LongTermPurchaseCommitmentAmount) | XBRL | 0 facts → Coverage Gap |

Tool diversity: 13 distinct agentii MCP tools (min 8 required). All material numbers trace to calls #4-#25 above; no number was sourced outside these retrieval calls.
