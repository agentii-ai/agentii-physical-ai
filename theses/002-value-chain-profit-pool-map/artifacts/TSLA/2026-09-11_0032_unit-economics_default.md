---
artifact_id: "002-TSLA-unit-economics-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: TSLA
skill: unit-economics
mode: default
affix: unit-economics
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "e87ee63269a2"
as_of: 2026-09-11
entity_claims:
  - entity: TSLA
    metric: automotive_gross_margin_pct
    value: 17.8
    unit: pct
    period: FY2025
    source: "10-K:page43"
    retrieved_at: 2026-09-11
    tag: FACT
  - entity: TSLA
    metric: automotive_gross_margin_pct
    value: 18.4
    unit: pct
    period: FY2024
    source: "10-K:page43"
    retrieved_at: 2026-09-11
    tag: FACT
  - entity: TSLA
    metric: automotive_gross_margin_pct
    value: 19.4
    unit: pct
    period: FY2023
    source: "10-K:page43"
    retrieved_at: 2026-09-11
    tag: FACT
  - entity: TSLA
    metric: automotive_cost_of_revenue_usd
    value: 57165000000
    unit: USD
    period: FY2025
    source: "10-K:page43"
    retrieved_at: 2026-09-11
    tag: FACT
  - entity: TSLA
    metric: automotive_revenue_usd
    value: 69526000000
    unit: USD
    period: FY2025
    source: "10-K:page42"
    retrieved_at: 2026-09-11
    tag: FACT
  - entity: TSLA
    metric: revenue_per_vehicle_usd
    value: 42394
    unit: USD
    period: FY2025
    source: "10-K:page42"
    retrieved_at: 2026-09-11
    tag: DEDUCTED
  - entity: TSLA
    metric: cost_per_vehicle_usd
    value: 34857
    unit: USD
    period: FY2025
    source: "10-K:page43"
    retrieved_at: 2026-09-11
    tag: DEDUCTED
  - entity: TSLA
    metric: gross_profit_per_vehicle_usd
    value: 7537
    unit: USD
    period: FY2025
    source: "10-K:page43"
    retrieved_at: 2026-09-11
    tag: DEDUCTED
citations:
  - "sec253 (FY2025 10-K, filed 2026-01-29, accession 0001628280-26-003952): p36, p42, p43, p55, p98"
pillars_addressed: [PIL-1]
claim_state: pinned
key_metrics:
  FY2025_automotive_gross_margin_pct: 17.8
  FY2024_automotive_gross_margin_pct: 18.4
  FY2023_automotive_gross_margin_pct: 19.4
  FY2025_automotive_revenue_usd_bn: 69.526
  FY2025_automotive_cogs_usd_bn: 57.165
  FY2025_automotive_gross_profit_usd_bn: 12.361
  FY2025_deliveries_m: 1.64
  FY2025_revenue_per_vehicle_usd: 42394
  FY2025_cost_per_vehicle_usd: 34857
  FY2025_gross_profit_per_vehicle_usd: 7537
  FY2025_total_gross_margin_pct: 18.0
  FY2025_capex_usd_bn: 8.53
conclusions:
  - "TSLA automotive GM series FY2023→FY2025 (19.4% → 18.4% → 17.8%, −1.6pp over three fiscal years) is reproduced from sec253 p43 and is a shallow negative trend — an input to PIL-1b's motion_model_gm_gap_change_pp test, far from the −10pp falsifier band on its own."
  - "FY2025 per-vehicle economics (~$42.4K revenue / ~$34.9K cost / ~$7.5K gross profit on ~1.64M deliveries) reproduce the T-001 baseline exactly; automotive COGS is the only filed per-unit cost reference for the vertically-integrated motion structure."
  - "No Optimus per-unit cost, BOM split, or price disclosure exists in any retrieved filing; the automotive cost stack is the PIL-1 analogue and is labeled as such throughout — PIL-1a's >55% actuation+sensing BOM share cannot be validated from TSLA disclosures."
  - "The 10-K enumerates automotive COGS components qualitatively (materials, labor, overhead/depreciation, logistics, tariffs, warranty, connectivity/FSD maintenance); the only numeric structural fact is segment D&A (5.5% of automotive-segment COGS FY2025)."
facts_count: 16
deducted_count: 8
views_count: 3
citation_count: 55
---

# TSLA — Unit Economics (default) | Thesis 002, Pillar PIL-1

> PIL-1: vertically-integrated cost reference. Retrieval per CHAIN: preflight → Layer 1 → Layer 2 → Layer 3 → XBRL cross-check. All figures trace to agentii MCP retrieval calls made in this run; uncited numbers are void (constitution P4).

## 1. Executive Summary

Tesla's filed FY2025 automotive economics are the vertically-integrated cost reference for PIL-1: on ~1.64M delivered vehicles https://agentii.ai/v/TSLA/sec253/36, automotive revenues of $69,526M https://agentii.ai/v/TSLA/sec253/42 and automotive cost of revenues of $57,165M https://agentii.ai/v/TSLA/sec253/43 produce a 17.8% automotive gross margin — ~$42.4K revenue, ~$34.9K cost, ~$7.5K gross profit per vehicle [DEDUCTED]. The FY2023→FY2025 automotive GM series is 19.4% → 18.4% → 17.8% (−1.6pp) https://agentii.ai/v/TSLA/sec253/43: a shallow decline that serves as PIL-1b's integrated-OEM motion-side gap-change input. The 10-K enumerates the COGS stack qualitatively — materials, labor, manufacturing overhead incl. depreciation, shipping/logistics, tariffs, warranty reserves, FSD/connectivity maintenance https://agentii.ai/v/TSLA/sec253/43 — with depreciation the only numeric structural anchor (5.5% of automotive-segment COGS) https://agentii.ai/v/TSLA/sec253/98. No Optimus per-unit cost exists in any filing; the automotive stack is the analogue for humanoid actuation+motion economics and is labeled as such. XBRL authority-3 facts for Revenues and CostOfRevenue match the filing tables exactly for all three years https://agentii.ai/v/TSLA/sec253/55.

## 2. Core Analysis

### 2.1 Automotive per-unit economics FY2025 — the vertically-integrated cost reference

[FACT] In 2025 Tesla produced approximately 1.66M consumer vehicles and delivered approximately 1.64M https://agentii.ai/v/TSLA/sec253/36. [FACT] Revenue (Table 7): automotive sales $65,821M, automotive regulatory credits $1,993M, automotive leasing $1,712M — total automotive revenues $69,526M (−10% YoY); services and other $12,530M; energy $12,771M; total revenues $94,827M https://agentii.ai/v/TSLA/sec253/42. [FACT] Cost (Table 8): automotive sales cost $56,267M plus automotive leasing cost $898M — total automotive cost of revenues $57,165M (−9% YoY); total cost of revenues $77,733M; total-automotive gross profit $12,361M; total-automotive gross margin 17.8% https://agentii.ai/v/TSLA/sec253/43. [FACT] The same figures appear on the consolidated income statement https://agentii.ai/v/TSLA/sec253/55.

[DEDUCTED] Per-vehicle (÷ ~1.64M deliveries): revenue ≈ $69,526M / 1.64M ≈ **$42,394/vehicle**; cost ≈ $57,165M / 1.64M ≈ **$34,857/vehicle**; gross profit ≈ $12,361M / 1.64M ≈ **$7,537/vehicle** (17.8% margin) https://agentii.ai/v/TSLA/sec253/36 https://agentii.ai/v/TSLA/sec253/42 https://agentii.ai/v/TSLA/sec253/43. [DEDUCTED] On a sales-only basis (excluding leasing and regulatory credits, the closest analogue to a pure vehicle sale): revenue ≈ $65,821M / 1.64M ≈ **$40,135/vehicle** and cost ≈ $56,267M / 1.64M ≈ **$34,309/vehicle** https://agentii.ai/v/TSLA/sec253/42 https://agentii.ai/v/TSLA/sec253/43. [DEDUCTED] Regulatory credits were 2.9% of total automotive revenues in FY2025 ($1,993M / $69,526M), down from 3.6% in FY2024 ($2,763M / $77,070M) https://agentii.ai/v/TSLA/sec253/42. [FACT] Context on the cost envelope: FY2025 capex was $8.53B (vs $11.34B in 2024) https://agentii.ai/v/TSLA/sec253/36.

[VIEW] **Analogue labeling (mandatory under CLAIM DISCIPLINE):** these per-vehicle figures describe the *automotive* cost stack, not humanoid economics. No Optimus per-unit cost or BOM disclosure exists in any retrieved filing (consistent with T-001's audited finding). The automotive stack is offered strictly as the vertically-integrated cost reference — an integrated OEM's demonstrated ability to build a ~$35K-unit-cost electromechanical product at 17.8% GM — not as a prediction of Optimus unit cost.

### 2.2 COGS structure — what the filing does and does not disclose

[FACT] The 10-K enumerates the automotive COGS stack without numeric splits: "direct and indirect materials, labor costs, manufacturing overhead, including depreciation costs of tooling and machinery, shipping and logistic costs, tariffs, reserves for estimated warranty expenses, FSD (Supervised) ongoing maintenance costs, vehicle connectivity costs, and allocations of electricity and infrastructure costs related to our free Supercharging programs", plus inventory write-downs and obsolescence charges; cost of automotive sales revenue also "benefits from manufacturing credits recognized" https://agentii.ai/v/TSLA/sec253/43. [FACT] No numeric materials/labor/overhead split is disclosed anywhere in the retrieved pages — the composition of the ~$35K per-vehicle cost is not filed. [FACT] The one numeric structural anchor is depreciation: D&A inside automotive-segment cost of revenues was $3.78B (FY2025), $3.68B (FY2024), $3.45B (FY2023) https://agentii.ai/v/TSLA/sec253/98.

[DEDUCTED] D&A share of automotive-segment COGS: $3.78B / $68,764M ≈ **5.5%** (FY2025); $3.68B / $72,794M ≈ 5.1% (FY2024); $3.45B / $74,219M ≈ 4.6% (FY2023) https://agentii.ai/v/TSLA/sec253/98. Against total-automotive (ex-services) COGS of $57,165M, D&A is ≈6.6% in FY2025 https://agentii.ai/v/TSLA/sec253/43 https://agentii.ai/v/TSLA/sec253/98.

[VIEW] **Analogue implication:** the filing evidence shows an integrated manufacturing cost stack dominated by materials + overhead and a modest (~5–7%) depreciation component — consistent with the thesis framing that motion/actuation hardware (materials- and process-intensive) rather than software or depreciation drives unit cost. This is directionally supportive of PIL-1's profit-pool location but is a filing-proxy observation only; it does not quantify actuation+sensing share of BOM (PIL-1a's >55% test remains untestable on TSLA's record).

### 2.3 Automotive GM series FY2023→FY2025 — the PIL-1b gap-change input

[FACT] Gross-margin series (Table 8, all three fiscal years): total-automotive GM **19.4% (FY2023) → 18.4% (FY2024) → 17.8% (FY2025)**; total-automotive & services GM 18.2% / 16.9% / 16.2%; energy GM 18.9% / 26.2% / 29.8%; total GM 18.2% / 17.9% / 18.0% https://agentii.ai/v/TSLA/sec253/43. [FACT] Segment note (Note 16): automotive segment (incl. services) revenues $82,056M / $87,604M / $90,738M and cost of revenues $68,764M / $72,794M / $74,219M for 2025/2024/2023; the CODM evaluates segments on gross profit https://agentii.ai/v/TSLA/sec253/98.

[DEDUCTED] Arithmetic reconciliation: 1 − COGS/revenues reproduces the filed GMs to one decimal for every year — 1 − 66,389/82,419 = 19.4%; 1 − 62,873/77,070 = 18.4%; 1 − 57,165/69,526 = 17.8% https://agentii.ai/v/TSLA/sec253/42 https://agentii.ai/v/TSLA/sec253/43. [DEDUCTED] Segment GM recomputation matches the A&S line exactly: 16.2% / 16.9% / 18.2% https://agentii.ai/v/TSLA/sec253/98. [DEDUCTED] Three-fiscal-year change in the automotive GM series: **−1.6pp total** (−1.0pp in FY2024, −0.6pp in FY2025) https://agentii.ai/v/TSLA/sec253/43.

[VIEW] **PIL-1b framing:** this series is the integrated-OEM ("motion-side") input to `motion_model_gm_gap_change_pp`. TSLA's own 3-FY trend is shallowly negative (−1.6pp), far from the < −10pp falsifier threshold on its own; the falsifier fires only if the *gap versus the model layer* (NVDA/ISRG series, retrieved in their own artifacts) falls >10pp. TSLA GM here also reflects mix/incentive pressure the 10-K attributes to lower ASP and financing incentives rather than cost degradation: automotive sales revenue fell 9% on an ~8% cash-delivery decline and lower average selling price https://agentii.ai/v/TSLA/sec253/42.

### 2.4 Audit — XBRL cross-check and T-001 reconciliation

[FACT] XBRL `us-gaap:Revenues` (is_primary, source_authority 3 = 10-K facts): $94,827M (2025-01-01→2025-12-31), $97,690M (FY2024), $96,773M (FY2023) — matching Table 7 and the income statement exactly https://agentii.ai/v/TSLA/sec253/55. [FACT] XBRL `us-gaap:CostOfRevenue` (authority 3): $77,733M (FY2025), $80,240M (FY2024), $79,113M (FY2023) — matching Table 8 exactly https://agentii.ai/v/TSLA/sec253/43 https://agentii.ai/v/TSLA/sec253/55. [FACT] Concept discovery: `us-gaap:CostOfGoodsAndServicesSold` returns zero facts for TSLA; the filer uses `CostOfRevenue` (85 facts). [FACT] Reconciliation against the T-001 baseline: FY2025 automotive GM 17.8% ✓, automotive revenue $69,526M ✓, COGS $57,165M ✓, per-vehicle $42,394 / $34,857 ✓ — all reproduced from fresh retrieval. [FACT] Geographic revenue (Note 16): United States $47,627M, China $20,962M, other international $26,238M for FY2025 https://agentii.ai/v/TSLA/sec253/98. [FACT] The 10-K states the current tariff regime "will have a relatively larger impact on our energy generation and storage business compared to our automotive business" https://agentii.ai/v/TSLA/sec253/36.

## 3. Key Metrics

| Metric | FY2023 | FY2024 | FY2025 | Tag | Citation |
|---|---|---|---|---|---|
| Total automotive revenues | $82,419M | $77,070M | $69,526M | FACT | https://agentii.ai/v/TSLA/sec253/42 |
| Total automotive cost of revenues | $66,389M | $62,873M | $57,165M | FACT | https://agentii.ai/v/TSLA/sec253/43 |
| Total automotive gross profit | $16,030M | $14,197M | $12,361M | FACT | https://agentii.ai/v/TSLA/sec253/43 |
| **Automotive gross margin** | **19.4%** | **18.4%** | **17.8%** | FACT | https://agentii.ai/v/TSLA/sec253/43 |
| Automotive & services GM | 18.2% | 16.9% | 16.2% | FACT | https://agentii.ai/v/TSLA/sec253/43 |
| Energy generation & storage GM | 18.9% | 26.2% | 29.8% | FACT | https://agentii.ai/v/TSLA/sec253/43 |
| Total gross margin | 18.2% | 17.9% | 18.0% | FACT | https://agentii.ai/v/TSLA/sec253/43 |
| Total revenues | $96,773M | $97,690M | $94,827M | FACT | https://agentii.ai/v/TSLA/sec253/42 |
| Total cost of revenues | $79,113M | $80,240M | $77,733M | FACT | https://agentii.ai/v/TSLA/sec253/43 |
| Vehicle deliveries / production | — | — | ~1.64M / ~1.66M | FACT | https://agentii.ai/v/TSLA/sec253/36 |
| Revenue per vehicle | — | — | ~$42,394 | DEDUCTED | https://agentii.ai/v/TSLA/sec253/42 |
| Cost per vehicle | — | — | ~$34,857 | DEDUCTED | https://agentii.ai/v/TSLA/sec253/43 |
| Gross profit per vehicle | — | — | ~$7,537 | DEDUCTED | https://agentii.ai/v/TSLA/sec253/43 |
| Sales-only rev / cost per vehicle | — | — | ~$40,135 / ~$34,309 | DEDUCTED | https://agentii.ai/v/TSLA/sec253/42 |
| D&A in automotive-segment COGS | $3.45B | $3.68B | $3.78B | FACT | https://agentii.ai/v/TSLA/sec253/98 |
| D&A share of automotive-segment COGS | 4.6% | 5.1% | 5.5% | DEDUCTED | https://agentii.ai/v/TSLA/sec253/98 |
| Capex | — | $11.34B | $8.53B | FACT | https://agentii.ai/v/TSLA/sec253/36 |
| XBRL Revenues (authority 3) | $96,773M | $97,690M | $94,827M | FACT | https://agentii.ai/v/TSLA/sec253/55 |
| XBRL CostOfRevenue (authority 3) | $79,113M | $80,240M | $77,733M | FACT | https://agentii.ai/v/TSLA/sec253/43 |
| Optimus per-unit economics | none disclosed in any filing | | | FACT | https://agentii.ai/v/TSLA/sec253/36 |

## 4. Coverage Gaps & Citations

**Coverage gaps:**
1. **Optimus unit economics**: no per-unit cost, BOM split, or price exists in any retrieved filing. PIL-1a's actuation+sensing >55% BOM-share falsifier cannot be run against TSLA disclosures; the automotive stack above is the labeled analogue (clarify round-3 rule: filing proxies carry the tests).
2. **Numeric COGS composition**: the 10-K enumerates automotive cost components but discloses no materials/labor/overhead dollar split; D&A is the only numeric structural anchor (Note 16 footnote).
3. **FY2024/FY2023 per-vehicle figures**: deliveries for those years live in sec235 (FY2024 10-K) and sec221 (FY2023 10-K), not retrieved in this run; per-unit economics are therefore FY2025-only. Revenue/COGS/GM series for all three years come from sec253's own 3-year tables.
4. **Vehicle-only D&A**: the Note 16 footnote covers the automotive segment including services and other; a vehicle-only D&A figure is not separable.
5. **Automotive manufacturing-credit dollar amount** (referenced qualitatively on p43; detailed on p64) was not page-read this run and is intentionally omitted.
6. **Concept registry**: `list_xbrl_concepts` returned an empty set for the search term; concept discovery was completed empirically via fact counts (CostOfRevenue 85 facts vs CostOfGoodsAndServicesSold 0).

**Citation index (roll-up, non-duplicative):**

| citation_id | Filing | Pages used |
|---|---|---|
| sec253 | FY2025 10-K, filed 2026-01-29, accession 0001628280-26-003952 | 36, 42, 43, 55, 98 |

**Dispatcher note (entity-map append, per entities.md §2 discipline):** this artifact emits four metric names beyond the current TSLA map rows — `automotive_revenue_usd` [FACT], `revenue_per_vehicle_usd`, `cost_per_vehicle_usd`, `gross_profit_per_vehicle_usd` [DEDUCTED arithmetic on map metrics ÷ filed deliveries]. These are presented for the implement dispatcher to append to `entities.md`; no shared file was edited.

## 5. Verification

| # | Tool call | Purpose | Result |
|---|---|---|---|
| 1 | search_companies(TSLA) | Ticker resolution | Tesla, Inc., CIK 0001318605, NASDAQ, industrial.automotive |
| 2 | get_ticker_coverage(TSLA) | Coverage preflight | 7 sources; xbrl_facts 63,523; src_documents 92; 19 transcripts |
| 3 | get_company_fiscal_calendar(TSLA) | Fiscal alignment | fiscal_year_end_month 1 (corpus encoding); filings keyed to Dec-31 report dates — FY2025 = calendar 2025 |
| 4 | search_sec_filings(TSLA, 10-K) | Layer 1 | sec253 = FY2025 10-K (accession 0001628280-26-003952, filed 2026-01-29); sec235 = FY2024; sec221 = FY2023 |
| 5 | search_documents(TSLA, 10-K) | Layer 1 (alt) | FY2025 10-K confirmed, filed 2026-01-29 |
| 6 | read_source_outline(TSLA, sec253) | Layer 2 | 107-page map; revenue Table 7 p42, cost/GM Table 8 p43, segment note p98 |
| 7 | read_source_pages(TSLA, sec253, p36/42/43/55/98) | Layer 3 | All revenue/COGS/GM/deliveries/D&A numbers extracted (Tables 7, 8, 18, 64-66) |
| 8 | search_xbrl_facts(TSLA, Revenues, FY) | XBRL cross-check | FY2025 $94,827M / FY2024 $97,690M / FY2023 $96,773M, authority 3 — match p42/p55 |
| 9 | search_xbrl_facts(TSLA, CostOfGoodsAndServicesSold, FY) | XBRL concept check | 0 facts — TSLA does not file this concept |
| 10 | search_xbrl_facts(TSLA, CostOfRevenue, FY) | XBRL cross-check | FY2025 $77,733M / FY2024 $80,240M / FY2023 $79,113M, authority 3 — match p43/p55 |
| 11 | list_xbrl_concepts("cost of revenue") | Concept discovery | Empty result; discovery completed empirically via calls 9-10 |

All material numbers above trace to retrieval calls in this table; nothing was imported from memory or external sources. No price data used (`market_data_stage: none`). T-001 baseline figures appear only as reconciliation checks and are labeled as such. Retrieval was paced against the shared MCP rate limit (60 req/60s); two calls were retried after 61s backoff.
