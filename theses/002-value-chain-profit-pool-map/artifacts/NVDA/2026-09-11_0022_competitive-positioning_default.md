---
artifact_id: "002-NVDA-competitive-positioning-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: NVDA
skill: competitive-positioning
mode: default
affix: competitive-structure
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "61f794be22a5"
as_of: 2026-09-11
entity_claims:
  - entity: NVDA
    metric: consolidated_gross_margin_pct
    value: 75.0
    unit: pct
    period: FY2025
    source: "10-K:page41"
    retrieved_at: 2026-09-11
  - entity: NVDA
    metric: consolidated_gross_margin_pct
    value: 71.1
    unit: pct
    period: FY2026
    source: "10-K:page41"
    retrieved_at: 2026-09-11
  - entity: NVDA
    metric: consolidated_gross_margin_pct
    value: 74.9
    unit: pct
    period: Q1-FY2027
    source: "10-Q:page24"
    retrieved_at: 2026-09-11
  - entity: NVDA
    metric: edge_computing_revenue_usd
    value: 6369000000
    unit: USD
    period: Q1-FY2027
    source: "10-Q:page25"
    retrieved_at: 2026-09-11
citations:
  - "https://agentii.ai/v/NVDA/sec173/24"
  - "https://agentii.ai/v/NVDA/sec173/25"
  - "https://agentii.ai/v/NVDA/sec173/27"
  - "https://agentii.ai/v/NVDA/sec173/20"
  - "https://agentii.ai/v/NVDA/sec173/19"
  - "https://agentii.ai/v/NVDA/sec173/32"
  - "https://agentii.ai/v/NVDA/sec173/35"
  - "https://agentii.ai/v/NVDA/sec173/16"
  - "https://agentii.ai/v/NVDA/sec169/10"
  - "https://agentii.ai/v/NVDA/sec169/26"
  - "https://agentii.ai/v/NVDA/sec169/36"
  - "https://agentii.ai/v/NVDA/sec169/41"
  - "https://agentii.ai/v/NVDA/sec169/78"
  - "https://agentii.ai/v/NVDA/sec169/4"
  - "https://agentii.ai/v/NVDA/sec169/6"
  - "https://agentii.ai/v/NVDA/sec169/8"
pillars_addressed: [PIL-1, PIL-2]
claim_state: pinned
key_metrics:
  consolidated_gross_margin_pct_FY2025: 75.0
  consolidated_gross_margin_pct_FY2026: 71.1
  consolidated_gross_margin_pct_Q1-FY2027: 74.9
  edge_computing_revenue_usd_Q1-FY2027: 6369000000
  data_center_revenue_usd_Q1-FY2027: 75246000000
  hyperscale_revenue_usd_Q1-FY2027: 37869000000
  acie_revenue_usd_Q1-FY2027: 37377000000
  total_revenue_usd_FY2026: 215938000000
  total_revenue_usd_Q1-FY2027: 81615000000
  china_revenue_usd_FY2025: 25048000000
  china_revenue_usd_FY2026: 19677000000
  china_revenue_usd_Q1-FY2027: 4550000000
  china_revenue_share_pct_FY2025: 19.2
  china_revenue_share_pct_FY2026: 9.1
  china_revenue_share_pct_Q1-FY2027: 5.6
  h20_inventory_charge_usd_Q1-FY2026: 4500000000
  h20_licensed_revenue_usd_FY2026: 60000000
  inventory_provision_net_gm_impact_pct_Q1-FY2027: 1.2
  inventory_provision_net_gm_impact_pct_FY2026: 2.6
  customer_concentration_top3_pct_Q1-FY2027: 54
  cumulative_rd_usd: 76700000000
  rd_expense_usd_FY2026: 18497000000
conclusions:
  - "NVDA compute-layer moat (CUDA ecosystem, cadence, platform co-design) is intact; FY2026 GM dip to 71.1% was Hopper-to-Blackwell mix transition plus a one-off $4.5B H20 charge, not competitive erosion — GM recovered to 74.9% in Q1 FY2027."
  - "China is structurally lost as a data-center compute market: NVDA states it is 'effectively foreclosed', China revenue share fell from 19.2% (FY2025) to 5.6% (Q1 FY2027), and the company admits the foreclosure is feeding competitor ecosystems globally."
  - "Export controls — not customer ASICs — are the principal substitution risk to the compute-layer moat; ASIC development by customers is disclosed as a real but slower-moving threat."
  - "Pricing power evidence is strong: 74.9% GM with demand-constrained supply, non-cancellable purchase orders, and stated pricing stability against short-term cost moves."
facts_count: 28
deducted_count: 5
views_count: 6
citation_count: 59
---

# Competitive Positioning — NVDA (PIL-1: compute-layer barriers; PIL-2: China dynamics)

Thesis 002 — Value Chain Profit Pool Map | Skill: competitive-positioning | Mode: default
As of 2026-09-11. FY2026 = fiscal year ended 2026-01-25; Q1-FY2027 = quarter ended 2026-04-26.

## Executive Summary

NVDA's competitive position at the compute layer of the physical-AI value chain rests on a software-gated platform moat: CUDA plus hundreds of domain libraries, $76.7B of cumulative R&D, and a one-year silicon cadence (Blackwell → GB300 → Rubin) that rivals cannot match on pace alone. Pricing power is demonstrated: gross margin of 74.9% in Q1-FY2027, restored to the FY2025 level after the FY2026 dip to 71.1% — which NVDA attributes to the Hopper→Blackwell system mix shift plus a one-off $4.5B H20 inventory charge, not competitive price pressure. The dominant structural threat is substitution via export controls, not ASICs: NVDA states it is "effectively foreclosed" from China's data-center market, China revenue share collapsed from 19.2% (FY2025) to 5.6% (Q1-FY2027), and the company concedes the foreclosure is feeding competitor developer ecosystems worldwide. Customer-ASIC development is disclosed as a real, slower-moving threat. For thesis 002, NVDA's compute-layer margins anchor the top of the profit pool; the main falsifier exposure is long-horizon ecosystem leakage from export controls and open-source models, not near-term margin compression.

## Data Sources

- Q1-FY2027 10-Q (filed 2026-05-20, report 2026-04-26) — citation_id `sec173`, accession 0001045810-26-000052
- FY2026 10-K (filed 2026-02-25, report 2026-01-25) — citation_id `sec169`, accession 0001045810-26-000021
- XBRL facts (us-gaap:GrossProfit, us-gaap:Revenues, geographic revenue text blocks), FY2025–Q1-FY2027, is_primary only
- Preflight: gold.companies (NVDA, CIK 0001045810, FY end month 2), fiscal calendar, coverage (sec_filings 169 records, xbrl_facts 40,156, transcripts 17 through 2026-05-20)

## Analysis

### A. Competitive structure of the AI-compute layer (PIL-1)

[FACT] NVIDIA discloses its principal competitive factors as performance, breadth of product offerings, access to customers/partners/distribution channels, software support, conformity to industry-standard APIs, manufacturing capabilities, processor pricing, and total system cost (https://agentii.ai/v/NVDA/sec169/8).

[FACT] The platform's demand-side anchor: "All major cloud service providers, or CSPs, AI model makers, and enterprises use our data center-scale infrastructure and computing platforms" (https://agentii.ai/v/NVDA/sec169/4).

[FACT] Compute & Networking revenue was $74,550M (+88% YoY) and Graphics $7,065M (+58% YoY) in Q1-FY2027, with segment operating income of $53,335M and $2,941M respectively (https://agentii.ai/v/NVDA/sec173/19). [DEDUCTED] Compute & Networking is 91.3% of total revenue — the AI-compute layer dominates the business.

[FACT] FY2026 segment operating income was $139,297M on total revenue of $215,938M, against $87,960M in FY2025 (https://agentii.ai/v/NVDA/sec169/78).

[FACT] Buyer structure: three direct customers were 21%, 17%, and 16% of Q1-FY2027 revenue (https://agentii.ai/v/NVDA/sec173/20), up from one at 22% and another at 14% in FY2026 (https://agentii.ai/v/NVDA/sec169/78). [DEDUCTED] Top-three direct-customer concentration is 54% in Q1-FY2027. [VIEW] Concentrated hyperscaler buyers are the main counterweight to the moat — but concentration rising while GM is rising suggests demand-side lock-in currently outweighs buyer power.

[FACT] NVIDIA does not disclose market share of the AI-compute layer; share proxies are limited to segment revenue, customer breadth statements, and cadence. Coverage gap — see section E.

### B. Moat sources (PIL-1)

[FACT] The technology stack is anchored by "the foundational NVIDIA CUDA development platform that runs on all NVIDIA GPUs, as well as hundreds of domain-specific software libraries, frameworks, algorithms, SDKs, and APIs" (https://agentii.ai/v/NVDA/sec169/4).

[FACT] Platform strategy: a "unified underlying programmable architecture" addresses multiple multi-billion-dollar end markets, and "the large and growing number of developers and installed base across our platforms strengthens our ecosystem and increases the value of our platform for our customers" — an explicit network-effect claim (https://agentii.ai/v/NVDA/sec169/4).

[FACT] Innovation scale: "over $76.7 billion in research and development since our inception" and "more than half of our engineers work on software" (https://agentii.ai/v/NVDA/sec169/4). FY2026 R&D spend was $18,497M, +43% YoY (https://agentii.ai/v/NVDA/sec169/41); Q1-FY2027 R&D was $6,321M, +58% YoY, with compute/infrastructure spend up 112% (https://agentii.ai/v/NVDA/sec173/27).

[FACT] Cadence moat: "one-year product cadence, including our Rubin platform"; GB300/Blackwell Ultra shipped from Q2-FY2026; Rubin production shipments expected H2-FY2027, with "up to a 10x reduction in cost per token compared to Blackwell" (https://agentii.ai/v/NVDA/sec169/36; https://agentii.ai/v/NVDA/sec169/6). Blackwell "represented the majority of our Data Center revenue" in FY2026 (https://agentii.ai/v/NVDA/sec169/36) and remained the majority of system shipments in Q1-FY2027 (https://agentii.ai/v/NVDA/sec173/24).

[FACT] Co-design moat: data-center-scale offerings feature "extreme co-design where the infrastructure's chips, networking, systems, software, and algorithms are holistically architected"; "hundreds of thousands of GPUs can be interconnected to function as a single giant computer" (https://agentii.ai/v/NVDA/sec169/4). Ecosystem investments continue: $18.6B in private companies and infrastructure funds in Q1-FY2027 alone (https://agentii.ai/v/NVDA/sec173/24).

[FACT] Supply lock-in: manufacturing and capacity commitments of ~$119B, predominantly due in FY2027, plus ~$30B of multi-year cloud service agreements (https://agentii.ai/v/NVDA/sec173/16).

[VIEW] The moat is a software-plus-cadence flywheel: CUDA's installed developer base raises switching costs, while the one-year cadence denies rivals a technology window. Nothing in the retrieved filings contradicts this for ex-China markets.

### C. Pricing power evidence — margin trajectory (PIL-1)

[FACT] Consolidated gross margin: 75.0% FY2025 → 71.1% FY2026 → 74.9% Q1-FY2027 (https://agentii.ai/v/NVDA/sec169/41; https://agentii.ai/v/NVDA/sec173/24). Q1-FY2027 GM was approximately flat sequentially vs 75.0% (https://agentii.ai/v/NVDA/sec173/24).

[FACT] The FY2026 decline was structural-mix plus one-off, not competitive: "Gross margins decreased to 71.1% in fiscal year 2026 from 75.0% in fiscal year 2025 as our business model transitioned from offering Hopper HGX systems to Blackwell full-scale datacenter solutions and a $4.5 billion charge associated with H20 excess inventory and purchase obligations" (https://agentii.ai/v/NVDA/sec169/41).

[FACT] Inventory-provision burden is normalizing: gross provisions of $7.2B in FY2026 (incl. the $4.5B H20 charge) vs $1.1B in Q1-FY2027; net gross-margin impact improved from 2.6pp unfavorable (FY2026) to 1.2pp unfavorable (Q1-FY2027) (https://agentii.ai/v/NVDA/sec169/41; https://agentii.ai/v/NVDA/sec173/27). [DEDUCTED] Q1-FY2027 gross margin excluding the inventory-provision drag was ≈76.1% (74.9% + 1.2pp) — above the FY2025 level.

[FACT] Pricing-power statement: "Our product and solution pricing generally does not fluctuate with short-term changes in our costs" (https://agentii.ai/v/NVDA/sec173/24).

[FACT] Supply-demand posture favors the seller: manufacturing lead times have extended beyond 12 months; NVIDIA has paid premiums and deposits and holds non-cancellable purchase orders placed in advance of historical lead times (https://agentii.ai/v/NVDA/sec173/32).

[VIEW] A 74.9% gross margin on $81.6B quarterly revenue in a demand-constrained, allocation-style market is the strongest available quantitative evidence of compute-layer pricing power; the 71.1% FY2026 trough is attributable to self-inflicted mix transition and the China-driven H20 write-down, and it has already fully recovered.

### D. Substitution threats — ASICs, custom silicon, open source (PIL-1)

[FACT] NVIDIA discloses direct substitution risk from customer silicon: "Some of our customers are developing their own ASICs and other products, including designs optimized for certain workloads that may not require all of the features and functionality our data center systems provide. Others may offer cloud-based services that compete with our AI cloud service offerings" (https://agentii.ai/v/NVDA/sec173/32).

[FACT] Competitive resource asymmetry is disclosed: some competitors "operate their own fabrication facilities, and have longer operating histories, larger customer bases, more comprehensive IP portfolios and patent protections, more design wins, and greater financial, sales, marketing and distribution resources than we do" (https://agentii.ai/v/NVDA/sec173/32).

[FACT] Open-source models are framed as a demand-side substitution channel: "Open-source AI is dependent on developer adoption, and if deployed on our competitors' platforms, it could reduce demand for our products and services" (https://agentii.ai/v/NVDA/sec173/24).

[FACT] NVIDIA's fabless structure concentrates manufacturing risk: foundries TSMC and Samsung; memory from SK Hynix, Micron, Samsung; CoWoS packaging; contract manufacturers Hon Hai, Wistron, Fabrinet (https://agentii.ai/v/NVDA/sec169/8). Supply chain is being diversified into the US and Latin America (https://agentii.ai/v/NVDA/sec169/36).

[FACT] Export-control-driven substitution is the disclosed systemic threat: NVIDIA states its China-market foreclosure "helped our competitors build larger developer and customer ecosystems to challenge us worldwide" (https://agentii.ai/v/NVDA/sec169/10).

[VIEW] The ASIC threat is real but bounded: customer ASICs optimize narrow workloads and lack the full-stack ecosystem; NVIDIA's own risk-factor language ranks export-control-enabled ecosystem leakage as the material long-term moat risk.

### E. China competitive dynamics (PIL-2)

[FACT] Regulatory timeline (https://agentii.ai/v/NVDA/sec169/10): August 2022 controls (A100/H100); October 2023 performance-threshold licensing (A800/H800/GB200/B200); April 2025 H20 license requirement; August 2025 H20 licenses granted; February 2026 H200 license with pre-shipment US inspection and 25% US import tariff; January 2025 AI Diffusion IFR (rescission announced May 2025, replacement rule pending); October 2025 GAIN AI Act passed by the Senate in the NDAA.

[FACT] The H20 case in numbers: $4.5B charge in Q1-FY2026 for H20 excess inventory and purchase obligations (https://agentii.ai/v/NVDA/sec169/10); ≈$60M of licensed H20 revenue in FY2026 (https://agentii.ai/v/NVDA/sec169/10); zero H200 revenue to date under the February 2026 license (https://agentii.ai/v/NVDA/sec173/24). USG officials expressed an expectation that the USG receives "15% or more of the revenue generated from licensed sales" — a de-facto revenue tax on licensed China sales (https://agentii.ai/v/NVDA/sec169/10).

[FACT] Foreclosure admission: "As of the end of fiscal year 2026, we were effectively foreclosed from competing in China's data center computing/compute market"; NVIDIA is "unable to create and deliver a competitive product for China's data center market that receives approval from both the USG and the Chinese government" (https://agentii.ai/v/NVDA/sec169/10).

[FACT] Shipment evidence of domestic substitution: "No shipments of Data Center Hopper products to China occurred during the quarter [Q1-FY2027], compared with $4.6 billion in the first quarter of fiscal year 2026" (https://agentii.ai/v/NVDA/sec173/25).

[FACT] China revenue trajectory (customer-headquarters basis): FY2025 $25,048M → FY2026 $19,677M → Q1-FY2027 $4,550M (https://agentii.ai/v/NVDA/sec169/78; Q1-FY2027 geographic disclosure in sec173, XBRL is_primary fact, see Verification table). Q1-FY2026 (recast) China revenue was $9,659M (sec173 XBRL text block). [DEDUCTED] China revenue share: 19.2% (FY2025) → 9.1% (FY2026) → 5.6% (Q1-FY2027); Q1-FY2027 China revenue fell ~53% YoY on the recast base.

[FACT] China is applying reciprocal pressure: on September 15, 2025, China's antitrust regulator published a preliminary finding that NVIDIA's export-control compliance (degraded products for the China market) "discriminated unfairly against customers in the China market and therefore violated the terms of China's approval of our Mellanox acquisition"; remedies could include "restrictions or other orders regarding our networking business" (https://agentii.ai/v/NVDA/sec169/26).

[FACT] Overall non-US exposure shrank sharply: revenue from customers headquartered outside the US was 31% in FY2026 vs 41% in FY2025 (https://agentii.ai/v/NVDA/sec169/41), and 22% in Q1-FY2027 vs 42% in Q1-FY2026 (https://agentii.ai/v/NVDA/sec173/20). Taiwan-headquartered revenue was $42,345M in FY2026, of which NVIDIA estimates 76% of Data Center revenue was attributed to end customers in the US and Europe (https://agentii.ai/v/NVDA/sec169/78).

[VIEW] For thesis 002's PIL-2 test (non-China vs China humanoid-BOM cost ratio), the NVDA-side implication is that China's compute layer is being served by domestic silicon — from NVDA's P&L, China demand is no longer a material revenue pool (5.6% share and falling), so any China-side cost advantage rests on non-NVDA compute stacks.

[VIEW] The 15% USG revenue-share expectation structurally caps the economics of any future licensed re-entry into China and signals that export control is now a persistent architecture of the AI-compute layer, not a temporary shock.

## Key Metrics

| Metric | Value | Period | Source |
|---|---|---|---|
| Consolidated gross margin | 75.0% | FY2025 | https://agentii.ai/v/NVDA/sec169/41 |
| Consolidated gross margin | 71.1% | FY2026 | https://agentii.ai/v/NVDA/sec169/41 |
| Consolidated gross margin | 74.9% | Q1-FY2027 | https://agentii.ai/v/NVDA/sec173/24 |
| Total revenue | $215,938M | FY2026 | https://agentii.ai/v/NVDA/sec169/78 |
| Total revenue | $81,615M (+85% YoY) | Q1-FY2027 | https://agentii.ai/v/NVDA/sec173/24 |
| Data Center revenue | $75,246M (+92% YoY) | Q1-FY2027 | https://agentii.ai/v/NVDA/sec173/25 |
| Edge Computing revenue | $6,369M (+29% YoY) | Q1-FY2027 | https://agentii.ai/v/NVDA/sec173/25 |
| Compute & Networking segment op income | $53,335M | Q1-FY2027 | https://agentii.ai/v/NVDA/sec173/19 |
| China revenue | $25,048M → $19,677M → $4,550M | FY2025 → FY2026 → Q1-FY2027 | https://agentii.ai/v/NVDA/sec169/78; sec173 XBRL |
| China revenue share [DEDUCTED] | 19.2% → 9.1% → 5.6% | FY2025 → FY2026 → Q1-FY2027 | arithmetic on above |
| H20 charge | $4,500M | Q1-FY2026 | https://agentii.ai/v/NVDA/sec169/10 |
| Licensed H20 revenue | ≈$60M | FY2026 | https://agentii.ai/v/NVDA/sec169/10 |
| China Hopper shipments | $4,600M → $0 | Q1-FY2026 → Q1-FY2027 | https://agentii.ai/v/NVDA/sec173/25 |
| Top-3 direct customers [DEDUCTED] | 54% of revenue | Q1-FY2027 | https://agentii.ai/v/NVDA/sec173/20 |
| Cumulative R&D | >$76.7B | inception | https://agentii.ai/v/NVDA/sec169/4 |
| Manufacturing commitments | ≈$119B | due predominantly FY2027 | https://agentii.ai/v/NVDA/sec173/16 |

## Coverage Gaps & Citations

Coverage gaps:
1. **Market share of the AI-compute layer**: NVIDIA does not disclose share; no third-party share data retrievable within the skill's tool allowlist. Share is proxied by segment revenue, customer-breadth statements, and cadence.
2. **China domestic-vendor substitution**: no quantitative data on Huawei Ascend or other domestic Chinese compute in NVDA filings; substitution is evidenced only by NVDA's own zero-shipment disclosure and foreclosure language.
3. **Q2-FY2027 10-Q** (quarter ended 2026-07-26) not yet in the corpus: latest indexed 10-Q is sec173 (filed 2026-05-20); coverage latest_data_date for sec_filings is 2026-05-09, transcripts through 2026-05-20. Freshness flagged `missing` tier in coverage.
4. **Peer filings** (AMD, AVGO, TSM) not retrieved — chain scope is single-ticker (NVDA × competitive-positioning × default).
5. **Earnings-call transcripts** (17 records through 2026-05-20) not used in this run — available for a follow-up on H200 licensing commentary.
6. **H200 China license outcome**: pending — zero revenue to date per filing; import approval into China unknown.
7. XBRL-verified values (GrossProfit/Revenues) carry no page-level /v/ anchor; they reconcile to the filing-stated percentages (see Verification table) and are attributed to the source filings sec169/sec173.

Citations index (unique /v/ links used above): sec173 pages 16, 19, 20, 24, 25, 27, 32, 35; sec169 pages 4, 6, 8, 10, 26, 36, 41, 78.

## Verification

| # | Claim | Value | Filing-stated source | XBRL cross-check (retrieval call) | Status |
|---|---|---|---|---|---|
| 1 | FY2026 gross margin | 71.1% | 10-K page41 (sec169) | GrossProfit $153,463M ÷ Revenues $215,938M = 71.07% (us-gaap, is_primary, source_authority 3) | PASS |
| 2 | FY2025 gross margin | 75.0% | 10-K page41 (sec169) | GrossProfit $97,858M ÷ Revenues $130,497M = 74.99% | PASS |
| 3 | Q1-FY2027 gross margin | 74.9% | 10-Q page24 (sec173) | GrossProfit $61,157M ÷ Revenues $81,615M = 74.94% | PASS |
| 4 | Q1-FY2027 China revenue | $4,550M | 10-Q geographic text block (sec173, XBRL is_primary fact; HQ basis) | Revenues $81,615M reconciles to table total | PASS |
| 5 | FY2026 China revenue | $19,677M | 10-K page78 (sec169) | Same value in sec169 geographic XBRL text block | PASS |
| 6 | Q1-FY2026 recast China revenue | $9,659M | sec173 XBRL text block (HQ basis) | Consistent with 22%→42% outside-US shift on page20 | PASS |
| 7 | Edge Computing revenue Q1-FY2027 | $6,369M | 10-Q page25 (sec173) | Market-platform table stated in MD&A; no separate XBRL dimension | PASS (single source) |
| 8 | Q3-FY2026 gross margin (trend context) | 73.4% | — | GrossProfit $41,849M ÷ Revenues $57,006M (sec164 facts) | PASS (XBRL only) |
