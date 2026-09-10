---
artifact_id: "002-CGNX-supply-chain-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: CGNX
skill: supply-chain
mode: default
affix: supply-chain-map
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "8cb3ac1de486"
as_of: 2026-09-11
entity_claims:
  - entity: CGNX
    metric: revenue_usd
    value: 837547000
    unit: USD
    period: FY2023
    source: "10-K:page59"
    retrieved_at: 2026-09-11
  - entity: CGNX
    metric: revenue_usd
    value: 914515000
    unit: USD
    period: FY2024
    source: "10-K:page59"
    retrieved_at: 2026-09-11
  - entity: CGNX
    metric: revenue_usd
    value: 994359000
    unit: USD
    period: FY2025
    source: "10-K:page59"
    retrieved_at: 2026-09-11
  - entity: CGNX
    metric: gross_margin_pct
    value: 71.8
    unit: pct
    period: FY2023
    source: "XBRL:RFCCExcludingAssessedTax+COGSandServicesSold"
    retrieved_at: 2026-09-11
  - entity: CGNX
    metric: gross_margin_pct
    value: 68.4
    unit: pct
    period: FY2024
    source: "XBRL:RFCCExcludingAssessedTax+COGSandServicesSold"
    retrieved_at: 2026-09-11
  - entity: CGNX
    metric: gross_margin_pct
    value: 66.9
    unit: pct
    period: FY2025
    source: "XBRL:RFCCExcludingAssessedTax+COGSandServicesSold"
    retrieved_at: 2026-09-11
citations:
  - "CGNX sec93 page3 — end-market mix ~85%"
  - "CGNX sec93 page4 — end markets, automotive headwinds, robot guidance"
  - "CGNX sec93 page7 — OneVision, VisionPro, DataMan product structure"
  - "CGNX sec93 page8 — CM structure, in-house optics, 67% non-US, services <10%"
  - "CGNX sec93 page11 — China/tariff/BIS/Taiwan-chip risks"
  - "CGNX sec93 page15 — supply-chain risks, Indonesia CM fire, single-source components"
  - "CGNX sec93 page16 — large-customer concentration, seasonality"
  - "CGNX sec93 page24 — MD&A: revenue +9%, GM 67/68/72, $13M one-time, services <10%"
  - "CGNX sec93 page25 — geo revenue + gross profit tables, GM decline drivers"
  - "CGNX sec93 page56 — $57.7M purchase orders, CM component buy-backs"
  - "CGNX sec93 page59 — 3-yr geo/revenue-type disaggregation, channel-partner license"
  - "CGNX sec93 page71 — single-customer 15%/10%, one segment"
  - "CGNX sec93 page72 — 3-yr segment expense disaggregation (COR/GP/RD&E/SG&A)"
  - "CGNX sec93 page73 — Moritex PPA $296.1M, 2022 fire $8.0M recoveries"
  - "CGNX sec93 page74 — Moritex Japan trading divestiture, $500M buyback"
pillars_addressed: [PIL-1, PIL-2]
claim_state: pinned
key_metrics:
  revenue_fy2023_usd: 837547000
  revenue_fy2024_usd: 914515000
  revenue_fy2025_usd: 994359000
  cost_of_revenue_fy2023_usd: 236306000
  cost_of_revenue_fy2024_usd: 288721000
  cost_of_revenue_fy2025_usd: 328966000
  gross_margin_fy2023_pct: 71.8
  gross_margin_fy2024_pct: 68.4
  gross_margin_fy2025_pct: 66.9
  gm_3fy_change_pp: -4.9
  non_us_revenue_share_fy2025_pct: 67
  greater_china_revenue_share_fy2025_pct: 16
  single_customer_revenue_share_fy2025_pct: 15
  service_revenue_share_fy2025_pct_lt: 10
  application_specific_solutions_share_fy2025_pct: 11.5
conclusions:
  - "CGNX is the automation-side sensing profit-pool reference: 66.9% FY2025 gross margin, -4.9pp over FY2023-FY2025 (PIL-1b input)."
  - "Asset-light supply structure: EMS contract manufacturing (Indonesia/Malaysia) + in-house optics (China/Vietnam) + software loading at own DCs."
  - "Demand concentration: 4 end markets ~85% of revenue; single customer 15% (2025); 67% of revenue non-US."
  - "Recurring/software share is low and not separately disclosed: services <10%; software largely embedded with hardware."
  - "Robotics exposure is INDIRECT (factory-automation vision, robot guidance) — no humanoid robotics revenue claim can be made from filings."
facts_count: 32
deducted_count: 7
views_count: 6
citation_count: 15
---

# CGNX — Supply-Chain Map (skill: supply-chain, mode: default)

## Executive Summary

Cognex (CGNX) is an asset-light industrial machine-vision company: most hardware
(vision systems, sensors, barcode readers) is assembled by EMS contractors in
Indonesia and Malaysia, optical components (lenses/lighting) are made in-house in
China and Vietnam via the 2023 Moritex acquisition, and Cognex loads software and
does final QC at its own distribution centers ([FACT] https://agentii.ai/v/CGNX/sec93/8).
Demand is concentrated: logistics, packaging, consumer electronics, and automotive
are ~85% of 2025 revenue ([FACT] https://agentii.ai/v/CGNX/sec93/3), one customer is
15% of 2025 revenue ([FACT] https://agentii.ai/v/CGNX/sec93/71), and 67% of revenue
is non-US ([FACT] https://agentii.ai/v/CGNX/sec93/8). Recurring revenue is thin —
services are <10% of revenue and software is mostly embedded with hardware
([FACT] https://agentii.ai/v/CGNX/sec93/24). For the thesis, CGNX is the
automation-side **sensing-layer profit-pool reference** (PIL-1): FY2025 revenue
$994.4M at 66.9% gross margin, a **-4.9pp decline from FY2023's 71.8%** — the
PIL-1b gap-change input ([DEDUCTED] https://agentii.ai/v/CGNX/sec93/72). Robotics
exposure is **indirect** (factory-automation vision and robot guidance, no
humanoid-robotics revenue identifiable in filings).

## Data Sources

- **Layer 1**: `search_sec_filings` CGNX 10-K index → FY2025 10-K = `sec93`
  (filed 2026-02-12, accession 0000851205-26-000012); FY2024 = `sec92`; FY2023 = `sec91`.
- **Layer 2**: `read_source_outline` on `sec93` (82 pages mapped).
- **Layer 3**: `read_source_pages` on `sec93` pages 3, 4, 5, 7, 8, 11, 15, 16,
  24, 25, 56, 59, 71, 72, 73, 74.
- **XBRL** (`search_xbrl_facts`): `RevenueFromContractWithCustomerExcludingAssessedTax`
  (single revenue concept per task) and `CostOfGoodsAndServicesSold`, multi-period
  FY2023/FY2024/FY2025, authority-3 (10-K) facts cross-checked against the FY2025
  10-K note tables.
- **Preflight**: `search_companies` (CIK 0000851205, industrial.machinery.machine_vision),
  `get_ticker_coverage`, `get_company_fiscal_calendar`.

## Analysis

### 1. Hardware/software supply structure [FACT]

- Most hardware products — vision systems, vision sensors, barcode readers — are
  manufactured via third-party contractors; the majority of component procurement,
  system assembly, and initial testing is performed by electronics manufacturing
  services (EMS) suppliers, with primary contract manufacturers in **Indonesia and
  Malaysia** ([FACT] https://agentii.ai/v/CGNX/sec93/8).
- Assembled goods are routed to Cognex distribution centers (US, Europe, Asia),
  where Cognex personnel **load software, perform additional assembly/image
  alignment, and QC** before shipping ([FACT] https://agentii.ai/v/CGNX/sec93/8).
- Optical components (lenses, lighting) are manufactured **in-house at plants in
  China and Vietnam**, a capability added by the October 2023 acquisition of
  Moritex Corporation (Japan-based premium optical component maker; purchase price
  $296.1M allocated, incl. $151.5M goodwill, $64.8M customer relationships,
  $32.3M completed technologies amortized to cost of revenue over 9 years)
  ([FACT] https://agentii.ai/v/CGNX/sec93/73).
- Supply-side dependency: a "significant portion" of inventory purchase orders and
  preauthorized component commitments sit with the **primary contract
  manufacturer**; Cognex bought back non-cancelable/non-returnable components
  worth $5.0M (2025), $17.5M (2024), $10.6M (2023) under those terms
  ([FACT] https://agentii.ai/v/CGNX/sec93/56). Outstanding inventory purchase
  orders at 12/31/2025: **$57.7M**, primarily for expected 2026 sales
  ([FACT] https://agentii.ai/v/CGNX/sec93/56).
- Certain Cognex products use **single-source components**, and integrated-circuit
  chips from Taiwan-based vendors are flagged as a China-Taiwan escalation risk
  ([FACT] https://agentii.ai/v/CGNX/sec93/15).
- Historical bottleneck event: a June 2022 fire at the primary CM's Indonesian
  plant destroyed significant Cognex inventories; shipments were delayed through
  H1-2023, with $8.0M recoveries recognized in 2023 ($2.5M business-interruption
  insurance + $5.5M settlement) ([FACT] https://agentii.ai/v/CGNX/sec93/73).
- Software: VisionPro licenses (usable with third-party cameras), OneVision cloud
  platform launched 2025 (AI model training + edge deployment), DataMan barcode
  readers — software revenue is **not separately disclosed**; it is embedded in
  hardware sales ([FACT] https://agentii.ai/v/CGNX/sec93/7).

### 2. Customer and industry concentration [FACT]

- Largest end markets — logistics, packaging, consumer electronics, automotive —
  combined ≈ **85% of 2025 revenue** ([FACT] https://agentii.ai/v/CGNX/sec93/3).
- One customer = **15% of revenue in 2025** (10% in 2024, <10% in 2023);
  its receivables were 10% of AR at 12/31/2024 ([FACT] https://agentii.ai/v/CGNX/sec93/71).
- Geographic revenue (customer domicile), FY2025: Americas $407.3M (41%),
  Europe $251.6M (25%), Greater China $158.5M (16%), Other Asia $177.0M (18%)
  ([FACT] https://agentii.ai/v/CGNX/sec93/25). 3-year series on
  https://agentii.ai/v/CGNX/sec93/59 confirms $837.5M/$914.5M/$994.4M totals.
- **67% of 2025 revenue from non-US customers** ([FACT] https://agentii.ai/v/CGNX/sec93/8).
  Greater China revenue fell 3% in 2025, in part on customer procurement shifts
  out of China ([FACT] https://agentii.ai/v/CGNX/sec93/25). US tariffs on Chinese
  components have raised costs (not material to total cost of revenue to date);
  BIS export controls have negatively impacted China revenue
  ([FACT] https://agentii.ai/v/CGNX/sec93/11).
- 2025 growth (+9%) was driven by logistics and consumer electronics, partially
  offset by automotive weakness ([FACT] https://agentii.ai/v/CGNX/sec93/24).

### 3. Recurring/software share of revenue [FACT + DEDUCTED]

- Service revenue (maintenance/support, consulting, training) is **<10% of total
  revenue for all periods presented** ([FACT] https://agentii.ai/v/CGNX/sec93/24).
- Revenue by type, FY2025: standard products and services $880.0M (88.5%) vs
  application-specific customer solutions $114.3M (11.5%)
  ([FACT] https://agentii.ai/v/CGNX/sec93/59).
- The only quantified software-recurring element: a 2025 strategic channel
  partnership (medical lab automation) with exclusive hardware+licensed-software
  rights through 2030 and **annual minimum license fees**; ~$13M one-time revenue
  recognized in 2025 on software access + inventory transfer
  ([FACT] https://agentii.ai/v/CGNX/sec93/59).
- [DEDUCTED] Recurring revenue share ≈ 10–12% of revenue (services <10% plus
  annual license fees <$13M); the business model is predominantly transactional
  hardware+embedded-software sales — a structurally different profile from ISRG's
  recurring base used elsewhere in the thesis.

### 4. Gross-margin series — PIL-1b gap-change input

| FY | Revenue ($K) | Cost of revenue ($K) | Gross profit ($K) | GM (computed) | GM (filing) |
|---|---|---|---|---|---|
| 2023 | 837,547 | 236,306 | 601,241 | 71.8% | 72% |
| 2024 | 914,515 | 288,721 | 625,794 | 68.4% | 68% |
| 2025 | 994,359 | 328,966 | 665,393 | 66.9% | 67% |

- Revenue: XBRL `RevenueFromContractWithCustomerExcludingAssessedTax`, authority-3
  facts ([FACT] via search_xbrl_facts; filing cross-check
  https://agentii.ai/v/CGNX/sec93/59 and https://agentii.ai/v/CGNX/sec93/72).
- Cost of revenue / gross profit: 10-K Note 20 disaggregation
  ([FACT] https://agentii.ai/v/CGNX/sec93/72), cross-checked to XBRL
  `CostOfGoodsAndServicesSold` authority-3 facts.
- GM computed from XBRL: 71.8% → 68.4% → 66.9%; filing-rounded 72% → 68% → 67%
  ([FACT] https://agentii.ai/v/CGNX/sec93/24). **3-FY change: -4.9pp** [DEDUCTED].
- Decline drivers stated by the company: a **$13M excess-and-obsolete inventory
  charge in Q4 2025** (strategic product-portfolio review under new leadership),
  less favorable industry mix, and tariffs ([FACT] https://agentii.ai/v/CGNX/sec93/25).
- [DEDUCTED] Cost of revenue includes acquired-technology amortization of
  $12.4M (2025), $12.5M (2024), $7.1M (2023) — the Moritex step-up weighs ~1.2pp
  on FY2025 GM, so the FY2025 66.9% understates underlying product margin
  ([FACT source] https://agentii.ai/v/CGNX/sec93/72; the pp impact is [DEDUCTED]).
- [VIEW] For PIL-1b: CGNX sensing-layer GM fell ~4.9pp over FY2023→FY2025 while
  its revenue grew 18.7% — a margin-dilution pattern driven by mix, tariffs, and
  one-off inventory charges rather than a structural BOM shift; pairing against
  motion-layer GM series (PH) should treat the $13M E&O charge and Moritex
  amortization as one-off vs structural components.

### 5. Fiscal-calendar pairing (4-4-5, Sunday quarter-ends) [FACT]

Cognex reports on a 4-4-5 fiscal calendar with **Sunday quarter-ends** (XBRL
`period_end` values, all verified this run):

| Fiscal period | period_start | period_end |
|---|---|---|
| FY2023 Q1 | 2023-01-01 | 2023-04-02 |
| FY2023 Q2 | 2023-04-03 | 2023-07-02 |
| FY2023 Q3 | 2023-07-03 | 2023-10-01 |
| FY2024 Q1 | 2024-01-01 | 2024-03-31 |
| FY2024 Q2 | 2024-04-01 | 2024-06-30 |
| FY2024 Q3 | 2024-07-01 | 2024-09-29 |
| FY2025 Q1 | 2025-01-01 | 2025-03-30 |
| FY2025 Q2 | 2025-03-31 | 2025-06-29 |
| FY2025 Q3 | 2025-06-30 | 2025-09-28 |
| FY2026 Q1 | 2026-01-01 | 2026-04-05 |
| FY2026 Q2 | 2026-04-06 | 2026-07-05 |

**Pairing statement**: the GM series above aligns at the fiscal-year level —
FY2023 = period_end 2023-12-31, FY2024 = 2024-12-31, FY2025 = 2025-12-31 (all
authority-3 10-K facts). Quarterly facts must be paired by `period_end`, not by
calendar quarter (e.g., FY2026 Q2 ends **2026-07-05**, matching the task's
example). The MCP fiscal-calendar endpoint returned calendar-month quarter-ends
(2025-03-31 etc.), which **do not match** the filing-XBRL period_end values — the
XBRL period_end is authoritative for quarter pairing.

### 6. Robotics relevance and honest labeling [VIEW]

- [FACT] Cognex discloses no humanoid-robotics product or customer; its robotics
  exposure is **indirect**: machine vision for "guiding robot assembly" in
  automotive ([FACT] https://agentii.ai/v/CGNX/sec93/4) and "3D measurement for
  robotic guidance" in other end markets ([FACT] https://agentii.ai/v/CGNX/sec93/5).
- [VIEW] CGNX is best used in this thesis as the **industrial sensing-layer
  profit-pool reference** (PIL-1): a dedicated vision franchise earning 67–72%
  gross margins off an outsourced-assembly supply chain, evidencing that the
  sensing layer of the automation stack sustains premium economics even with
  hardware commoditization elsewhere in the stack.
- [DEDUCTED] For PIL-2 (non-China vs China BOM cost ratio): CGNX's supply chain
  shows **dual optionality** — optics made in both China and Vietnam, EMS
  assembly in Indonesia/Malaysia (neither in China), and Greater China revenue
  already declining (16% share) under BIS controls and customer procurement
  shifts. This is proxy evidence that a non-China sensing supply chain exists at
  scale, but CGNX discloses **no cost data** to quantify a ratio; treat as
  directional only.
- [VIEW] Bottleneck assessment: the single point of failure is the primary EMS
  contractor in Indonesia (2022 fire precedent, component buy-back obligations);
  single-source components and Taiwan-sourced ICs are the secondary
  dependencies.

## Key Metrics

| Metric | FY2023 | FY2024 | FY2025 | Source |
|---|---|---|---|---|
| Revenue ($K) | 837,547 | 914,515 | 994,359 | XBRL RFCC; [sec93/59](https://agentii.ai/v/CGNX/sec93/59) |
| Cost of revenue ($K) | 236,306 | 288,721 | 328,966 | XBRL COGSandServicesSold; [sec93/72](https://agentii.ai/v/CGNX/sec93/72) |
| Gross profit ($K) | 601,241 | 625,794 | 665,393 | [sec93/72](https://agentii.ai/v/CGNX/sec93/72) |
| **Gross margin** | **71.8%** | **68.4%** | **66.9%** | computed; filing 72/68/67 [sec93/24](https://agentii.ai/v/CGNX/sec93/24) |
| 3-FY GM change | — | — | **-4.9pp** | computed (PIL-1b input) |
| Revenue growth YoY | — | +9.2% | +8.7% | computed from above; +9% stated [sec93/24](https://agentii.ai/v/CGNX/sec93/24) |

Supporting metrics (FY2025 unless noted):

| Metric | Value | Source |
|---|---|---|
| Non-US revenue share | 67% | [sec93/8](https://agentii.ai/v/CGNX/sec93/8) |
| Greater China revenue share (FY25 / FY24) | 16% / 18% | [sec93/25](https://agentii.ai/v/CGNX/sec93/25) |
| Single-customer revenue share (FY25 / FY24) | 15% / 10% | [sec93/71](https://agentii.ai/v/CGNX/sec93/71) |
| Top-4 end-market revenue share | ~85% | [sec93/3](https://agentii.ai/v/CGNX/sec93/3) |
| Service revenue share | <10% (all periods) | [sec93/24](https://agentii.ai/v/CGNX/sec93/24) |
| Application-specific solutions share | 11.5% | [sec93/59](https://agentii.ai/v/CGNX/sec93/59) |
| Inventory purchase orders outstanding | $57.69M | [sec93/56](https://agentii.ai/v/CGNX/sec93/56) |
| CM component buy-backs (25/24/23) | $5.0M / $17.5M / $10.6M | [sec93/56](https://agentii.ai/v/CGNX/sec93/56) |
| Moritex acquisition (Oct 2023) | ~$270M EV; $296.1M PPA | [sec93/73](https://agentii.ai/v/CGNX/sec93/73) |
| Fire recoveries (2023) | $8.0M | [sec93/73](https://agentii.ai/v/CGNX/sec93/73) |
| RD&E spend (25/24/23) | $139.0M / $139.8M / $139.4M | [sec93/72](https://agentii.ai/v/CGNX/sec93/72) |

## Coverage Gaps & Citations

**Coverage gaps:**

1. **Recurring/software revenue** — not separately disclosed; only the <10%
   service cap and the $13M one-time license are quantified. A precise
   recurring-share metric cannot be constructed from filings.
2. **Supplier identity** — CMs and component vendors are unnamed in the 10-K
   ("primary contract manufacturer in Indonesia"), so supplier-level
   concentration cannot be quantified.
3. **China vs non-China cost split** (PIL-2 proxy) — no cost data disclosed;
   only the dual-country manufacturing footprint is visible.
4. **End-market revenue split by industry** — only the ~85% aggregate for four
   industries is disclosed; no per-industry revenue table.
5. **Price data** — excluded per audit mandate.

**Citation index** (all https://agentii.ai/v/CGNX/sec93/{page}):

1. page3 — company overview, ~85% end-market concentration
2. page4 — end markets, automotive headwinds, robot-guidance applications
3. page7 — OneVision / VisionPro / DataMan / accessories
4. page8 — operations: EMS structure, in-house optics, 67% non-US, services <10%
5. page11 — international/China/tariff/BIS/Taiwan-chip risks
6. page15 — supply-chain risks, Indonesia fire, single-source components
7. page16 — large-customer concentration, seasonality
8. page24 — MD&A: revenue +9%, GM 67/68/72, $13M one-time, services <10%
9. page25 — geographic revenue + gross profit tables, GM-decline drivers
10. page56 — $57.7M purchase orders, CM component buy-back history
11. page59 — 3-yr geographic and revenue-type disaggregation, license deal
12. page71 — one segment; single-customer 15%/10%; long-lived assets by region
13. page72 — 3-yr segment expense disaggregation (COR/GP/RD&E/SG&A)
14. page73 — Moritex PPA, fire loss-recovery $8.0M
15. page74 — subsequent events: Moritex Japan trading divestiture ($10–12M
    target), $500M repurchase authorization, $0.085 dividend

## Verification

| # | Claim | Expected | Retrieved | Status |
|---|---|---|---|---|
| 1 | FY2025 revenue = $994.4M (entity map anchor) | 994,359,000 | XBRL RFCC authority-3 = 994,359,000; sec93/59 + sec93/72 = 994,359 | PASS |
| 2 | Revenue sum of geo segments = total | 994,359 | 407,288+251,638+158,456+176,977 = 994,359 | PASS |
| 3 | Revenue-type sum = total | 994,359 | 880,015+114,344 = 994,359 | PASS |
| 4 | Gross profit = revenue − cost of revenue, 3 yrs | 601,241 / 625,794 / 665,393 | matches for all three FYs | PASS |
| 5 | GM% vs filing-stated | 72/68/67 | computed 71.8/68.4/66.9 (rounds to filing) | PASS |
| 6 | XBRL COR cross-check vs note table | 236,306 / 288,721 / 328,966 | identical (authority-3 facts from cgnx-20251231.htm) | PASS |
| 7 | 4-4-5 Sunday quarter-end calendar | 2026-07-05 Q2 end | XBRL period_end 2026-07-05 (cgnx-20260705.htm) confirmed; 2023/2024/2025 Sunday ends confirmed | PASS |
| 8 | No price data used | none | none retrieved | PASS |
| 9 | Single revenue concept used | RFCCExcludingAssessedTax only | RFCCExcludingAssessedTax only (COR = separate expense concept, not revenue) | PASS |

All numbers in this artifact trace to retrieval calls made in this run (XBRL
facts via `search_xbrl_facts`, pages via `read_source_pages` on sec93) and are
inline-cited. Uncited = void per audit mandate.
