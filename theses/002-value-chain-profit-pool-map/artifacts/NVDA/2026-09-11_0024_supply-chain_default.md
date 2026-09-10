---
artifact_id: "002-NVDA-supply-chain-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: NVDA
skill: supply-chain
mode: default
affix: supply-chain-map
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "8cb3ac1de486"
as_of: 2026-09-11
entity_claims:
  - entity: NVDA
    metric: consolidated_gross_margin_pct
    value: 72.7
    unit: pct
    period: FY2024
    source: "10-K:page51"
    retrieved_at: 2026-09-11
  - entity: NVDA
    metric: consolidated_gross_margin_pct
    value: 75.0
    unit: pct
    period: FY2025
    source: "10-K:page51"
    retrieved_at: 2026-09-11
  - entity: NVDA
    metric: consolidated_gross_margin_pct
    value: 71.1
    unit: pct
    period: FY2026
    source: "10-K:page37"
    retrieved_at: 2026-09-11
  - entity: NVDA
    metric: consolidated_gross_margin_pct
    value: 74.9
    unit: pct
    period: 2027Q1
    source: "10-Q:page27"
    retrieved_at: 2026-09-11
  - entity: NVDA
    metric: edge_computing_revenue_usd
    value: 6369000000
    unit: USD
    period: 2027Q1
    source: "10-Q:page21"
    retrieved_at: 2026-09-11
citations:
  - https://agentii.ai/v/NVDA/sec169/8
  - https://agentii.ai/v/NVDA/sec169/10
  - https://agentii.ai/v/NVDA/sec169/37
  - https://agentii.ai/v/NVDA/sec169/41
  - https://agentii.ai/v/NVDA/sec169/50
  - https://agentii.ai/v/NVDA/sec169/51
  - https://agentii.ai/v/NVDA/sec169/70
  - https://agentii.ai/v/NVDA/sec169/78
  - https://agentii.ai/v/NVDA/sec169/79
  - https://agentii.ai/v/NVDA/sec173/16
  - https://agentii.ai/v/NVDA/sec173/20
  - https://agentii.ai/v/NVDA/sec173/21
  - https://agentii.ai/v/NVDA/sec173/25
  - https://agentii.ai/v/NVDA/sec173/27
  - https://agentii.ai/v/NVDA/sec173/38
pillars_addressed: [PIL-1, PIL-2]
claim_state: pinned
key_metrics:
  revenue_fy2026_usd_b: 215.9
  gross_margin_fy2026_pct: 71.1
  gross_margin_fy2025_pct: 75.0
  gross_margin_fy2024_pct: 72.7
  gross_margin_q1fy2027_pct: 74.9
  gross_margin_q1fy2026_pct: 60.5
  gm_change_fy2024_to_fy2026_pp: -1.6
  h20_charge_q1fy2026_usd_b: 4.5
  h20_licensed_revenue_aug2025_usd_m: 60
  h200_import_tariff_pct: 25
  china_revenue_fy2026_usd_b: 19.7
  china_revenue_share_fy2026_pct: 9.1
  china_revenue_share_fy2024_pct: 20.2
  china_revenue_q1fy2027_usd_b: 4.55
  china_revenue_share_q1fy2027_pct: 5.6
  supply_commitments_fy2026_end_usd_b: 95.2
  supply_commitments_apr2026_usd_b: 119
  cloud_commitments_apr2026_usd_b: 30
  inventory_fy2026_end_usd_b: 21.4
  edge_revenue_q1fy2027_usd_b: 6.37
  edge_share_q1fy2027_revenue_pct: 7.8
  data_center_revenue_fy2026_usd_b: 193.7
  top1_direct_customer_share_fy2026_pct: 22
  top2_direct_customer_share_fy2026_pct: 14
  top_direct_customer_shares_q1fy2027_pct: [21, 17, 16]
  nonus_revenue_share_fy2026_pct: 31
  segment_operating_income_margin_fy2026_pct: 64.5
conclusions:
  - "PIL-1: NVDA confirms the compute/model-layer margin anchor (71.1% FY2026 GM, 64.5% segment OI margin); within its own chain, profit concentrates at the bottlenecks NVDA owns or pre-purchases (architecture/IP, CoWoS advanced packaging, HBM capacity) while assembly is outsourced to Hon Hai/Wistron/Fabrinet."
  - "PIL-1b input: NVDA model-layer GM changed -1.6pp over FY2024-FY2026 (72.7% to 71.1%); the motion-minus-model gap falsifier (< -10pp) would require PH motion-layer GM to fall roughly 8.5pp+ over the same window."
  - "PIL-2: NVDA-China is the canonical import-substitution case - $4.5B H20 charge, ~$60M licensed revenue, H200 25% tariff, effective foreclosure from China DC compute; China revenue share fell 20.2% (FY2024) to 9.1% (FY2026) to 5.6% (Q1 FY2027), with Chinese-government procurement steering toward domestic competitors."
  - "Supply-side structure: $95.2B manufacturing/supply/capacity commitments at FY2026-end grew to $119B by Apr 2026 (+$23.8B in one quarter); dependence concentrated in Taiwan (TSMC, CoWoS) and South Korea (HBM)."
  - "Edge platform ($6.37B Q1 FY2027, +29% YoY; robotics/automotive/AI-RAN) is NVDA's direct physical-AI device-economics exposure and the demand-side bridge to the thesis's motion/sensing layers."
facts_count: 53
deducted_count: 14
views_count: 5
citation_count: 15
---

# NVDA Supply-Chain Map — Thesis 002 Value Chain Profit Pool (compute/model layer)

## 1. Executive Summary

NVDA anchors the thesis's compute/model layer: FY2026 revenue $215.9B (+65%) at 71.1% gross margin, GM down 3.9pp on the Hopper-HGX-to-Blackwell transition plus a $4.5B H20 charge [FACT] (https://agentii.ai/v/NVDA/sec169/37). Its fabless supply chain concentrates around bottlenecks — TSMC/Samsung foundries, CoWoS advanced packaging, HBM memory (SK Hynix, Micron, Samsung) — while assembly is outsourced to Hon Hai, Wistron, Fabrinet [FACT] (https://agentii.ai/v/NVDA/sec169/8). Upstream commitments grew from $95.2B at FY2026-end to $119B by Apr 2026 [FACT] (https://agentii.ai/v/NVDA/sec169/70, https://agentii.ai/v/NVDA/sec173/16). Customer concentration is rising: top direct customer 22% of FY2026 revenue vs 13% in FY2024 [FACT] (https://agentii.ai/v/NVDA/sec169/41). China is the PIL-2 import-substitution case: $4.5B H20 inventory/purchase-obligation charge in Q1 FY2026, ~$60M licensed H20 revenue, an H200 license carrying a 25% tariff, and effective foreclosure from China's data-center compute market; China revenue share fell from 20.2% (FY2024) to 9.1% (FY2026) to 5.6% (Q1 FY2027) [FACT] (https://agentii.ai/v/NVDA/sec169/10, https://agentii.ai/v/NVDA/sec169/78, https://agentii.ai/v/NVDA/sec173/20). GM series for the PIL-1b gap test: 72.7% [DEDUCTED] → 75.0% → 71.1% (FY2024–FY2026) [FACT], Q1 FY2027 at 74.9% [FACT] (https://agentii.ai/v/NVDA/sec169/51, https://agentii.ai/v/NVDA/sec173/27). Edge — robotics/automotive/AI-RAN physical-AI platform — ran $6.37B in Q1 FY2027, +29% YoY [FACT] (https://agentii.ai/v/NVDA/sec173/21).

## 2. Data Sources

- **sec169** — NVDA FY2026 Form 10-K, filed 2026-02-25, period ended 2026-01-25; pages read: 8, 10, 37, 41, 50, 51, 70, 78, 79 (via Layer-1 `search_sec_filings` → Layer-2 `read_source_outline` → Layer-3 `read_source_pages`).
- **sec173** — NVDA Q1 FY2027 Form 10-Q, filed 2026-05-20, period ended 2026-04-26; pages read: 16, 20, 21, 25, 27, 38.
- **XBRL** — `search_xbrl_facts` (is_primary; source_authority 3 = 10-K, 2 = 10-Q) for `Revenues`, `GrossProfit` (us-gaap), and `ScheduleOfRevenuesFromExternalCustomersAndLongLivedAssetsByGeographicalAreasTableTextBlock`. Per task note, NVDA tags consolidated `Revenues` (not `RevenueFromContractWithCustomerExcludingAssessedTax`); period alignment by `period_end` (FYE late January).
- **Preflight** — `search_companies` (CIK 0001045810, FYE month 2), `get_ticker_coverage` (169 sec_filings; 40,156 xbrl_facts), `get_company_fiscal_calendar` (FYE February; quarters mapped to `period_end`).

## 3. Analysis

### 3.1 Compute-layer supply chain — foundry / HBM / CoWoS (PIL-1)

- [FACT] NVDA is fabless: wafers from TSMC and Samsung foundries; memory from SK Hynix, Micron, and Samsung; CoWoS technology for semiconductor packaging; final assembly, testing, and packaging via Hon Hai Precision, Wistron, and Fabrinet (https://agentii.ai/v/NVDA/sec169/8).
- [FACT] The supply chain "is mainly concentrated in Asia," with expansion into the U.S. and Latin America to build redundancy (https://agentii.ai/v/NVDA/sec169/8).
- [FACT] NVDA's business "depends on our ability to receive consistent and reliable supply from our overseas partners, especially in Taiwan and South Korea" (https://agentii.ai/v/NVDA/sec173/38).
- [FACT] Long-lived assets: United States $5,125M, Taiwan $3,219M, Israel $1,471M (https://agentii.ai/v/NVDA/sec169/79).
- [FACT] Manufacturing, supply, and capacity commitments: $95.2B as of 2026-01-25, substantially all payable through FY2027 (https://agentii.ai/v/NVDA/sec169/70).
- [FACT] Same commitments at $119B as of 2026-04-26 — $95B payable in remainder of FY2027, balance FY2028–2031 (https://agentii.ai/v/NVDA/sec173/16).
- [DEDUCTED] Commitment growth of $23.8B in a single quarter (119.0 − 95.2).
- [FACT] Multi-year cloud-service commitments: $27B at FY2026-end (https://agentii.ai/v/NVDA/sec169/70); $30B at 2026-04-26 (https://agentii.ai/v/NVDA/sec173/16).
- [FACT] Inventory $21.4B at FY2026-end; PwC's critical audit matter covers inventory valuation and excess purchase commitments (https://agentii.ai/v/NVDA/sec169/50).
- [FACT] Inventory and excess-purchase-obligation provisions: $7.2B FY2026 vs $3.7B FY2025; net gross-margin impact −2.6% vs −2.3% (https://agentii.ai/v/NVDA/sec169/41).
- [DEDUCTED] Segment operating income $139,297M on $215,938M revenue = 64.5% segment operating margin in FY2026 (https://agentii.ai/v/NVDA/sec169/78).
- [VIEW] The compute layer's profit pool concentrates in the bottleneck inputs NVDA controls by design (architecture/IP) or pre-purchases at scale (CoWoS/HBM capacity), not in the outsourced assembly tier — the PIL-1 profit-concentration logic operating inside NVDA's own chain.

### 3.2 Customer concentration

- [FACT] Direct customers: FY2026 one customer = 22% of revenue, another = 14% (Compute & Networking); FY2025: 12%, 11%, 11%; FY2024: 13% (https://agentii.ai/v/NVDA/sec169/41).
- [FACT] Q1 FY2027: three direct customers at 21%, 17%, and 16% of revenue (vs 16% and 14% in Q1 FY2026) (https://agentii.ai/v/NVDA/sec173/20).
- [DEDUCTED] Top-1 direct-customer share rose from 13% (FY2024) to 22% (FY2026).
- [FACT] Indirect customers: some individually represent 10% or more of revenue; one AI research-and-deployment company contributed a "meaningful amount" by purchasing cloud services from NVDA customers in FY2026 and Q1 FY2027 (https://agentii.ai/v/NVDA/sec169/41, https://agentii.ai/v/NVDA/sec173/27).
- [FACT] Revenue from customers headquartered outside the US: 48% (FY2024), 41% (FY2025), 31% (FY2026) (https://agentii.ai/v/NVDA/sec169/78); 22% in Q1 FY2027 (https://agentii.ai/v/NVDA/sec173/20).
- [VIEW] Rising hyperscaler concentration makes the demand side a small set of mega-customers while the supply side binds on Taiwan/South Korea capacity — a squeeze structure at both ends of NVDA's chain.

### 3.3 China exposure — PIL-2 import-substitution case

- [FACT] April 2025: USG imposed a license requirement on H20 exports to China and D:5 countries; NVDA recorded a $4.5B charge in Q1 FY2026 for H20 excess inventory and purchase obligations as demand diminished (https://agentii.ai/v/NVDA/sec169/10).
- [FACT] August 2025: licenses granted for certain H20 shipments; ~$60M H20 revenue generated; USG officials expected ≥15% of licensed-sale revenue, not codified (https://agentii.ai/v/NVDA/sec169/10).
- [FACT] February 2026: license granted for small amounts of H200 to specific China customers; no revenue yet; US pre-shipment inspection required and a 25% tariff applies on importation into the US (https://agentii.ai/v/NVDA/sec169/10).
- [FACT] As of FY2026-end NVDA was "effectively foreclosed from competing in China's data center computing/compute market," which "helped our competitors build larger developer and customer ecosystems" (https://agentii.ai/v/NVDA/sec169/10).
- [FACT] Q1 FY2027: no Data Center Hopper shipments to China, vs $4.6B in Q1 FY2026 (https://agentii.ai/v/NVDA/sec173/25).
- [FACT] China (incl. Hong Kong) revenue by customer HQ: FY2024 $12,330M; FY2025 $25,048M; FY2026 $19,677M (https://agentii.ai/v/NVDA/sec169/78). Q1 FY2027: $4,550M vs $9,659M year-ago (XBRL geographic-areas text block, same filing as https://agentii.ai/v/NVDA/sec173/20).
- [DEDUCTED] China share of revenue: 20.2% (FY2024) → 19.2% (FY2025) → 9.1% (FY2026) → 5.6% (Q1 FY2027).
- [FACT] The Chinese government has encouraged customers to purchase from China-based competitors and issued an Action Plan endorsing accelerator standards (compute-per-watt, per-memory-bandwidth) for new and renovated data centers (https://agentii.ai/v/NVDA/sec173/38).
- [FACT] Gross-margin impact: Q1 FY2026 GM was 60.5% vs 74.9% in Q1 FY2027; net provision impact −11.0% vs −1.2% (https://agentii.ai/v/NVDA/sec173/27).
- [VIEW] NVDA-China is the PIL-2 import-substitution template: export controls converted a ~20% revenue geography into a subsidized competitor ecosystem, and the same dynamic plausibly applies to physical-AI BOMs sourced from China (motion/sensing components) under PIL-2's non-China-to-China cost-ratio falsifier.

### 3.4 Multi-year gross margin — PIL-1b gap-change input

- [FACT] Three-year income statement (period_end aligned): FY2024 revenue $60,922M / gross profit $44,301M; FY2025 $130,497M / $97,858M; FY2026 $215,938M / $153,463M (https://agentii.ai/v/NVDA/sec169/51).
- [DEDUCTED] Computed GM: FY2024 72.7%; FY2025 75.0%; FY2026 71.1%.
- [FACT] Disclosed GM 71.1% FY2026 vs 75.0% FY2025 (−3.9pp), driven by the Hopper HGX → Blackwell full-scale datacenter-solution transition and the $4.5B H20 charge (https://agentii.ai/v/NVDA/sec169/37).
- [FACT] Q1 FY2027 GM 74.9%, approximately flat sequentially, up from 60.5% a year ago on lower inventory provisions (https://agentii.ai/v/NVDA/sec173/27).
- [DEDUCTED] Model-layer GM change FY2024 → FY2026 = −1.6pp (71.1 − 72.7).
- [VIEW] PIL-1b falsifier input (model leg): Δ = −1.6pp over 3 FYs. For the motion-minus-model gap to fall more than 10pp (falsification), PH's motion-layer GM would need to fall roughly 8.5pp or more over the same window; the synthesis computes this against the PH series.

### 3.5 Edge platform — physical-AI adjacency

- [FACT] New market-platform disclosure (Q1 FY2027, recast): Edge Computing $6,369M, +29% YoY, +10% QoQ; comparatives Q4 FY2026 $5,813M and Q1 FY2026 $4,950M (https://agentii.ai/v/NVDA/sec173/21).
- [FACT] Edge "highlights devices for agentic and physical AI including PCs, game consoles, workstations, AI-RAN base stations, robotics and automotive" (https://agentii.ai/v/NVDA/sec173/25).
- [FACT] Growth driven by robust Blackwell workstation demand, partially offset by slower consumer PC demand tempered by elevated memory and system prices (https://agentii.ai/v/NVDA/sec173/25).
- [DEDUCTED] Edge = 7.8% of Q1 FY2027 revenue (6,369 / 81,615).
- [VIEW] Edge is NVDA's direct physical-AI device-economics exposure (robotics + automotive), the demand-side bridge to the thesis's motion/sensing layers.

## 4. Key Metrics

| Metric | FY2024 | FY2025 | FY2026 | Q1 FY2027 | Source |
|---|---|---|---|---|---|
| Revenue ($B) | 60.9 | 130.5 | 215.9 | 81.6 | [FACT] /v/NVDA/sec169/51 |
| Gross profit ($B) | 44.3 | 97.9 | 153.5 | 61.2 | [FACT] /v/NVDA/sec169/51 |
| Gross margin (%) | 72.7 [DEDUCTED] | 75.0 [FACT] | 71.1 [FACT] | 74.9 [FACT] | /v/NVDA/sec169/37, /v/NVDA/sec173/27 |
| GM change FY2024→FY2026 | — | — | −1.6pp [DEDUCTED] | — | — |
| China (incl. HK) revenue ($B) | 12.3 | 25.0 | 19.7 | 4.55 | [FACT] /v/NVDA/sec169/78, /v/NVDA/sec173/20 |
| China share of revenue (%) | 20.2 [DEDUCTED] | 19.2 [DEDUCTED] | 9.1 [DEDUCTED] | 5.6 [DEDUCTED] | — |
| Top direct customer (% of revenue) | 13 [FACT] | 12 [FACT] | 22 [FACT] | 21 [FACT] | /v/NVDA/sec169/41, /v/NVDA/sec173/20 |
| Supply/capacity commitments ($B) | — | — | 95.2 (2026-01-25) | 119 (2026-04-26) | [FACT] /v/NVDA/sec169/70, /v/NVDA/sec173/16 |
| Cloud commitments ($B) | — | — | 27 | 30 | [FACT] /v/NVDA/sec169/70, /v/NVDA/sec173/16 |
| H20 charge ($B) | — | — | 4.5 (Q1 FY2026) | — | [FACT] /v/NVDA/sec169/10 |
| Edge Computing revenue ($B) | — | — | 5.8 (Q4 FY2026, recast) | 6.37 (+29% YoY) | [FACT] /v/NVDA/sec173/21 |
| Data Center revenue ($B) | 47.5 | 115.2 | 193.7 | 75.2 | [FACT] /v/NVDA/sec169/79, /v/NVDA/sec173/21 |

## 5. Coverage Gaps & Citations

**Coverage gaps**
- Customer and supplier names are not disclosed in filings (standard practice); only concentration percentages.
- No quantified supplier-concentration percentages (e.g., TSMC share of wafers, HBM volume) — narrative only.
- China revenue is not split by product beyond the H20/H200 narrative.
- No teardown/BOM data retrieved; teardown figures would be [VIEW]-only per falsifier spec and none are used.
- No price data used (mandate).
- FY2025 10-K (sec154) not re-read; the FY2026 10-K supplies the recast 3-year China series, FY2024 GM line, and the H20 charge.

**Citations (roll-up index — non-duplicative)**
1. https://agentii.ai/v/NVDA/sec169/8 — fabless manufacturing, TSMC/Samsung, CoWoS, memory suppliers, contract manufacturers
2. https://agentii.ai/v/NVDA/sec169/10 — H20 $4.5B charge, ~$60M licensed revenue, H200 25% tariff, China foreclosure
3. https://agentii.ai/v/NVDA/sec169/37 — FY2026 summary: GM 71.1% vs 75.0%, −3.9pp, drivers
4. https://agentii.ai/v/NVDA/sec169/41 — customer concentration + provisions ($7.2B/$3.7B)
5. https://agentii.ai/v/NVDA/sec169/50 — inventory $21.4B, $95.2B obligations (CAM)
6. https://agentii.ai/v/NVDA/sec169/51 — 3-year income statement (GM series basis)
7. https://agentii.ai/v/NVDA/sec169/70 — commitments $95.2B, cloud $27B
8. https://agentii.ai/v/NVDA/sec169/78 — geographic revenue + direct-customer concentration
9. https://agentii.ai/v/NVDA/sec169/79 — end markets, long-lived assets
10. https://agentii.ai/v/NVDA/sec173/16 — commitments $119B, cloud $30B
11. https://agentii.ai/v/NVDA/sec173/20 — Q1 FY2027 concentration (21/17/16), non-US 22%
12. https://agentii.ai/v/NVDA/sec173/21 — Edge $6,369M platform table
13. https://agentii.ai/v/NVDA/sec173/25 — Edge +29%, no China Hopper shipments vs $4.6B
14. https://agentii.ai/v/NVDA/sec173/27 — GM 74.9% vs 60.5%, provision impact −11.0%/−1.2%
15. https://agentii.ai/v/NVDA/sec173/38 — Taiwan/South Korea supply dependency, China government procurement steering

## 6. Verification (T-001 baseline reconciliation)

| T-001 baseline | Retrieved this run | Status | Source |
|---|---|---|---|
| FY2026 revenue $215.9B | $215,938M | MATCH | [FACT] /v/NVDA/sec169/37, /v/NVDA/sec169/51 |
| FY2026 GM 71.1% | 71.1% | MATCH | [FACT] /v/NVDA/sec169/37 |
| Supply commitments $119B | $119B as of 2026-04-26 (Q1 FY2027 10-Q); $95.2B at FY2026 year-end (10-K) | MATCH with period note — the $119B baseline is the 10-Q figure, not the 10-K year-end | [FACT] /v/NVDA/sec173/16, /v/NVDA/sec169/70 |
| Edge $6.4B | $6,369M Q1 FY2027 | MATCH | [FACT] /v/NVDA/sec173/21 |

Audit: every number above was retrieved in this run via agentii MCP tools (`search_xbrl_facts`, `read_source_pages`) and carries an inline `https://agentii.ai/v/NVDA/{citation_id}/{page}` citation. No price data used. Uncited numbers are void.
