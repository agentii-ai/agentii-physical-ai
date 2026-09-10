---
artifact_id: "001-SPCX-supply-chain-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: SPCX
skill: supply-chain
mode: default
affix: supply-chain-map
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "8cb3ac1de486"
as_of: 2026-09-10
entity_claims: []
citations: []
pillars_addressed: [PIL-4]
claim_state: pinned
key_metrics:
  revenue_h1_2026_usd_m: 12508
  revenue_h1_2025_usd_m: 8138
  capex_h1_2026_usd_m: 28476
  capex_h1_2025_usd_m: 6965
  ai_capex_q2_2026_usd_m: 15828
  ai_share_h1_capex_pct: 82.7
  ai_share_q2_capex_pct: 86.2
  nameplate_compute_draw_gw_q2_2026: 1.4
  nameplate_compute_draw_gw_q2_2025: 0.4
  backlog_usd_m: 47461
  deferred_revenue_usd_m: 14286
  cash_and_cash_equiv_usd_m: 93522
  total_assets_usd_m: 192770
  total_debt_principal_usd_m: 38433
  inventory_usd_m: 2718
  falcon_launches_q2_2026: 37
  customer_launches_h1_2026: 17
  mass_to_orbit_t_q2_2026: 485
  starlink_subscribers_m_q2_2026: 12.0
conclusions:
  - "SPCX H1-2026 capex of $28.5B (AI segment 82.7%) is a measured, on-balance-sheet upstream demand signal for GPU, power, and data-center supply chains."
  - "Nameplate compute draw grew 0.4 GW to 1.4 GW YoY; management targets >2 GW by end-2026 (promotional, to triangulate)."
  - "The deployment-rate analogue (launch cadence, mass to orbit) was flat-to-down in H1-2026 while capex exploded — SPCX growth is compute-led, not launch-led."
  - "Named upstream suppliers are few: Tesla (Megapacks), Valor (AI-infrastructure financing), EchoStar (spectrum), NVIDIA (GPU supply, transcript claim); supplier policy has no long-term binding purchase orders."
facts_count: 38
deducted_count: 8
views_count: 11
citation_count: 26
---

# SPCX Supply-Chain Map — PIL-4 (Capex / Compute Demand as Upstream Leading Indicator)

## Executive Summary

SpaceX's first public 10-Q shows a company whose capital spending has abruptly pivoted from rockets and satellites to AI compute infrastructure. H1-2026 capex was $28,476M versus $6,965M a year earlier — a 309% increase — and the AI segment absorbed 82.7% of it (https://agentii.ai/v/SPCX/sec8/9). Nameplate compute draw rose from 0.4 GW to 1.4 GW year-over-year, with servers and networking equipment on the balance sheet up from $22,694M to $34,771M in six months (https://agentii.ai/v/SPCX/sec8/36). This is the upstream demand pulse that PIL-4 tracks: GPU, power, cooling, and memory supply chains are being pulled by a single quarter of SPCX disclosure alone. Simultaneously, the deployment-rate analogue is weak: Falcon customer launches fell from 21 to 17 half-over-half and mass to orbit declined (https://agentii.ai/v/SPCX/sec8/35). SPCX's compute build-out is contract-backed — $1.6B of new cloud revenue in Q2 plus a further $6.7B contracted in early Q3 — but forward compute targets are promotional claims, not measurements. Named suppliers are few (Tesla, Valor, EchoStar, NVIDIA via transcript); supplier purchase policy carries no long-term binding orders.

## Data Sources

- **10-Q (sec8)**, filed 2026-08-04, `spcx-20260630.htm` — sole quarterly report; 55 pages mapped via `read_source_outline`, 18 pages deep-read: pages 3, 4, 9, 10, 11, 13, 14, 21, 30, 31, 35, 36, 40, 41, 42, 43, 44, 47, 48, 49, 50.
- **8-Ks (sec1–sec9)** — discovery via `search_sec_filings` (9 filings, 2026-06-15 to 2026-08-14); outlines read for sec1 (IPO completion 8-K) and sec9 (Cursor merger completion 8-K).
- **Earnings call transcript (ect1)**, 2026-08-04 — pages 3–5 read (CFO segment/capex commentary and Q&A; promotional claims flagged).
- **Structured XBRL** via `search_xbrl_facts`: revenue, capex, cash, intangible-asset payments, fair-value holdings.
- **P2.1 verification record**: `get_ticker_coverage` (SPCX: 8 sec_filings records, 1,517 xbrl_facts, 10 src_documents, 1 transcript); `search_xbrl_facts` on `RevenueFromContractWithCustomerExcludingAssessedTax` returned H1-2026 = $12,508M (https://agentii.ai/v/SPCX/sec8/13); `Revenues` returned zero rows — both as expected. [FACT]

## Analysis

### 1. Capex: the measured PIL-4 leading indicator

H1-2026 purchases of property, plant, and equipment were $28,476M versus $6,965M in H1-2025, per the cash flow statement (https://agentii.ai/v/SPCX/sec8/9) and confirmed as the XBRL fact `PaymentsToAcquirePropertyPlantAndEquipment` (H1-2026: 28,476,000,000; H1-2025: 6,965,000,000). [FACT] [FACT]

Segment-level capex is disclosed in Note 18: Q2-2026 capex was $18,369M total — Space $1,174M, Connectivity $1,367M, AI $15,828M (https://agentii.ai/v/SPCX/sec8/30); H1-2026 was Space $2,226M, Connectivity $2,699M, AI $23,551M (https://agentii.ai/v/SPCX/sec8/31). The AI segment alone carried 82.7% of H1 capex and 86.2% of Q2 capex. [DEDUCTED] [DEDUCTED]

The year-over-year trajectory is starker at the segment level: AI segment capex was $749M in Q2-2025 and $15,828M in Q2-2026, a roughly 21x increase in one year (https://agentii.ai/v/SPCX/sec8/31). [FACT] [DEDUCTED]

The MD&A attributes the $21,511M year-over-year increase in investing outflows to "the build out of data centers and related infrastructure, and space launch facilities and related infrastructure" (https://agentii.ai/v/SPCX/sec8/50). [FACT] On the balance sheet the composition confirms compute dominance: servers and networking equipment $34,771M (vs $22,694M at Dec 31, 2025), satellites $13,788M, data center infrastructure $3,991M, and construction-in-progress $12,554M (vs $4,604M), "primarily comprised of ongoing construction and expansion of the facilities and equipment as well as AI infrastructure that has not yet been placed in service" (https://agentii.ai/v/SPCX/sec8/14). [FACT] Servers and networking grew 53% in six months. [DEDUCTED]

Additional unbooked-but-real capex flows: $5,513M of PP&E purchases were sitting in accrued expenses/accounts payable at June 30, 2026, and $3,921M of PP&E was financed by "other financings" (https://agentii.ai/v/SPCX/sec8/10). [FACT] [FACT] Depreciation is already ramping: $2,735M in Q2-2026 alone, versus $1,310M in Q2-2025 (https://agentii.ai/v/SPCX/sec8/14). [FACT] The AI segment carries $3,378M of the $5,290M H1 depreciation (https://agentii.ai/v/SPCX/sec8/31). [FACT]

### 2. Compute demand: installed capacity, contracted revenue, and the GPU pipeline

Nameplate compute draw — GPUs installed multiplied by all-in power draw — reached 1.4 GW at June 30, 2026 versus 0.4 GW a year earlier (https://agentii.ai/v/SPCX/sec8/36). [FACT] Forward targets are promotional: the CFO expects "over 2 gigawatts of compute capacity" by end-2026, and Musk stated a 10 GW end-2027 target with 20 GW of power/cooling projects (~15 GW expected online) and "a very significant percent of [NVIDIA's] GPUs next year" (https://agentii.ai/v/SPCX/ect1/3). [VIEW] None of these is auditable; treat as claims to triangulate against supplier order books and utility interconnection data.

Contractual demand is the harder evidence. Q2-2026 AI Solutions & Infrastructure revenue was $2,194M, up from $311M a year earlier, of which ~$1,600M was incremental AI infrastructure (cloud) revenue from "new AI infrastructure contracts" (https://agentii.ai/v/SPCX/sec8/13) (https://agentii.ai/v/SPCX/sec8/44). [FACT] [FACT] On the call, the CFO said another $6.7B of cloud services revenue was contracted in the first weeks of Q3 on a 6-month contract beginning October 2026, with Google and Anthropic deals ramping in late Q3/October (https://agentii.ai/v/SPCX/ect1/3). [FACT — transcript claim, promotional] Management claims a less-than-1-year payback on new compute capex (https://agentii.ai/v/SPCX/ect1/3). [VIEW] The company's own risk language names the supply-side constraint: "our ability to obtain sufficient power, GPUs, and other critical components and manage our supply chain to support our operations and growth" (https://agentii.ai/v/SPCX/sec8/3). [FACT] Musk adds the memory constraint: memory output growing ~20%/yr against demand he estimates at 200%+/yr (https://agentii.ai/v/SPCX/ect1/5). [VIEW — estimate]

Customer concentration in the AI segment is disclosed but unnamed: "Customer B" was 19.5% of consolidated revenue in Q2-2026 (12.2% H1) and "relates to the AI segment" (https://agentii.ai/v/SPCX/sec8/14). [FACT] Given the disclosed cloud-services ramp, this is consistent with a single hyperscaler-like anchor tenant — a concentration risk for SPCX's compute monetization. [DEDUCTED] "Customer A" (18.3% of Q2 revenue, spanning all three segments) is consistent with the U.S. government; it has been 16.7–19.9% across the disclosed periods (https://agentii.ai/v/SPCX/sec8/14). [FACT] [DEDUCTED]

### 3. Deployment-rate analogue: launch cadence is flat-to-down while capex explodes

Falcon launches: 37 in Q2-2026 (45 in Q2-2025); customer launches 10 (9); internal 27 (36). H1: 77 Falcon launches (81), customer 17 (21), internal 60 (60). Starship: 1 launch in both Q2 periods; 1 H1-2026 versus 3 H1-2025 (https://agentii.ai/v/SPCX/sec8/35). [FACT] [FACT] Mass to orbit fell to 485 metric tons in Q2-2026 from 652 a year earlier, and customer payload mass was flat at 87–88t (https://agentii.ai/v/SPCX/sec8/35). [FACT] The AI segment is expected to consume "a significant amount" of launch capacity in the future per the company's own statement (https://agentii.ai/v/SPCX/sec8/36) — a forward claim, not yet visible in launch data. [VIEW]

The triangulation point for PIL-4: internal constellation deployment (the mechanism that would carry embodied-AI infrastructure to orbit) was flat (60 internal launches in both H1 periods), while ground-based compute capex rose 309%. [DEDUCTED] SPCX's capex pulse currently signals data-center build-out, not an orbital embodied-AI deployment ramp. SpaceX R&D still funds the carrier: Space R&D rose $383M in Q2 "to support continued development of the Starship vehicle" (https://agentii.ai/v/SPCX/sec8/42), and Space capex of $2,226M in H1 funds launch pads, Gigabays, and Raptor production (https://agentii.ai/v/SPCX/ect1/3). [FACT] [FACT] Musk's "at least 1 flight a day within a year" Starship cadence is promotional (https://agentii.ai/v/SPCX/ect1/4). [VIEW]

### 4. Supplier relationships: named and structured

Named upstream relationships are sparse in a one-quarter filing:
- **Tesla (related party):** $329M of Megapack battery products purchased in H1-2026 and recorded in PP&E (Q2: $295M); $506M of Megapacks and $131M of Cybertrucks in 2025 (https://agentii.ai/v/SPCX/sec8/30). [FACT] This is the only equipment supplier quantified on the balance sheet — relevant to power-storage supply chains for data centers. [VIEW]
- **Valor Equity Partners (related party):** April 2026 equipment lease for AI infrastructure hardware, deemed a failed sale-leaseback; debt of $2,039M current and $11,290M non-current recorded, with $327M (Q2) / $513M (H1) interest expense (https://agentii.ai/v/SPCX/sec8/30) (https://agentii.ai/v/SPCX/sec8/21). [FACT] [FACT] AI-infrastructure hardware is thus partly financed via related-party lease structures — a financing-structure concentration worth monitoring. [DEDUCTED]
- **EchoStar:** ~$19.6B spectrum acquisition (AWS-4, H-Block, AWS-3); $856M paid through June 30, 2026 (also the XBRL fact `PaymentsToAcquireIntangibleAssets`) (https://agentii.ai/v/SPCX/sec8/49). [FACT]
- **NVIDIA:** transcript-only claim that SpaceX "will receive a very significant percent of their GPUs next year" (https://agentii.ai/v/SPCX/ect1/4). [FACT — transcript claim] Not verifiable from filings; treat as promotional. [VIEW]
- **The Bank of New York Mellon:** trustee on the $25,000M SpaceX Notes (https://agentii.ai/v/SPCX/sec8/48). [FACT]

On supplier contracts generally, the company states it enters "agreements with suppliers for the purchase of parts and raw materials" but "these contracts generally do not have long-term binding and enforceable purchase orders" (https://agentii.ai/v/SPCX/sec8/49). [FACT] This limits supply-chain-map granularity: SPCX's upstream exposure (GPU vendors, power equipment, turbine/memory suppliers) is not itemized anywhere in the filing. [VIEW]

Inventory — the in-house manufactured build pipeline — is $2,718M (raw materials $1,122M, WIP $875M, finished goods $721M), up from $2,416M at year-end (https://agentii.ai/v/SPCX/sec8/14). [FACT] Vertical integration is explicit: Starlink satellite production is internal, and launch costs for internal Starlink launches are capitalized into satellites in PP&E rather than recognized as revenue (https://agentii.ai/v/SPCX/sec8/36). [FACT] Starlink Kit production spend rose $148M in Q2 supporting Connectivity growth (https://agentii.ai/v/SPCX/sec8/43). [FACT]

### 5. Funding capacity: how long the capex pulse can run

The balance sheet can sustain the current pace: cash and cash equivalents of $93,522M, marketable securities $6,487M, total assets $192,770M, and shareholders' equity of $127,224M after the June IPO (https://agentii.ai/v/SPCX/sec8/4). [FACT] IPO net proceeds were $85,675M (638.9M shares at $135.00) and the June 2026 SpaceX Notes raised $25,000M (five tranches, 2031–2056, weighted-average coupon 5.855%), partially repaying a bridge loan (https://agentii.ai/v/SPCX/sec8/47) (https://agentii.ai/v/SPCX/sec8/48). [FACT] [FACT] Total debt principal is $38,433M with only $944M maturing in the rest of 2026 and $25,201M thereafter (https://agentii.ai/v/SPCX/sec8/21). [FACT] The CFO's framing: next two quarters of capex "very similar to the current quarter," i.e., roughly $18B/quarter run-rate (https://agentii.ai/v/SPCX/ect1/4). [VIEW] Management retains explicit flexibility: "if our near-term data center needs decrease in scale or ramp more slowly than expected... we may reduce future capital expenditures in this segment and reallocate" (https://agentii.ai/v/SPCX/sec8/47). [FACT] This makes the compute-capex pulse contingent on cloud-contract absorption — a genuine falsifier hook for PIL-4. [VIEW]

### 6. Starlink and robotics: context, not falsifier material

Starlink grew to 12.0M subscribers (from 6.0M) at $66 ARPU (from $85) (https://agentii.ai/v/SPCX/sec8/36), and Connectivity income from operations was $1,656M in Q2 (https://agentii.ai/v/SPCX/sec8/30). [FACT] Management claims robotics (autos, humanoids) "will dramatically increase the demand for connectivity" (https://agentii.ai/v/SPCX/ect1/4). [VIEW] Per plan risk note 7, Starlink's relevance to embodied AI is indirect (connectivity backhaul, not embodiment): recorded here as context only, excluded from pillar falsifiers.

## Key Metrics

| Metric | Value | Period | Citation |
|---|---|---|---|
| Revenue (RFCCET) | $12,508M | H1-2026 | https://agentii.ai/v/SPCX/sec8/13 |
| Capex (PP&E purchases) | $28,476M | H1-2026 | https://agentii.ai/v/SPCX/sec8/9 |
| Capex YoY | +309% ($6,965M → $28,476M) | H1 | https://agentii.ai/v/SPCX/sec8/9 |
| AI segment capex | $15,828M (Q2) / $23,551M (H1) | 2026 | https://agentii.ai/v/SPCX/sec8/30 |
| AI share of capex | 86.2% (Q2) / 82.7% (H1) | 2026 | https://agentii.ai/v/SPCX/sec8/30 |
| AI capex Q2-2025 → Q2-2026 | $749M → $15,828M (~21x) | Q2 | https://agentii.ai/v/SPCX/sec8/31 |
| Nameplate compute draw | 1.4 GW (vs 0.4 GW) | Jun 30 | https://agentii.ai/v/SPCX/sec8/36 |
| Servers & networking equipment | $34,771M (vs $22,694M) | Jun 30 | https://agentii.ai/v/SPCX/sec8/14 |
| AI infrastructure revenue | +$1,600M incremental (Q2) | Q2-2026 | https://agentii.ai/v/SPCX/sec8/44 |
| Backlog | $47,461M | Jun 30 | https://agentii.ai/v/SPCX/sec8/14 |
| Deferred revenue | $14,286M | Jun 30 | https://agentii.ai/v/SPCX/sec8/13 |
| Customer A / Customer B revenue share | 18.3% / 19.5% | Q2-2026 | https://agentii.ai/v/SPCX/sec8/14 |
| Falcon / Starship launches | 37 / 1 (Q2); 77 / 1 (H1) | 2026 | https://agentii.ai/v/SPCX/sec8/35 |
| Mass to orbit | 485 t (vs 652 t) | Q2 | https://agentii.ai/v/SPCX/sec8/35 |
| Cash + marketable securities | $93,522M + $6,487M | Jun 30 | https://agentii.ai/v/SPCX/sec8/4 |
| Total debt principal | $38,433M | Jun 30 | https://agentii.ai/v/SPCX/sec8/21 |
| Inventory | $2,718M | Jun 30 | https://agentii.ai/v/SPCX/sec8/14 |

## Coverage Gaps

1. **No multi-year history**: one 10-Q (sec8) + 8-Ks only; the audited 10-K/Prospectus-level supplier detail referenced in the filing ("Material Cash Commitments in our Prospectus") is not in this corpus. Trend analysis is limited to the H1-2025 comparatives inside the 10-Q.
2. **No named GPU/ASIC/memory/power suppliers in filings**: NVIDIA is transcript-only. GPU purchase obligations, utility interconnection agreements, and turbine/power-equipment orders are not disclosed.
3. **Customer A/B not named**: government (A) and AI-segment (B) identities inferred, not stated.
4. **Supplier tier detail absent**: no 10%+ supplier concentration disclosure beyond related parties (Tesla, Valor).
5. **No market data**: market_data_stage none — no price-derived indicators.
6. **Failed calls**: initial `get_ticker_coverage` and a `sec4` outline call hit `RATE_LIMIT_EXCEEDED` (shared backend); both superseded by later successful calls. `search_xbrl_facts` on the exact concept `Assets` fuzzy-matched 41 related concepts instead of the total (recovered via balance-sheet page read).
7. **P2.1 note**: the 10-Q reports $12.508B H1-2026 revenue; `Revenues` concept confirmed empty — citations must use the RFCCET concept only.

## Citations (roll-up index)

1. https://agentii.ai/v/SPCX/sec8/9 — cash flow statement: capex $28,476M/$6,965M, investing $(34,487)M
2. https://agentii.ai/v/SPCX/sec8/10 — supplemental: PP&E in AP/accruals $5,513M; financed $3,921M
3. https://agentii.ai/v/SPCX/sec8/13 — revenue disaggregation; P2.1 revenue verification
4. https://agentii.ai/v/SPCX/sec8/14 — PP&E composition; backlog; customer concentration; inventory; depreciation
5. https://agentii.ai/v/SPCX/sec8/30 — related party (Tesla, Valor); Q2-2026 segment P&L and capex
6. https://agentii.ai/v/SPCX/sec8/31 — H1-2026 segment capex; Q2-2025 comparatives
7. https://agentii.ai/v/SPCX/sec8/35 — launches, mass to orbit
8. https://agentii.ai/v/SPCX/sec8/36 — nameplate compute draw; Starlink subscribers/ARPU; revenue recognition
9. https://agentii.ai/v/SPCX/sec8/40 — consolidated results
10. https://agentii.ai/v/SPCX/sec8/41 — R&D drivers (AI data center expansion, Starship)
11. https://agentii.ai/v/SPCX/sec8/42 — Space segment results; Starship R&D
12. https://agentii.ai/v/SPCX/sec8/43 — Connectivity results; Starlink Kit production spend
13. https://agentii.ai/v/SPCX/sec8/44 — AI segment results; $1.6B cloud revenue
14. https://agentii.ai/v/SPCX/sec8/47 — Segment Adjusted EBITDA; liquidity; capex flexibility language
15. https://agentii.ai/v/SPCX/sec8/48 — SpaceX Notes $25B terms
16. https://agentii.ai/v/SPCX/sec8/49 — supplier purchase-order policy; EchoStar spectrum $19.6B
17. https://agentii.ai/v/SPCX/sec8/50 — cash flow variance (capex +$21,511M build-out explanation)
18. https://agentii.ai/v/SPCX/sec8/3 — forward-looking statements (power, GPUs, critical components)
19. https://agentii.ai/v/SPCX/sec8/4 — balance sheet
20. https://agentii.ai/v/SPCX/sec8/21 — failed sale-leaseback AI infrastructure; debt maturities
21. https://agentii.ai/v/SPCX/sec8/11 — nature of business; IPO; xAI merger
22. https://agentii.ai/v/SPCX/ect1/3 — CFO: Q2 capex ~$18.4B, >2 GW target, $6.7B new cloud contracts, payback <1yr
23. https://agentii.ai/v/SPCX/ect1/4 — Musk: 10 GW/20 GW targets, NVIDIA GPUs; Starship cadence; robotics-connectivity claim
24. https://agentii.ai/v/SPCX/ect1/5 — memory supply-demand; Google/Anthropic ramp; Grok 10% compute
25. https://agentii.ai/v/SPCX/sec9/2 — Cursor (Anysphere) merger completion, ~$60B, 389.3M shares
26. https://agentii.ai/v/SPCX/sec1/3 — IPO completion 8-K: 638,888,888 shares at $135.00

## Verification (call trace)

| # | Tool call | Target | Result |
|---|---|---|---|
| 1 | get_ticker_coverage | SPCX | coverage profile: sec_filings 8, xbrl_facts 1,517, src_documents 10, transcript 1 (first attempt rate-limited; retried OK) |
| 2 | search_xbrl_facts | RevenueFromContractWithCustomerExcludingAssessedTax | 4 rows; H1-2026 $12.508B — P2.1 verified |
| 3 | search_xbrl_facts | Revenues | 0 rows — P2.1 verified |
| 4 | search_sec_filings | SPCX | 9 filings sec1–sec9 (6/15–8/14/2026) |
| 5 | read_source_outline | sec8 | 55-page map |
| 6 | read_source_pages | sec8: 9,10,13,14 | cash flows, supplemental, revenue, inventory/PP&E |
| 7 | read_source_pages | sec8: 30,31,35,36 | related parties, segment capex, launch/compute metrics |
| 8 | read_source_pages | sec8: 40,42,44,50 | consolidated/segment results, cash flow variance |
| 9 | read_source_pages | sec8: 41,47,48,49 | R&D drivers, liquidity, debt, spectrum, supplier policy |
| 10 | read_source_pages | sec8: 3,11,43 | forward-looking statements, business description, Connectivity |
| 11 | read_source_outline | sec1 | IPO completion 8-K |
| 12 | batch_search | 7 sub-queries | XBRL results stripped of values; transcript confirmed (rate-limited partial) |
| 13 | search_xbrl_facts | PaymentsToAcquirePropertyPlantAndEquipment | $28,476M / $6,965M — matches page 9 |
| 14 | search_documents | SPCX | 10 docs; 8-K descriptions (notes offering, Cursor, earnings release) |
| 15 | list_sources | SPCX earnings_call_transcript | source_id resolved |
| 16 | read_source_outline | (transcript source_id) | citation_id = ect1 |
| 17 | read_source_pages | ect1: 3,4,5 | CFO capex/compute commentary; Q&A |
| 18 | search_xbrl_facts | CashAndCashEquivalentsAtCarryingValue | $93,522M (6/30/26); $24,747M (12/31/25) |
| 19 | search_xbrl_facts | Assets | fuzzy match (41 rows) — no clean total; PaymentsToAcquireIntangibleAssets $856M captured |
| 20 | read_source_pages | sec8: 4,21 | balance sheet ($192,770M assets); debt maturities $38,433M |
| 21 | read_source_outline | sec9 | Cursor completion ~$60B, 389.3M shares, Aug 14, 2026 |

Tool diversity: 8 distinct agentii tools used (get_ticker_coverage, search_xbrl_facts, search_sec_filings, read_source_outline, read_source_pages, batch_search, search_documents, list_sources). All material numbers trace to calls above; no UNFRAMED_REFERENCE.
