---
artifact_id: "001-NVDA-risk-general-risk-factors-identification-assessment-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: NVDA
skill: risk
mode: general-risk-factors-identification-assessment
affix: risk-assessment
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "953fc5d396e7"
as_of: 2026-09-10
entity_claims: []
citations:
  - "https://agentii.ai/v/NVDA/sec169/37"
  - "https://agentii.ai/v/NVDA/sec169/23"
  - "https://agentii.ai/v/NVDA/sec169/8"
  - "https://agentii.ai/v/NVDA/sec169/9"
  - "https://agentii.ai/v/NVDA/sec169/13"
  - "https://agentii.ai/v/NVDA/sec169/25"
  - "https://agentii.ai/v/NVDA/sec169/15"
  - "https://agentii.ai/v/NVDA/sec169/16"
  - "https://agentii.ai/v/NVDA/sec169/50"
  - "https://agentii.ai/v/NVDA/sec169/70"
  - "https://agentii.ai/v/NVDA/sec169/10"
  - "https://agentii.ai/v/NVDA/sec169/36"
  - "https://agentii.ai/v/NVDA/sec169/77"
  - "https://agentii.ai/v/NVDA/sec169/78"
  - "https://agentii.ai/v/NVDA/sec169/79"
  - "https://agentii.ai/v/NVDA/sec173/3"
  - "https://agentii.ai/v/NVDA/sec173/16"
  - "https://agentii.ai/v/NVDA/sec173/21"
  - "https://agentii.ai/v/NVDA/sec173/23"
  - "https://agentii.ai/v/NVDA/sec173/27"
  - "https://agentii.ai/v/NVDA/sec173/32"
  - "https://agentii.ai/v/NVDA/sec173/33"
  - "https://agentii.ai/v/NVDA/sec173/38"
  - "https://agentii.ai/v/NVDA/sec157/2"
pillars_addressed: [PIL-3]
claim_state: pinned
key_metrics:
  revenue_fy2026_usd_b: 215.938
  revenue_q1_fy2027_usd_b: 81.615
  gross_margin_fy2026_pct: 71.1
  gross_margin_q1_fy2027_pct: 74.9
  net_income_fy2026_usd_b: 120.067
  customer_concentration_fy2026_pct: "22% + 14%"
  customer_concentration_q1_fy2027_pct: "21% + 17% + 16%"
  manufacturing_commitments_apr2026_usd_b: 119
  inventory_fy2026_usd_b: 21.4
  purchase_obligations_fy2026_usd_b: 95.2
  h20_charge_q1_fy2026_usd_b: 4.5
conclusions:
  - "NVDA's dominant risk cluster is demand/supply mismatch at datacenter scale: 12-month+ lead times against $119B of supply commitments, already crystallized once via the $4.5B H20 charge."
  - "Customer concentration is rising: 22%/14% in FY2026 vs 12%/11% in FY2025; three direct customers were 54% of Q1 FY2027 revenue."
  - "Energy and data-center capacity are external gates on NVDA's revenue growth - a multi-year constraint outside NVDA's control."
  - "For PIL-3's counterfactual: NVDA's physical-AI exposure (Automotive $2.349B, ~1.1% of FY2026 revenue) is de minimis versus Data Center, so robotics-side reliability risks do not currently threaten the compute thesis; compute-side concentration risks do."
facts_count: 31
deducted_count: 10
views_count: 3
citation_count: 24
---

# NVDA — General Risk Factors Identification & Assessment
**Mode:** general-risk-factors-identification-assessment · **Skill:** risk · **Corpus:** agentii-2026-09-10 · **Pillar:** PIL-3 (manipulation-reliability gates deployment — NVDA as compute-boundness counterfactual)

## Executive Summary

NVIDIA closed FY2026 (ended 2026-01-25) with revenue of $215.9B, up 65%, gross margin 71.1% (-3.9 pts), and net income of $120.1B [FACT] https://agentii.ai/v/NVDA/sec169/37. Q1 FY2027 revenue was $81.6B, +85% YoY, with gross margin rebounding to 74.9% from 60.5% [FACT] https://agentii.ai/v/NVDA/sec173/27. The issuer-identified risk stack concentrates on five clusters: (1) demand/supply mismatch driven by >12-month manufacturing lead times against $119B of supply commitments [FACT] https://agentii.ai/v/NVDA/sec173/16; (2) revenue concentration — two direct customers at 22% and 14% of FY2026 revenue, and three at 21%/17%/16% in Q1 FY2027 [FACT] https://agentii.ai/v/NVDA/sec169/23 https://agentii.ai/v/NVDA/sec173/27; (3) energy/data-center capacity gating customer buildouts [FACT] https://agentii.ai/v/NVDA/sec169/16; (4) product-transition execution at a one-year cadence (Blackwell → Rubin) [FACT] https://agentii.ai/v/NVDA/sec169/36; and (5) export-control shocks, already crystallized once in the $4.5B H20 charge [FACT] https://agentii.ai/v/NVDA/sec169/10. Near-term risk is dominated by export-control economics and Gaming supply headwinds; long-term risk by China-market foreclosure strengthening competitor ecosystems [DEDUCTED] https://agentii.ai/v/NVDA/sec169/10. For PIL-3, the counterfactual reading is that NVDA's physical-AI (robotics/automotive) revenue exposure is de minimis (~1.1% of revenue) while its compute-side concentration risks are large — the thesis's compute-boundness assumption, not manipulation reliability, is where NVDA's vulnerability lies [DEDUCTED] https://agentii.ai/v/NVDA/sec169/79.

## Risk Identification

Standardized category inventory from Item 1A of the FY2026 10-K risk-factor summary [FACT] https://agentii.ai/v/NVDA/sec169/13:

| Category | Issuer risk factor (condensed) | Evidence page |
|---|---|---|
| Supply/manufacturing | Dependency on third-party suppliers; reduced control over yields and delivery | https://agentii.ai/v/NVDA/sec169/13 |
| Demand estimation | Long lead times + demand mis-estimation → mismatches, inventory write-downs | https://agentii.ai/v/NVDA/sec169/15 |
| Product transitions | Multi-architecture concurrency; inventory provisions for low-yielding Blackwell in Q2 FY2025 | https://agentii.ai/v/NVDA/sec169/16 |
| Customer concentration | 22% + 14% direct customers FY2026; indirect customers ≥10% individually | https://agentii.ai/v/NVDA/sec169/23 |
| Counterparty | Long-term capacity purchase obligations; financing requests from partners (none entered) | https://agentii.ai/v/NVDA/sec169/23 |
| Export controls | H20 license requirement → $4.5B charge; China data-center market effectively foreclosed | https://agentii.ai/v/NVDA/sec169/10 |
| Energy/capacity | Data-center, energy, and capital availability gate customer AI buildouts | https://agentii.ai/v/NVDA/sec169/16 |
| Geopolitics | Taiwan/South Korea supply dependence; Hong Kong warehousing/distribution | https://agentii.ai/v/NVDA/sec173/38 |
| IP/competition | AMD, Huawei, Intel; cloud internal ASIC teams | https://agentii.ai/v/NVDA/sec169/9 |
| Regulatory/antitrust | Worldwide regulator interest; EU AI Act; China Mellanox probe | https://agentii.ai/v/NVDA/sec169/25 |

All rows above are issuer-disclosed Item 1A risk factors reproduced from the cited pages [FACT].

## Near-Term Risk Assessment (0–4 quarters)

- **Export-control economics.** Q1 FY2027 gross margin included a net unfavorable inventory-provision effect of 1.2%, versus 11.0% a year earlier driven by the $4.5B H20 charge [FACT] https://agentii.ai/v/NVDA/sec173/27. The H200 license path (Feb 2026) carries a 25% tariff upon U.S. importation and has generated zero revenue to date [FACT] https://agentii.ai/v/NVDA/sec169/10.
- **Gaming supply headwind.** NVIDIA states it expects supply constraints to be a headwind to Gaming in Q1 FY2027 and beyond [FACT] https://agentii.ai/v/NVDA/sec169/16. Gaming was $16.0B of FY2026 revenue, 7.4% of total [FACT] https://agentii.ai/v/NVDA/sec169/79.
- **Commitment wall.** As of 2026-04-26, manufacturing/supply/capacity commitments were $119B, of which $95B is payable in the remainder of FY2027, plus $30B of multi-year cloud service agreements [FACT] https://agentii.ai/v/NVDA/sec173/16. A demand pause would convert this into margin compression or charges, as the H20 episode demonstrated [DEDUCTED] https://agentii.ai/v/NVDA/sec169/10.
- **Transition execution.** Rubin is expected to begin shipping in H2 FY2027 while Blackwell still accounts for the majority of system shipments [FACT] https://agentii.ai/v/NVDA/sec173/33 https://agentii.ai/v/NVDA/sec173/23. Concurrency of architectures is flagged by the issuer as a source of revenue volatility [FACT] https://agentii.ai/v/NVDA/sec173/33.
- **Concentration trajectory.** Direct-customer concentration deepened from 12%/11% in FY2025 to 22%/14% in FY2026 and 21%/17%/16% in Q1 FY2027 [FACT] https://agentii.ai/v/NVDA/sec169/78 https://agentii.ai/v/NVDA/sec173/27. Purchase orders are generally cancellable without penalty, amplifying demand-shock transmission [DEDUCTED] https://agentii.ai/v/NVDA/sec169/23.

## Long-Term Risk Assessment (>1 year)

- **China-market foreclosure.** NVIDIA states it is "effectively foreclosed from competing in China's data center computing/compute market" and that this "helped our competitors build larger developer and customer ecosystems to challenge us worldwide" [FACT] https://agentii.ai/v/NVDA/sec169/10. This converts a single-market loss into a global competitive-structure risk over 3–5 years [DEDUCTED] https://agentii.ai/v/NVDA/sec169/10.
- **Supply-chain geographic concentration.** NVDA's fabless chain (TSMC/Samsung foundries, SK Hynix/Micron memory, Hon Hai/Wistron/Fabrinet assembly) is concentrated in Taiwan and South Korea; long-lived assets in Taiwan were $3.2B of $10.4B total [FACT] https://agentii.ai/v/NVDA/sec169/8 https://agentii.ai/v/NVDA/sec169/79. The issuer explicitly warns that restrictions on Taiwan/Korea supply would "negatively impact our business and financial results" [FACT] https://agentii.ai/v/NVDA/sec173/38.
- **Substitution threat.** Customers are developing their own ASICs "optimized for certain workloads that may not require all of the features and functionality our data center systems provide" [FACT] https://agentii.ai/v/NVDA/sec173/32. Open-source foundation models, if deployed on competitors' platforms, "could reduce demand for our products and services" [FACT] https://agentii.ai/v/NVDA/sec169/36.
- **Energy as structural gate.** "Expanding energy capacity to meet demand is a complex, multi-year process involving significant regulatory, technical, and construction challenges" [FACT] https://agentii.ai/v/NVDA/sec169/16. This is the single most PIL-3-relevant constraint: it caps the deployment rate of the very systems whose reliability the thesis's physical-AI pillar depends on [VIEW] https://agentii.ai/v/NVDA/sec173/23.

## Risk Trend Analysis

- **Scale of mismatch risk is growing.** Purchase obligations grew from $95.2B at FY2026 year-end to $119B three months later (+25%), with $95B due inside twelve months [FACT] https://agentii.ai/v/NVDA/sec169/50 https://agentii.ai/v/NVDA/sec173/16. The auditor (PwC) designated inventory/purchase-commitment provisions a critical audit matter, citing "significant judgment... regarding future demand and market conditions" [FACT] https://agentii.ai/v/NVDA/sec169/50.
- **Concentration risk is trending up, not down**, across FY2024→FY2026 (13% → 12%+11% → 22%+14% for the largest direct customers) [DEDUCTED] https://agentii.ai/v/NVDA/sec169/78.
- **Margin trend is recovering but provision-laden.** Q1 FY2027 GM of 74.9% versus FY2026's 71.1% reflects the non-repeat of the H20 charge more than structural improvement [DEDUCTED] https://agentii.ai/v/NVDA/sec173/27 https://agentii.ai/v/NVDA/sec169/37.
- **Risk disclosures themselves are widening**: the 10-K adds energy/capacity, open-source-model, and U.S.-manufacturing-ramp factors absent from prior years' typical lists [DEDUCTED] https://agentii.ai/v/NVDA/sec169/16.

## Novel Risk Factors (not in prior-year filings)

- **USG revenue-sharing expectation.** USG officials "expressed an expectation that the USG will receive 15% or more of the revenue generated from licensed sales of our products" — a novel quasi-fiscal condition on export licenses [FACT] https://agentii.ai/v/NVDA/sec169/10. No regulation codifies it, creating a non-quantifiable contingent liability [DEDUCTED] https://agentii.ai/v/NVDA/sec169/10.
- **Chip-level government mandates.** The USG may require "chip tracking and throttling mechanisms that could disable or impair GPUs if certain events... are detected" — a direct intrusion into product architecture with system-vulnerability and liability implications [FACT] https://agentii.ai/v/NVDA/sec173/37. Notably, this is a manipulation/reliability risk imposed by policy, the inverse of the thesis's premise that reliability engineering is the moat [VIEW] https://agentii.ai/v/NVDA/sec173/37.
- **Open-source model geopolitics.** Regulatory restriction on models originating in China (DeepSeek, Qwen, KIMMI) "could have a material impact" because demand for those models drives demand for NVDA products [FACT] https://agentii.ai/v/NVDA/sec173/37.
- **Ecosystem-financing exposure.** NVDA invested $17.5B in private companies and infrastructure funds in FY2026 and provided $3.5B in land/power/shell guarantees to early-stage companies — risks borne to pull demand forward [FACT] https://agentii.ai/v/NVDA/sec169/37.

## PIL-3 (Pillar) Relevance

PIL-3 holds that manipulation reliability gates physical-AI deployment; NVDA is the compute-boundness counterfactual. The risk factors above show NVDA's exposure runs almost entirely through compute-scale economics (lead times, commitments, energy, concentration) rather than through physical-embodiment reliability [DEDUCTED]. Automotive — NVDA's closest physical-AI segment — was $2.349B of FY2026 revenue (1.1%), versus Data Center's $193.7B (89.7%) [FACT] https://agentii.ai/v/NVDA/sec169/79. This supports the thesis counterfactual: if compute-boundness (not manipulation) is the binding constraint, NVDA's risk factors — and the $4.5B H20 charge — are the template for what a compute-scarcity shock looks like, while manipulation-reliability shocks remain sub-material to NVDA today [VIEW] https://agentii.ai/v/NVDA/sec169/10.

## Coverage Gaps

- Q2 FY2027 (ended 2026-08-31) 10-Q was not in the corpus at retrieval time (latest 10-Q = Q1 FY2027, citation sec173); near-term risk statements are therefore one quarter stale [FACT] (from get_ticker_coverage: latest sec_filings date 2026-05-09).
- The FY2026 10-K geographic recast changed revenue reporting to customer-headquarters basis in Q3 FY2026; Taiwan figures (76% of Data Center revenue re-attributed to U.S./Europe end customers) complicate regional exposure comparisons [FACT] https://agentii.ai/v/NVDA/sec169/78.
- No retrieval of earnings-call transcripts for this mode; management's qualitative risk commentary beyond filings is not included.
- 8-K for the AI Diffusion rule (2025-01-17, sec153) was discovered at Layer 1 but not deep-read; IFR details are cited from 10-K/10-Q restatement instead.

## Citations (roll-up index)

1. FY2026 financial summary — https://agentii.ai/v/NVDA/sec169/37
2. Customer concentration FY2026 — https://agentii.ai/v/NVDA/sec169/23
3. Lead times / demand mismatch — https://agentii.ai/v/NVDA/sec169/15
4. Product transitions / energy gate — https://agentii.ai/v/NVDA/sec169/16
5. PwC critical audit matter (inventory $21.4B, obligations $95.2B) — https://agentii.ai/v/NVDA/sec169/50
6. Commitments and contingencies ($95.2B, $27B cloud) — https://agentii.ai/v/NVDA/sec169/70
7. Export-control timeline ($4.5B, $60M, H200 25% tariff) — https://agentii.ai/v/NVDA/sec169/10
8. MD&A overview (Blackwell majority, H20, open-source AI) — https://agentii.ai/v/NVDA/sec169/36
9. Segment table (C&N $193.5B, Graphics $22.5B) — https://agentii.ai/v/NVDA/sec169/77
10. Geography + concentration (US $149.6B, Taiwan $42.3B, China $19.7B) — https://agentii.ai/v/NVDA/sec169/78
11. End-market revenue (Data Center $193.7B, Gaming $16.0B, Automotive $2.3B) — https://agentii.ai/v/NVDA/sec169/79
12. Q1 FY2027 income statement ($81.6B revenue, $58.3B net income) — https://agentii.ai/v/NVDA/sec173/3
13. Q1 FY2027 commitments ($119B, $30B cloud) — https://agentii.ai/v/NVDA/sec173/16
14. Market-platform revenue (Data Center $75.2B, Hyperscale $37.9B, Edge $6.4B) — https://agentii.ai/v/NVDA/sec173/21
15. Q1 FY2027 MD&A overview — https://agentii.ai/v/NVDA/sec173/23
16. Concentration of revenue + gross margin (21/17/16%; 74.9% vs 60.5%) — https://agentii.ai/v/NVDA/sec173/27
17. Competition/ASIC + lead times (10-Q risk factors) — https://agentii.ai/v/NVDA/sec173/32
18. Architecture-transition risk (Rubin H2 FY2027) — https://agentii.ai/v/NVDA/sec173/33
19. Taiwan/Korea supply dependence; buyback/dividend — https://agentii.ai/v/NVDA/sec173/38
20. 8-K: H20 license requirement, expected up to $5.5B charge — https://agentii.ai/v/NVDA/sec157/2
21. Manufacturing/foundry partners (TSMC, Samsung, SK Hynix, Micron, Hon Hai, Wistron, Fabrinet) — https://agentii.ai/v/NVDA/sec169/8
22. Competition (AMD, Huawei, Intel, cloud internal teams) — https://agentii.ai/v/NVDA/sec169/9
23. Risk-factor summary list (Item 1A) — https://agentii.ai/v/NVDA/sec169/13
24. Worldwide regulator interest; EU AI Act; state AI laws — https://agentii.ai/v/NVDA/sec169/25

## Verification

| # | Tool | Query | Result | Evidence carried |
|---|---|---|---|---|
| 1 | search_companies | ticker=NVDA | NVIDIA Corp, CIK 0001045810, fiscal YE Feb | ticker resolution |
| 2 | get_ticker_coverage | NVDA | 169 SEC filings; latest 2026-05-09 | corpus freshness |
| 3 | get_company_fiscal_calendar | NVDA | FY2026 Q4 ends 2026-02-28; FY2027 Q1 ends 2026-05-31 | period mapping |
| 4 | search_documents | secondary_labels=other_events_8_01 | 6 risk-event 8-Ks (H20 2025-04-15; IFR 2025-01-17; Oct-2023 IFR; Aug-2022) | 8-K discovery |
| 5 | search_sec_filings | 10-K | sec169 FY2026 (filed 2026-02-25) | primary annual |
| 6 | search_sec_filings | 10-Q | sec173 Q1 FY2027 (filed 2026-05-20) | primary quarterly |
| 7 | search_sec_filings | 8-K 2025-01-01→2026-06-30 | sec157 H20 8-K (2025-04-15) | event filing |
| 8 | list_xbrl_concepts | search=Revenue | Revenues + RevenueFromContractWithCustomer* concepts | concept mapping |
| 9 | search_xbrl_facts | Revenues FY2026 | $215,938M (authority 3); Q1 FY2027 $81,615M (authority 2) | structured revenue |
| 10 | read_source_outline | sec169 | 85-page map; risk pages 13–28, 50, 70, 77–79 | page selection |
| 11 | read_source_outline | sec173 | 41-page map; risk pages 31–38, 16, 21, 23, 27 | page selection |
| 12 | read_source_pages | sec169 p13,15,16,23 | risk summary; lead times; transitions; concentration | Mode 1 core |
| 13 | read_source_pages | sec169 p36,37,50,70 | MD&A; CAM; commitments | Mode 1 core |
| 14 | read_source_pages | sec169 p77,78,79 | segments; geography; end markets | Mode 1 core |
| 15 | read_source_pages | sec173 p31,32,33,34 | 10-Q risk factors (competition, lead times, regulatory) | Mode 1 core |
| 16 | read_source_pages | sec173 p23,27 | MD&A; concentration; GM bridge | Mode 1 core |
| 17 | read_source_pages | sec173 p16,21 | $119B commitments; platform revenue | Mode 1 core |
| 18 | search_keyword_in_source | sec169 keyword=energy | 8 pages incl. 15, 16, 36 | cross-check |
| 19 | read_source_outline | sec157 | 3-page 8-K map; $5.5B expected charge | event evidence |
| 20 | read_source_pages | sec157 p2 | exact 8-K text | event evidence |

Every material number above traces to one of these calls; none is priced-derived (market_data_stage: none).
