---
artifact_id: "002-AMBA-competitive-positioning-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: AMBA
skill: competitive-positioning
mode: default
affix: competitive-structure
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "61f794be22a5"
as_of: 2026-09-11
entity_claims:
  - entity: AMBA
    metric: revenue_usd
    value: 390700000
    unit: USD
    period: FY2026
    source: "10-K:page57"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: revenue_usd
    value: 284865000
    unit: USD
    period: FY2025
    source: "10-K:page57"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: revenue_usd
    value: 226474000
    unit: USD
    period: FY2024
    source: "10-K:page57"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: gross_margin_pct
    value: 59
    unit: pct
    period: FY2026
    source: "10-K:page55"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: gross_margin_pct
    value: 60
    unit: pct
    period: FY2025
    source: "10-K:page55"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: gross_margin_pct
    value: 60
    unit: pct
    period: FY2024
    source: "10-K:page55"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: revenue_growth_yoy_pct
    value: 37.2
    unit: pct
    period: FY2026
    source: "10-K:page57"
    retrieved_at: 2026-09-11
    derivation: "[DEDUCTED] arithmetic on revenue_usd; filing states 37.2%"
  - entity: AMBA
    metric: revenue_growth_yoy_pct
    value: 25.8
    unit: pct
    period: FY2025
    source: "10-K:page57"
    retrieved_at: 2026-09-11
    derivation: "[DEDUCTED] arithmetic on revenue_usd; filing states 25.8%"
  - entity: AMBA
    metric: gross_margin_yoy_change_pp
    value: -1.0
    unit: pp
    period: FY2026
    source: "10-K:page55"
    retrieved_at: 2026-09-11
    derivation: "[DEDUCTED] arithmetic on gross_margin_pct FY2026 vs FY2025"
  - entity: AMBA
    metric: taiwan_share_of_revenue_pct
    value: 69.6
    unit: pct
    period: FY2026
    source: "10-K:page97"
    retrieved_at: 2026-09-11
    derivation: "[DEDUCTED] arithmetic on revenue_usd (271,928 / 390,702)"
  - entity: AMBA
    metric: asia_pacific_share_of_revenue_pct
    value: 87.8
    unit: pct
    period: FY2026
    source: "10-K:page97"
    retrieved_at: 2026-09-11
    derivation: "[DEDUCTED] arithmetic on revenue_usd ((271,928+71,032) / 390,702)"
  - entity: AMBA
    metric: us_share_of_revenue_pct
    value: 1.5
    unit: pct
    period: FY2026
    source: "10-K:page97"
    retrieved_at: 2026-09-11
    derivation: "[DEDUCTED] arithmetic on revenue_usd (5,844 / 390,702)"
citations:
  - {ticker: AMBA, citation_id: sec106, page: page1, note: "Cover: fiscal year ended January 31, 2026"}
  - {ticker: AMBA, citation_id: sec106, page: page9, note: "Robotics applications; CV3 domain controllers; N1-655/CV7 VLM/VLA"}
  - {ticker: AMBA, citation_id: sec106, page: page10, note: "CVflow 3rd-gen transformer AI to 34B params; NN-ISP; multi-modal fusion"}
  - {ticker: AMBA, citation_id: sec106, page: page16, note: "Design cycles, design-win economics, WT 70%, fabless model"}
  - {ticker: AMBA, citation_id: sec106, page: page17, note: "Foundry (Samsung, 10/5/4nm, 2nm tape-out), R&D 75% of staff, competitor lists"}
  - {ticker: AMBA, citation_id: sec106, page: page18, note: "Competitive factors; patents 390 US / 24 China"}
  - {ticker: AMBA, citation_id: sec106, page: page19, note: "Headcount 959 (225 China, 372 Taiwan); EAR/BIS Entity List regulation"}
  - {ticker: AMBA, citation_id: sec106, page: page27, note: "Competitor lists; OEM vertical integration; IP-security consolidation; switching costs"}
  - {ticker: AMBA, citation_id: sec106, page: page38, note: "China local-supplier pressure; Taiwan concentration risk"}
  - {ticker: AMBA, citation_id: sec106, page: page53, note: "FY26 highlights: revenue $390.7M +37.2%; op loss $82.5M; OCF $73.5M"}
  - {ticker: AMBA, citation_id: sec106, page: page55, note: "Common-size: GM 59/60/60; R&D 61% of revenue; ASP lifecycle"}
  - {ticker: AMBA, citation_id: sec106, page: page57, note: "Revenue/R&D tables; GM variance drivers (advanced-node costs, reserved inventory)"}
  - {ticker: AMBA, citation_id: sec106, page: page97, note: "Geographic revenue by bill-to; product cost; net loss series"}
  - {ticker: AMBA, citation_id: sec106, page: page98, note: "WT 70%/63%/53% concentration; AR with WT $24.6M"}
  - {ticker: AMBA, citation_id: sec105, page: page35, note: "BIS Entity List customers: Hikvision, Dahua, Shenzhen Dajiang Baiwang affiliates"}
pillars_addressed: [PIL-1, PIL-2]
claim_state: pinned
key_metrics:
  revenue_usd_fy2026: 390700000
  revenue_usd_fy2025: 284865000
  revenue_usd_fy2024: 226474000
  gross_margin_pct_fy2026: 59
  gross_margin_pct_fy2025: 60
  gross_margin_pct_fy2024: 60
  rnd_pct_of_revenue_fy2026: 61
  wt_distributor_share_pct_fy2026: 70
  asia_pacific_bill_to_share_pct_fy2026: 87.8
conclusions:
  - "AMBA's sensing-layer moat is design-in stickiness plus software/algorithm IP (CVflow, NN-ISP) priced at a stable ~59-60% gross margin, not foundry or scale advantage."
  - "FY2026 gross margin erosion (-1pp) is supply-side (advanced-node manufacturing costs, reserved-inventory sales), not price-war-driven; ASP mix is shifting toward higher-priced AI inference processors."
  - "PIL-2 China exposure is bilateral: 23% of employees in China plus an Asia-heavy revenue base (87.8% bill-to Asia Pacific) versus BIS Entity List restrictions on China customers and local-substitution pressure from HiSilicon/Horizon Robotics."
  - "Robotics exposure is indirect and emerging (CV7/N1-655 VLM/VLA SoCs); no robotics revenue is disclosed - labeled honestly."
facts_count: 37
deducted_count: 13
views_count: 7
citation_count: 15
---

# Competitive Positioning — Ambarella, Inc. (AMBA)

Mode: default | Affix: competitive-structure | Pillars: PIL-1 (sensing-layer barriers), PIL-2 (China competitive dynamics)
Corpus: agentii-2026-09-10 | Skill pin: 61f794be22a5 | Constitution: 1.3.0

## Executive Summary

Ambarella is a fabless edge-AI vision SoC designer whose competitive position rests on design-in stickiness and a stable ~60% gross margin, not scale. FY2026 (ended Jan 31, 2026) revenue grew 37.2% to $390.7M [FACT](https://agentii.ai/v/AMBA/sec106/53); gross margin held at 59-60% across FY2024-FY2026 [FACT](https://agentii.ai/v/AMBA/sec106/55). The moat: CVflow AI architecture (transformer models to 34B parameters, ~90% of edge AI requirements), NN-ISP, 12-24+ month design cycles, and software lock-in [FACT](https://agentii.ai/v/AMBA/sec106/10) [FACT](https://agentii.ai/v/AMBA/sec106/16). Threats: OEM vertical integration, and China — HiSilicon/Horizon Robotics import substitution plus BIS Entity List restrictions on customers Hikvision and Dahua [FACT](https://agentii.ai/v/AMBA/sec106/27) [FACT](https://agentii.ai/v/AMBA/sec105/35). Robotics is an emerging, indirect exposure (CV7/N1-655 VLM/VLA SoCs) with no disclosed robotics revenue [FACT](https://agentii.ai/v/AMBA/sec106/9). Fiscal-calendar quirk flagged: registry month-3 vs filing Jan 31 [FACT](https://agentii.ai/v/AMBA/sec106/1).

## 0. Fiscal-Period Quirk (flagged)

[FACT] The FY2026 10-K cover states the fiscal year ended January 31, 2026, and the SEC index reports `report_date: 2026-01-31` for citation sec106. [FACT] However, the agentii gold registry (`search_companies`, `get_company_fiscal_calendar`) returns `fiscal_year_end_month: 3` and a quarter map with FY2026 Q4 ending 2026-03-31 — misaligned by roughly one month. [DEDUCTED] The registry quarter boundaries are systematically shifted versus the filing header. Per task guidance, the filing header governs: FY2026 = year ended 2026-01-31 throughout this artifact. All `period` values in `entity_claims` follow the filing header.

## 1. PIL-1 — Sensing-Layer Barriers: Competitive Structure of Edge-AI Vision

### 1.1 Strategic groups (who AMBA competes with)

[FACT] AMBA discloses two competitor sets: in IoT — HiSilicon (Huawei-owned), Novatek, NVIDIA, Qualcomm, and SigmaStar; in the automotive camera market — Horizon Robotics, Mobileye (Intel subsidiary), Novatek, NVIDIA, Qualcomm, Renesas, and Texas Instruments (https://agentii.ai/v/AMBA/sec106/17). [FACT] The same lists are repeated in risk factors, with the addition that certain customers and suppliers have divisions producing competitive products (https://agentii.ai/v/AMBA/sec106/27).

[VIEW] This puts AMBA in a "focused challenger" strategic group: a single-product-category pure-play competing against full-platform giants (NVIDIA, Qualcomm, Intel/Mobileye, TI) and Chinese substitutes (HiSilicon, Horizon Robotics, SigmaStar) simultaneously.

### 1.2 Differentiation: SoC capability (ISP/AI engines)

[FACT] Third-generation CVflow processes transformer AI networks for model sizes up to 34 billion parameters covering an estimated 90% of broad edge AI requirements; it fuses cameras, 4D imaging radar, lidar, thermal, and NIR modalities (https://agentii.ai/v/AMBA/sec106/10). [FACT] NN-ISP provides neural-network-based low-light noise reduction; HDR, MCTF, and deep sensor fusion (centralized camera+radar perception on one CV3 SoC) round out the imaging IP (https://agentii.ai/v/AMBA/sec106/10). [FACT] Software moat components: full SDKs, Cooper developer platform, and a Developer Zone with pre-optimized models and agentic blueprints for ISVs and system integrators (https://agentii.ai/v/AMBA/sec106/10).

[FACT] Process capability: fabless; the substantial majority of SoCs supplied by Samsung (Austin, TX and South Korea) at 10nm/5nm/4nm, with the first 2nm design taped out (https://agentii.ai/v/AMBA/sec106/17). [FACT] R&D intensity: approximately 75% of 959 employees are in R&D (https://agentii.ai/v/AMBA/sec106/17); R&D expense was $238.5M in FY2026, 61% of revenue (https://agentii.ai/v/AMBA/sec106/57).

[VIEW] AMBA's differentiation is algorithm-plus-software co-design at the edge (power-efficient transformers + imaging IP), which is difficult for commodity video-SoC vendors (Novatek, SigmaStar) to replicate and overlaps only partially with data-center-oriented NVIDIA/Qualcomm roadmaps.

### 1.3 Barriers: design wins and embedded cycles

[FACT] Design cycles last 12-18 months for IoT and longer than 18 months for automotive; product lifecycles run 12-24 months in most markets and longer than 24 months in automotive OEM and robotics (https://agentii.ai/v/AMBA/sec106/16). [FACT] Volume production typically begins 12-18 months after a design win; once incorporated, a solution is likely used for the product's life, and "a design loss to a competitor will likely preclude any opportunity for future revenue from such customer's product" (https://agentii.ai/v/AMBA/sec106/16). [FACT] Automotive customers additionally require multi-month qualification processes of both product and third-party contractors (https://agentii.ai/v/AMBA/sec106/27). [FACT] Once an OEM designs a competitor's device in, switching involves "significant cost, time, effort and risk" (https://agentii.ai/v/AMBA/sec106/27).

[VIEW] These are textbook embedded-system switching costs — the core of PIL-1's sensing-layer barrier claim — but they bind both ways: they protect incumbents and penalize a challenger like AMBA trying to dislodge Mobileye/NVIDIA/TI from existing sockets.

### 1.4 Pricing power: gross margin trajectory

[FACT] Gross margin by fiscal year: FY2024 60%, FY2025 60%, FY2026 59% (cost of revenue 40%, 40%, 41% of revenue) (https://agentii.ai/v/AMBA/sec106/55). [FACT] The FY2026 decrease was driven by "higher manufacturing costs associated with advanced process technologies, as well as lower sales of previously reserved inventory, partially offset by a higher percentage of sales from higher average selling price AI inference processors" (https://agentii.ai/v/AMBA/sec106/57). [FACT] Revenue mix is shifting toward higher-ASP AI inference processors, and more complex configurations (high-performance cameras, future automotive OEM) carry higher prices and gross margins than lower-performance competitive camera applications (https://agentii.ai/v/AMBA/sec106/53) (https://agentii.ai/v/AMBA/sec106/55).

[DEDUCTED] Revenue rose 72.5% from FY2024 to FY2026 ($226.5M to $390.7M) while gross margin stayed within a 1pp band (60% to 59%) — margin stability under rapid growth is consistent with differentiation-based pricing rather than commodity erosion. [DEDUCTED] The -1.0pp FY2026 gross-margin change is supply-side (advanced-node cost, inventory mix), not evidence of a price war — yet.

[FACT] Structural pricing threats disclosed: (i) OEMs increasingly seek to develop their own semiconductor solutions, particularly in consolidating markets such as IP security cameras; (ii) mature products face systematic ASP declines offset only partially by yield and cost improvements (https://agentii.ai/v/AMBA/sec106/27) (https://agentii.ai/v/AMBA/sec106/55). [VIEW] The IP-security consolidation trend is the single most direct moat-erosion vector at the sensing layer, because it converts AMBA's captive-camera OEM customers into potential in-house silicon competitors.

## 2. PIL-2 — China Competitive Dynamics: Vision-SoC Import Substitution

### 2.1 Demand-side: Entity List restrictions on China customers

[FACT] AMBA states several customers — Hangzhou Hikvision Digital Technology (Hikvision), Zhejiang Dahua Technology (Dahua), and affiliates of Shenzhen Dajiang Baiwang Technology — have been added to the BIS Entity List, limiting supply of U.S.-controlled items (https://agentii.ai/v/AMBA/sec105/35). [FACT] Per the FY2025 10-K, these customers "may seek to obtain similar or substitute products from our competitors that are not subject to these limitations, or to develop similar or substitute products themselves" (https://agentii.ai/v/AMBA/sec105/35). [FACT] The FY2026 10-K retains the risk framing without re-naming the Entity List customers, and adds U.S. regulations requiring notification of or prohibiting certain transactions with China-linked entities that could apply to intracompany activities with AMBA's China subsidiary (https://agentii.ai/v/AMBA/sec106/38).

[DEDUCTED] Entity List restrictions convert AMBA's former China security-camera demand into a substitution runway for domestic alternatives (HiSilicon/Hisilicon-based and SigmaStar designs) — a realized, not hypothetical, PIL-2 mechanism, though AMBA does not quantify the lost revenue.

### 2.2 Supply-side: local-supplier pressure and substitution competitors

[FACT] AMBA flags the risk that the Chinese government may require use of local suppliers, compel partnerships with local companies, and incentivize government-backed customers to buy from local suppliers (https://agentii.ai/v/AMBA/sec105/35) (https://agentii.ai/v/AMBA/sec106/38). [FACT] Direct Chinese-substitution competitors sit inside AMBA's disclosed competitor sets: HiSilicon (Huawei-owned) in IoT and Horizon Robotics in automotive cameras (https://agentii.ai/v/AMBA/sec106/17). [FACT] AMBA has 225 employees in China out of 959 total, one of four R&D design centers (US, China, Italy, Taiwan), and 24 issued China patents versus 390 issued US patents (https://agentii.ai/v/AMBA/sec106/19) (https://agentii.ai/v/AMBA/sec106/17) (https://agentii.ai/v/AMBA/sec106/18).

### 2.3 Revenue-side exposure

[FACT] FY2026 geographic revenue by bill-to location: Taiwan $271.9M, Asia Pacific other than Taiwan $71.0M, Europe $20.1M, North America other than US $21.8M, US $5.8M (https://agentii.ai/v/AMBA/sec106/97). [DEDUCTED] Asia Pacific (Taiwan + other) is 87.8% of FY2026 bill-to revenue; Taiwan alone is 69.6%; the US is 1.5%. [FACT] Channel concentration: distributor WT Microelectronics (Taiwan) was ~70% of FY2026 revenue, 63% in FY2025, and 53% in FY2024 (with Chicony at 14%) (https://agentii.ai/v/AMBA/sec106/98).

[VIEW] The bill-to geography understates China end-demand (WT is the Asia ex-Japan fulfillment partner) and overstates it simultaneously as Taiwan bill-to; either way, AMBA's revenue base is almost entirely Asia-Pacific — so Chinese import-substitution policy and Taiwan/China relations are first-order competitive risks, not tail risks. [VIEW] AMBA's China posture is structurally bilateral: it needs China (R&D center, 225 employees, historic Hikvision/Dahua demand) while U.S. export controls restrict what it can sell there — a squeeze that HiSilicon and Horizon Robotics are positioned to exploit.

## 3. Robotics Exposure — Honest Labeling (risk note)

[FACT] Robotics appears in the FY2026 10-K as an emerging application set: fixed robotics (industrial/logistics automation; N1-655 and CV7 SoCs run VLMs/VLAs for inspection agents) and mobile robotics (drones, terrestrial robots; CV5/CV7 perception plus N1-655 agentic behaviors) (https://agentii.ai/v/AMBA/sec106/9). [FACT] AMBA discloses a single operating segment and does not break out robotics revenue anywhere in the FY2026 10-K (https://agentii.ai/v/AMBA/sec106/97). [VIEW] AMBA's robotics exposure is therefore indirect and early-stage: robotics rides inside the IoT/automotive revenue base, and product lifecycles in robotics are disclosed as longer than 24 months — revenue recognition from design wins today is years out (https://agentii.ai/v/AMBA/sec106/16). Any profit-pool attribution of AMBA revenue to physical-AI robotics must be treated as a small, unquantifiable fraction, not a line item.

## 4. Key Metrics

| Metric | FY2024 | FY2025 | FY2026 | Source |
|---|---|---|---|---|
| Revenue ($M) | 226.5 | 284.9 | 390.7 | https://agentii.ai/v/AMBA/sec106/57 |
| Revenue growth YoY (%) | — | +25.8 | +37.2 | https://agentii.ai/v/AMBA/sec106/57 |
| Gross margin (%) | 60 | 60 | 59 | https://agentii.ai/v/AMBA/sec106/55 |
| Cost of revenue (% of revenue) | 40 | 40 | 41 | https://agentii.ai/v/AMBA/sec106/55 |
| R&D (% of revenue) | 95 | 79 | 61 | https://agentii.ai/v/AMBA/sec106/55 |
| Net loss ($M) | -169.4 | -117.1 | -75.9 | https://agentii.ai/v/AMBA/sec106/97 |
| Product cost ($M) | 83.2 | 106.2 | 153.4 | https://agentii.ai/v/AMBA/sec106/97 |
| WT distributor share (%) | 53 | 63 | 70 | https://agentii.ai/v/AMBA/sec106/98 |
| Asia Pacific bill-to share (%) | — | — | 87.8 | https://agentii.ai/v/AMBA/sec106/97 |
| Taiwan bill-to share (%) | 52.8 | 63.0 | 69.6 | https://agentii.ai/v/AMBA/sec106/97 |

Note: FY2024/FY2025 Taiwan bill-to shares (119,601/226,474 and 179,324/284,865) are [DEDUCTED] arithmetic on the same geographic table; the table's own row values are [FACT].

## 5. Coverage Gaps & Citations

**Coverage gaps:**
1. No segment-level IoT vs automotive revenue split — AMBA reports a single operating segment, so the sensing-layer automotive pool size cannot be isolated from filings (https://agentii.ai/v/AMBA/sec106/97).
2. No China-specific revenue or customer disclosure — geographic revenue is bill-to only (Taiwan-dominated), and Entity List customer revenue impact is unquantified.
3. No robotics revenue disclosure — robotics exposure is labeled indirect (see §3).
4. Fiscal-calendar quirk: gold registry `fiscal_year_end_month: 3` conflicts with the Jan 31 filing header (see §0).
5. Entity-map metric discipline: metrics outside entities.md §2 (net loss, R&D expense, WT concentration, headcount, geographic shares) are emitted only as cited prose [FACT]/[DEDUCTED] tags and require dispatcher map amendment before entering `entity_claims`; only `revenue_usd`, `gross_margin_pct`, and arithmetic derived from them were structured into `entity_claims` per entities.md §2.
6. 16 earnings-call transcripts exist in coverage (latest 2026-05-28) but were not used — design-win commentary enrichment is a follow-up option within the skill's 4-quarter lookback.

**Citations (roll-up index):**

1. AMBA sec106 page1 — fiscal year ended January 31, 2026: https://agentii.ai/v/AMBA/sec106/1
2. AMBA sec106 page9 — robotics applications, CV3 domain controllers: https://agentii.ai/v/AMBA/sec106/9
3. AMBA sec106 page10 — CVflow 34B params, NN-ISP, multi-modal fusion: https://agentii.ai/v/AMBA/sec106/10
4. AMBA sec106 page16 — design cycles, design-win economics, WT 70%: https://agentii.ai/v/AMBA/sec106/16
5. AMBA sec106 page17 — Samsung foundry 10/5/4nm + 2nm, competitor lists: https://agentii.ai/v/AMBA/sec106/17
6. AMBA sec106 page18 — competitive factors, patents: https://agentii.ai/v/AMBA/sec106/18
7. AMBA sec106 page19 — headcount 959 (225 China), EAR/BIS: https://agentii.ai/v/AMBA/sec106/19
8. AMBA sec106 page27 — OEM vertical integration, switching costs: https://agentii.ai/v/AMBA/sec106/27
9. AMBA sec106 page38 — China local-supplier pressure: https://agentii.ai/v/AMBA/sec106/38
10. AMBA sec106 page53 — FY26 highlights: https://agentii.ai/v/AMBA/sec106/53
11. AMBA sec106 page55 — GM 59/60/60, R&D 61%: https://agentii.ai/v/AMBA/sec106/55
12. AMBA sec106 page57 — revenue tables, GM variance drivers: https://agentii.ai/v/AMBA/sec106/57
13. AMBA sec106 page97 — geographic revenue, net loss series: https://agentii.ai/v/AMBA/sec106/97
14. AMBA sec106 page98 — WT 70%/63%/53%: https://agentii.ai/v/AMBA/sec106/98
15. AMBA sec105 page35 — Entity List: Hikvision, Dahua, Shenzhen Dajiang Baiwang: https://agentii.ai/v/AMBA/sec105/35

## 6. Verification Table

| # | Claim | Tag | Source (my retrieval) | /v/ link | Status |
|---|---|---|---|---|---|
| 1 | FY2026 revenue $390.7M | FACT | sec106 p53/p57 | https://agentii.ai/v/AMBA/sec106/53 | Verified (p57 exact: $390,702k) |
| 2 | FY2025/FY2024 revenue $284.9M / $226.5M | FACT | sec106 p57 | https://agentii.ai/v/AMBA/sec106/57 | Verified ($284,865k / $226,474k) |
| 3 | GM FY24/FY25/FY26 = 60/60/59% | FACT | sec106 p55 | https://agentii.ai/v/AMBA/sec106/55 | Verified (common-size table) |
| 4 | FY26 GM decline drivers (advanced-node cost, reserved inventory) | FACT | sec106 p57 | https://agentii.ai/v/AMBA/sec106/57 | Verified (verbatim) |
| 5 | Competitor sets IoT + automotive | FACT | sec106 p17/p27 | https://agentii.ai/v/AMBA/sec106/17 | Verified (identical lists both pages) |
| 6 | CVflow 3rd gen up to 34B params, ~90% edge AI | FACT | sec106 p10 | https://agentii.ai/v/AMBA/sec106/10 | Verified |
| 7 | Design cycles 12-18 mo IoT; >18 mo auto; win-to-volume 12-18 mo | FACT | sec106 p16 | https://agentii.ai/v/AMBA/sec106/16 | Verified |
| 8 | WT 70%/63%/53% concentration | FACT | sec106 p98 | https://agentii.ai/v/AMBA/sec106/98 | Verified |
| 9 | Hikvision/Dahua/Shenzhen Dajiang Baiwang on BIS Entity List | FACT | sec105 p35 | https://agentii.ai/v/AMBA/sec105/35 | Verified (named in FY2025 10-K) |
| 10 | 225 employees in China; 959 total | FACT | sec106 p19 | https://agentii.ai/v/AMBA/sec106/19 | Verified |
| 11 | Samsung majority foundry; 10/5/4nm; 2nm tape-out | FACT | sec106 p17 | https://agentii.ai/v/AMBA/sec106/17 | Verified |
| 12 | Taiwan bill-to $271.9M; APAC other $71.0M; US $5.8M | FACT | sec106 p97 | https://agentii.ai/v/AMBA/sec106/97 | Verified (table) |
| 13 | Asia Pacific 87.8% of FY26 bill-to revenue | DEDUCTED | sec106 p97 arithmetic | https://agentii.ai/v/AMBA/sec106/97 | Cross-checked: 342,960/390,702 = 87.78% |
| 14 | Revenue +72.5% FY24→FY26 with GM in 1pp band | DEDUCTED | sec106 p57+p55 | https://agentii.ai/v/AMBA/sec106/57 | Cross-checked: 390,702/226,474 = 1.7253 |
| 15 | Fiscal year ends Jan 31; registry says month 3 | FACT | sec106 p1 + gold registry | https://agentii.ai/v/AMBA/sec106/1 | Quirk flagged in §0 |
| 16 | R&D expense $238.5M FY26, 61% of revenue | FACT | sec106 p57/p55 | https://agentii.ai/v/AMBA/sec106/57 | Verified |
| 17 | Robotics: no disclosed robotics revenue | FACT | sec106 p97 (single segment) | https://agentii.ai/v/AMBA/sec106/97 | Verified (absence of disclosure) |
| 18 | Product cost FY26 $153.4M | FACT | sec106 p97 | https://agentii.ai/v/AMBA/sec106/97 | Verified ($153,419k) |

Audit note: every number above traces to a retrieval call made in this session (search_companies, get_ticker_coverage, get_company_fiscal_calendar, search_documents, search_sec_filings, read_source_outline ×2, read_source_pages ×4). No price data used. No uncited numbers emitted.
