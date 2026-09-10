---
artifact_id: "002-AMBA-supply-chain-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: AMBA
skill: supply-chain
mode: default
affix: supply-chain-map
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "8cb3ac1de486"
as_of: 2026-09-11
entity_claims:
  - entity: AMBA
    metric: revenue_usd
    value: 390702000
    unit: USD
    period: FY2026
    source: "10-K:page72"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: revenue_usd
    value: 284865000
    unit: USD
    period: FY2025
    source: "10-K:page72"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: revenue_usd
    value: 226474000
    unit: USD
    period: FY2024
    source: "10-K:page72"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: gross_margin_pct
    value: 59.2
    unit: pct
    period: FY2026
    source: "10-K:page72"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: gross_margin_pct
    value: 60.5
    unit: pct
    period: FY2025
    source: "10-K:page72"
    retrieved_at: 2026-09-11
  - entity: AMBA
    metric: gross_margin_pct
    value: 60.4
    unit: pct
    period: FY2024
    source: "10-K:page72"
    retrieved_at: 2026-09-11
citations: [sec106, sec105, sec104, ect53, ect54]
pillars_addressed: [PIL-1, PIL-2]
claim_state: pinned
key_metrics:
  revenue_fy2026_usd: 390702000
  revenue_fy2025_usd: 284865000
  revenue_fy2024_usd: 226474000
  gross_margin_fy2026_pct: 59.2
  gross_margin_fy2025_pct: 60.5
  gross_margin_fy2024_pct: 60.4
  gm_gap_change_fy2024_to_fy2026_pp: -1.2
  non_gaap_gross_margin_fy2026_pct: 60.7
  wt_revenue_share_fy2026_pct: 70
  taiwan_bill_to_share_fy2026_pct: 69.6
  iot_revenue_share_fy2026_pct: 80
  contract_manufacturer_purchase_commitments_jan2026_usd: 80400000
  inventory_days_q1_fy2027: 145
conclusions:
  - "AMBA runs a fully outsourced fabless chain: Samsung supplies the substantial majority of SoCs (current nodes 10/5/4 nm, first 2 nm tape-out); assembly/test is split across Signetics, STATS ChipPAC, ASE, Sigurd and KYEC; each SoC is single-sourced at one facility with no long-term supply agreements."
  - "The sensing-layer GM series held ~60%: 60.4% (FY2024) to 60.5% (FY2025) to 59.2% (FY2026), a -1.2pp three-year drift driven by advanced-node manufacturing costs — far from the PIL-1b -10pp falsifier and consistent with a resilient sensing-silicon margin anchor."
  - "Customer and geographic concentration is extreme: WT Microelectronics (Taiwan) channeled ~70% of FY2026 revenue; Taiwan bill-to was 69.6% of revenue; end-market mix is ~80% IoT (physical-security-led) and ~20% automotive (telematics-led)."
  - "Robotics exposure is indirect and early-stage: one warehouse-robotics design win in low-volume production plus further perception/fusion design wins (mostly 5 nm CVflow), with humanoid-type engagements acknowledged but not yet disclosable. AMBA maps to the sensing-silicon layer, not to a direct humanoid BOM."
facts_count: 34
deducted_count: 10
views_count: 2
citation_count: 67
---

# AMBA — Supply-Chain Map (mode: default)

Thesis 002 · Value Chain Profit Pool Map · PIL-1 (sensing-layer chain) + PIL-2 (China/BOM concentration proxies) · CIK 0001280263 · Fabless edge-AI vision SoCs

## 1. Executive Summary

Ambarella is a fabless designer of low-power edge-AI vision SoCs and is this thesis's sensing-silicon layer anchor. Its supply chain is fully outsourced and heavily concentrated: Samsung supplies the substantial majority of SoCs (current nodes 10/5/4 nm; first 2 nm tape-out), with assembly/test split across Signetics, STATS ChipPAC, ASE, Sigurd and KYEC — each SoC single-sourced at one facility with no long-term supply agreements. WT Microelectronics (Taiwan) channels ~70% of FY2026 revenue; Taiwan bill-to is 69.6% of revenue. End-market mix is ~80% IoT (physical-security-led) and ~20% automotive (telematics-led); robotics is indirect — one warehouse-robotics win in low-volume production, further perception wins, and undisclosed humanoid-type engagements. The GAAP gross-margin series ran 60.4% (FY2024) → 60.5% (FY2025) → 59.2% (FY2026), a −1.2pp three-year drift from advanced-node manufacturing costs, far from the PIL-1b −10pp falsifier. China exposure is indirect: no mainland-China manufacturing found; concentration runs through Taiwan fulfillment plus a China R&D center. All financials verified against XBRL authority-3 (10-K) facts.

## 2. Data Sources

| Source | citation_id | Filing / period | Accession |
|---|---|---|---|
| FY2026 10-K | sec106 | year ended 2026-01-31, filed 2026-03-23 | 0001193125-26-119321 |
| FY2025 10-K | sec105 | year ended 2025-01-31, filed 2025-03-28 | 0000950170-25-046499 |
| FY2024 10-K | sec104 | year ended 2024-01-31, filed 2024-03-29 | 0000950170-24-038555 |
| Q4 FY2026 earnings call transcript | ect53 | 2026-02-26 | — |
| Q1 FY2027 earnings call transcript | ect54 | 2026-05-28 | — |
| XBRL facts | — | `RevenueFromContractWithCustomerExcludingAssessedTax`, `GrossProfit` (us-gaap, is_primary, authority 3 = 10-K) | — |

Fiscal-calendar quirk (flagged): `gold_companies` registry stores `fiscal_year_end_month: 3` for AMBA, but every 10-K header and XBRL `period_end` shows a **January 31** fiscal year-end (e.g., report_date 2026-01-31, source file `amba-20260131.htm`) [FACT]. Per task instruction, filing headers were trusted and XBRL verification was done on `period_start`/`period_end` boundaries, not on the registry's `fiscal_year` filter (which is misaligned). Sources: sec106 https://agentii.ai/v/AMBA/sec106/1, sec105, sec104.

## 3. Analysis

### 3.1 Foundry & assembly structure (fabless, single-sourced)

- [FACT] Ambarella employs a fabless model using third-party foundries and assembly/test contractors; it holds no guaranteed production capacity from any supplier. https://agentii.ai/v/AMBA/sec106/16
- [FACT] Currently the **substantial majority of SoCs are supplied by Samsung** in facilities located in Austin, Texas and South Korea, with an option to buy fully-assembled/tested product or tested die in wafer form. https://agentii.ai/v/AMBA/sec106/17
- [FACT] Assembly chain: Samsung subcontracts assembly and initial test to **Signetics Corporation** and **STATS ChipPAC Ltd.**; for tested-die purchases, Ambarella contracts assembly to **ASE**; final test is handled by **Sigurd Corporation** or **King Yuan Electronics (KYEC)**. https://agentii.ai/v/AMBA/sec106/17
- [FACT] Firm orders are placed with suppliers up to **40 weeks** ahead of delivery (longer during capacity shortages), usually without a corresponding customer purchase order. https://agentii.ai/v/AMBA/sec106/17
- [FACT] **Each SoC is fabricated in only one manufacturing facility** ("single sourced"); a facility disruption could not be easily offset, and there are **no long-term supply agreements** with any manufacturing supplier. https://agentii.ai/v/AMBA/sec106/34
- [FACT] For advanced nodes (4 nm, 2 nm) only **Samsung and TSMC** are available foundries; converting manufacturing to a backup supplier would take **two or more quarters**. https://agentii.ai/v/AMBA/sec106/35
- [FACT] Process nodes in production: **10 nm, 5 nm, 4 nm**; the company "recently taped out our first SoC design in the 2 nm process node." Portfolio node map: CV5/CV72/CV75/CV3-AD685/N1/N1-655 at 5 nm; CV7 at 4 nm; CV2/CV28/CV25/CV22/CV2FS and S6L/H32 at 10 nm; S5L/H22 at 14 nm; S2L/A12 and S3L/H12 at 28 nm. https://agentii.ai/v/AMBA/sec106/17 https://agentii.ai/v/AMBA/sec106/13
- [FACT] Samsung officially announced **NVIDIA and Ambarella as its 2 nm process customers** (management statement on the Q1 FY27 call); wafer commitments with Samsung are negotiated annually, and over an 18-year relationship the company has "never had any problem" securing wafers. https://agentii.ai/v/AMBA/ect54/4

### 3.2 Customer concentration & distribution channel

- [FACT] **WT Microelectronics** (non-exclusive sales representative and fulfillment partner in Asia ex-Japan) accounted for approximately **70%** of FY2026 revenue, **63%** of FY2025, and **53%** of FY2024. The WT agreement runs to **January 2029** with 12-month auto-renewals and 60-day termination notice. https://agentii.ai/v/AMBA/sec106/36
- [FACT] For FY2024, a second >10% customer, ODM **Chicony Electronics** (14%), joined WT (53%). FY2025/FY2026: WT was the only >10% customer (63%/70%). WT accounts receivable was **$24.6M** at Jan 31, 2026 vs $12.3M a year earlier. https://agentii.ai/v/AMBA/sec106/98
- [FACT] CFO on the Q4 FY26 call: WT was **73.1% of Q4 FY2026 revenue and 69.7% of FY2026 revenue**; on the Q1 FY27 call WT dropped to **60.7%** of Q1 FY2027 revenue. https://agentii.ai/v/AMBA/ect53/3 https://agentii.ai/v/AMBA/ect54/2
- [FACT] Geographic revenue by bill-to location, FY2026/FY2025/FY2024 (in thousands): **Taiwan 271,928 / 179,324 / 119,601**; Asia Pacific ex-Taiwan 71,032 / 61,663 / 58,506; Europe 20,065 / 22,778 / 11,949; North America ex-US 21,833 / 18,074 / 25,754; United States 5,844 / 3,026 / 10,664. https://agentii.ai/v/AMBA/sec106/97
- [DEDUCTED] Taiwan bill-to share = 271,928 / 390,702 = **69.6%** of FY2026 revenue (FY2025: 62.9%; FY2024: 52.8%) — a rising Taiwan concentration consistent with the WT channel. Source data: https://agentii.ai/v/AMBA/sec106/97
- [DEDUCTED] US bill-to share = 5,844 / 390,702 = **1.5%** of FY2026 revenue (FY2024: 4.7%) — direct US demand is negligible; revenue is fulfilled through Asia. Source data: https://agentii.ai/v/AMBA/sec106/97
- [FACT] Purchase orders typically arrive **20–30 weeks** before scheduled delivery; standard orders are cancelable/deferrable by customers with limited notice, so backlog is not a reliable revenue indicator. https://agentii.ai/v/AMBA/sec106/16

### 3.3 End-market mix (IoT / automotive / robotics)

- [FACT] Since FY2018, IoT and automotive have been the largest end markets, collectively generating the majority of revenue; the company discloses a **single operating segment** and no quantitative 10-K split. https://agentii.ai/v/AMBA/sec106/54 https://agentii.ai/v/AMBA/sec106/97
- [FACT] Management (Q4 FY26 call): FY2026 automotive revenue (led by telematics) grew **high single digits**; IoT grew **almost 50%** YoY, led by portable video and continued strong physical-security growth. https://agentii.ai/v/AMBA/ect53/3
- [FACT] Management (same call): **IoT was around 80% of FY2026 revenue** (implying automotive ≈ 20%), with IoT roughly 50/50 split between enterprise-CapEx-driven (security, video conferencing) and consumer/prosumer (360° cameras, drones). https://agentii.ai/v/AMBA/ect53/5
- [DEDUCTED] Implied FY2026 end-market revenue: IoT ≈ 0.80 × 390.7M ≈ **$313M**; automotive ≈ **$78M**. Source data: https://agentii.ai/v/AMBA/ect53/5 https://agentii.ai/v/AMBA/sec106/72
- [FACT] Robotics (Q4 FY26 call): an **e-commerce warehouse-robotics design win is in low-volume production** — a "perception hub" for warehouse automation; described as the first such design win and "meaningful" if it scales. https://agentii.ai/v/AMBA/ect53/3
- [FACT] Robotics (Q1 FY27 call): **multiple new design wins** span video-only, perception, sensor-fusion and robot-controller/decision-maker roles, weighted toward perception/fusion; wins use the CVflow portfolio, **mostly 5 nm products** (some 10 nm and 4 nm). "There are some of the humanoid type of applications in that design wins, but we are not in a place to talk about just yet." https://agentii.ai/v/AMBA/ect54/4
- [FACT] Competitors: IoT — HiSilicon (Huawei), Novatek, NVIDIA, Qualcomm, Sigmastar; automotive camera — Horizon Robotics, Mobileye (Intel), Novatek, NVIDIA, Qualcomm, Renesas, TI. https://agentii.ai/v/AMBA/sec106/17

### 3.4 Margin structure & the GM series (PIL-1 / PIL-1b input)

- [FACT] Consolidated results (in thousands), FY2026 / FY2025 / FY2024: Revenue **390,702 / 284,865 / 226,474**; Cost of revenue 159,436 / 112,535 / 89,657; **Gross profit 231,266 / 172,330 / 136,817**; R&D 238,519 / 226,109 / 215,052; loss from operations (82,527) / (126,595) / (154,560); net loss (75,865) / (117,126) / (169,417). https://agentii.ai/v/AMBA/sec106/72
- [DEDUCTED] **GAAP gross margin series: FY2024 60.4% (136,817/226,474); FY2025 60.5% (172,330/284,865); FY2026 59.2% (231,266/390,702)** — consistent with the 10-K's rounded 60/60/59. https://agentii.ai/v/AMBA/sec106/72 https://agentii.ai/v/AMBA/sec106/55
- [DEDUCTED] **GM gap change FY2024→FY2026 = −1.2pp.** This is the AMBA sensing-layer margin anchor for PIL-1; note the PIL-1b falsifier (`motion_model_gm_gap_change_pp`, threshold < −10pp) is defined on PH/NVDA/ISRG motion-vs-model series per entities.md §3, so AMBA's −1.2pp is context evidence, not the falsifier test input itself. Source data: https://agentii.ai/v/AMBA/sec106/72
- [FACT] 10-K narrative: FY2026 GM fell on **higher manufacturing costs of advanced process technologies** and lower sales of previously reserved inventory, partially offset by a higher-ASP AI-inference mix; FY2025 GM rose marginally on AI-inference mix and higher-margin NRE service revenue. https://agentii.ai/v/AMBA/sec106/57
- [FACT] Cost of revenue includes third-party-foundry wafers, packaging/assembly/test, logistics, planning, quality, inventory reserves, adverse purchase-commitment reserves, and amortization of developed technology. https://agentii.ai/v/AMBA/sec106/55
- [FACT] Non-GAAP gross margin: **FY2026 60.7% vs FY2025 62.7%**; Q4 FY2026 59.8%; Q1 FY2027 59.9%; long-term GM model **59%–62%** reaffirmed on the Q1 FY27 call. https://agentii.ai/v/AMBA/ect53/3 https://agentii.ai/v/AMBA/ect54/2 https://agentii.ai/v/AMBA/ect54/4
- [FACT] Segment-disclosure product cost (excludes SBC amortization mapping): FY2026 **153,419** / FY2025 106,237 / FY2024 83,221 (in thousands). https://agentii.ai/v/AMBA/sec106/97
- [DEDUCTED] Product cost as % of revenue: FY2026 **39.3%**, FY2025 37.3%, FY2024 36.7% — rising wafer/assembly cost intensity across the three years. Source data: https://agentii.ai/v/AMBA/sec106/97
- [FACT] FY2026 revenue grew **37.2%** YoY on higher unit shipments and a higher share of higher-ASP AI inference processors, partially offset by lower NRE service revenue; FY2025 grew 25.8%. https://agentii.ai/v/AMBA/sec106/53 https://agentii.ai/v/AMBA/sec106/57
- [FACT] Q1 FY2027 (period ended 2026-04-30): revenue **$100.4M** (+16.9% YoY); FY2027 growth expectation reiterated at **10–15%**, with automotive growing faster than IoT. https://agentii.ai/v/AMBA/ect54/2

### 3.5 Supply-chain working capital & commitments (PIL-2 demand-side signals)

- [FACT] **Contract-manufacturer purchase commitments: $80.4M at Jan 31, 2026 vs $56.4M at Jan 31, 2025** (+$24.0M YoY); purchase orders are cancelable upon agreement, with no material adverse-purchase-commitment loss liabilities recorded. https://agentii.ai/v/AMBA/sec106/96
- [DEDUCTED] Commitment growth (+42.6% YoY) outstripped revenue growth (+37.2% YoY) — consistent with building supply for new product cycles. Source data: https://agentii.ai/v/AMBA/sec106/96 https://agentii.ai/v/AMBA/sec106/53
- [FACT] Inventory days rose **76 → 99 days** during Q4 FY2026 ("to support our current level of business") and **99 → 145 days** in Q1 FY2027 ("to better service customers in the face of a number of new product cycles"); Q1 FY2027 operating cash flow was −$25.6M on that inventory build. https://agentii.ai/v/AMBA/ect53/3 https://agentii.ai/v/AMBA/ect54/2
- [FACT] FY2026 operating cash flow was **$73.5M** (vs $33.8M FY2025); free cash flow **$58.0M** (14.8% of revenue); capex (tangible + intangible) **$15.5M** for the year. https://agentii.ai/v/AMBA/sec106/53 https://agentii.ai/v/AMBA/ect53/3
- [FACT] R&D is the dominant cost: **~75% of employees** are in R&D across four design centers (US, China, Italy, Taiwan); EDA toolchain vendors Cadence, Mentor Graphics and Synopsys are critical suppliers. https://agentii.ai/v/AMBA/sec106/17 https://agentii.ai/v/AMBA/sec106/36

### 3.6 China / PIL-2 structural read (honest labeling)

- [FACT] No mainland-China manufacturing is disclosed: fabrication is Samsung (Austin, TX / South Korea), assembly/test in Korea and Taiwan (Signetics, STATS ChipPAC, ASE, Sigurd, KYEC). https://agentii.ai/v/AMBA/sec106/17
- [FACT] China exposure is indirect: a **China R&D design center**; sales/business-development offices in China and Hong Kong; Taiwan-centric fulfillment (~70% via WT, 69.6% bill-to Taiwan); export-control (BIS/EAR) risk factors include Huawei/HiSilicon as competitor and Entity-List dynamics. https://agentii.ai/v/AMBA/sec106/17 https://agentii.ai/v/AMBA/sec106/97 https://agentii.ai/v/AMBA/sec106/38
- [VIEW] For the PIL-2 falsifier proxy (`nonchina_to_china_humanoid_bom_cost_ratio`, threshold < 2.0 falsifies; proxies only, Deviation Register, expiry 2026-10-10): AMBA's chain is nominally non-China (Samsung/Austin + Korea/Taiwan OSAT), but ~70% of revenue is fulfilled through a Taiwan distributor whose end customers are Asia-based ODMs/OEMs with undocumented final geography. A naively computed "non-China BOM" ratio would be overstated; the honest read is *unknown end-demand geography* behind a Taiwan curtain, with China policy (export controls) as the binding supply risk, not China fabs.
- [VIEW] Robotics/humanoid mapping must stay honest: AMBA's disclosed robotics exposure is one warehouse-robotics production win plus undisclosed-size perception/fusion design wins, with humanoid-type engagements explicitly not yet disclosable. Mapping AMBA as a direct humanoid BOM component at the sensing layer is a [VIEW]-grade assumption, not a [FACT].

## 4. Key Metrics

| Metric | FY2024 | FY2025 | FY2026 | Source |
|---|---|---|---|---|
| Revenue ($K) | 226,474 | 284,865 | 390,702 | https://agentii.ai/v/AMBA/sec106/72 |
| Gross profit ($K) | 136,817 | 172,330 | 231,266 | https://agentii.ai/v/AMBA/sec106/72 |
| GAAP gross margin | 60.4% | 60.5% | 59.2% | [DEDUCTED] https://agentii.ai/v/AMBA/sec106/72 |
| Non-GAAP gross margin | — | 62.7% | 60.7% | https://agentii.ai/v/AMBA/ect53/3 |
| WT revenue share | 53% | 63% | ~70% (69.7% per CFO) | https://agentii.ai/v/AMBA/sec106/36 https://agentii.ai/v/AMBA/ect53/3 |
| Taiwan bill-to share | 52.8% | 62.9% | 69.6% | [DEDUCTED] https://agentii.ai/v/AMBA/sec106/97 |
| Contract-mfr purchase commitments (Jan 31) | — | $56.4M | $80.4M | https://agentii.ai/v/AMBA/sec106/96 |
| Inventory days (quarter-end) | — | — | 99 (Q4 FY26) → 145 (Q1 FY27) | https://agentii.ai/v/AMBA/ect53/3 https://agentii.ai/v/AMBA/ect54/2 |

GM series is the PIL-1b gap-change input carrier: **60.4% → 60.5% → 59.2% (−1.2pp over 3 FYs)** [DEDUCTED].

## 5. Coverage Gaps & Citations

Coverage gaps:

1. **No quantitative IoT vs automotive revenue split in the 10-K** (single operating segment); the ~80/20 mix rests on management's transcript statement (ect53 page5), not audited tabular data.
2. **No humanoid-specific revenue/BOM disclosure** — engagements are design-win stage and explicitly not quantifiable ("not in a place to talk about just yet", ect54 page4). Expected under the thesis's filing-proxy constraint; teardown figures would be [VIEW] only.
3. **No China-specific revenue or end-demand geography disclosure** — bill-to location is Taiwan-centric (fulfillment via WT); end-customer geography is opaque.
4. **Per-foundry allocation and wafer-cost series not quantified** — Samsung share is "substantial majority" (qualitative); GM drivers are narrative only.
5. **Inventory days sourced from transcripts** (press-release data relayed on calls), not from 10-K pages retrieved in this run; Q1 FY2027 financials rest on transcript + XBRL (10-Q not pulled).
6. **Registry fiscal-calendar quirk**: `fiscal_year_end_month: 3` in gold_companies vs actual January-31 year-end (filing headers) — flagged; XBRL verification performed on period boundaries.
7. **New metrics discovered but NOT added to `entity_claims`** (per entities.md §2 discipline — map append is the implement dispatcher's call): `wt_revenue_share_pct`, `chicony_revenue_share_pct`, `taiwan_bill_to_share_pct`, `iot_revenue_share_pct`, `non_gaap_gross_margin_pct`, `inventory_days`, `contract_manufacturer_purchase_commitments_usd`, `corporate_asp_usd` ($15 corporate ASP stated on ect54 page2).

Citation index (roll-up, non-duplicative of inline links):

- sec106 — FY2026 10-K (year ended 2026-01-31): pages 13, 16, 17, 34, 35, 36, 38, 53, 54, 55, 57, 72, 96, 97, 98 → https://agentii.ai/v/AMBA/sec106/{N}
- sec105 / sec104 — FY2025 / FY2024 10-Ks (XBRL authority-3 cross-verification of FY2024–FY2025 revenue and gross profit facts)
- ect53 — Q4 FY2026 earnings call (2026-02-26): pages 3, 5 → https://agentii.ai/v/AMBA/ect53/{N}
- ect54 — Q1 FY2027 earnings call (2026-05-28): pages 2, 4 → https://agentii.ai/v/AMBA/ect54/{N}

## 6. Verification table (audit mandate)

| Claim | Filing source | XBRL cross-check | Status |
|---|---|---|---|
| Revenue FY2024 $226,474K | sec106 page72 | RFCCExcludingAssessedTax = 226,474,000, period 2023-02-01→2024-01-31, authority 3 (amba-20240131.htm) | PASS |
| Revenue FY2025 $284,865K | sec106 page72 | 284,865,000, period 2024-02-01→2025-01-31, authority 3 (amba-20260131.htm) | PASS |
| Revenue FY2026 $390,702K | sec106 page72 | 390,702,000, period 2025-02-01→2026-01-31, authority 3 (amba-20260131.htm) | PASS |
| Gross profit FY2024 $136,817K | sec106 page72 | GrossProfit = 136,817,000, period 2023-02-01→2024-01-31, authority 3 (amba-20250131.htm) | PASS |
| Gross profit FY2025 $172,330K | sec106 page72 | 172,330,000, period 2024-02-01→2025-01-31, authority 3 (amba-20250131.htm) | PASS |
| Gross profit FY2026 $231,266K | sec106 page72 | 231,266,000, period 2025-02-01→2026-01-31, authority 3 (amba-20260131.htm) | PASS |
| WT ~70% FY2026 | sec106 pages 36/98 | CFO: 69.7% FY2026, 73.1% Q4 (ect53 page3); 60.7% Q1 FY27 (ect54 page2) | PASS (consistent) |
| FY2026 revenue +37.2% | sec106 page53 | Page-57 variance table: +105,837 / 37.2% | PASS |
| Q1 FY2027 revenue $100.4M | ect54 page2 | RFCCExcludingAssessedTax = 100,357,000, period 2026-02-01→2026-04-30 (amba-20260430.htm); GrossProfit = 58,589,000 | PASS |
