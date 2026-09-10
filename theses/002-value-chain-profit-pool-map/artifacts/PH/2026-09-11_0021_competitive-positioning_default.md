---
artifact_id: "002-PH-competitive-positioning-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: PH
skill: competitive-positioning
mode: default
affix: competitive-structure
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "61f794be22a5"
as_of: 2026-09-11
entity_claims:
  - entity: PH
    metric: motion_systems_revenue_usd
    value: 3580000000
    unit: USD
    period: FY2026
    source: "10-K:page44"
    retrieved_at: 2026-09-11
    note: "[FACT] sec166 Motion Systems technology platform, Diversified Industrial"
  - entity: PH
    metric: diversified_industrial_segment_operating_margin_pct
    value: 23.8
    unit: pct
    period: FY2026
    source: "10-K:page25"
    retrieved_at: 2026-09-11
    note: "[FACT] sec166; FY2025 22.8"
  - entity: PH
    metric: consolidated_gross_margin_pct
    value: 37.7
    unit: pct
    period: FY2026
    source: "10-K:page23"
    retrieved_at: 2026-09-11
    note: "[FACT] sec166; FY2025 36.9; includes $84M IEEPA tariff-refund benefit (~39bps)"
  - entity: PH
    metric: consolidated_gross_margin_pct
    value: 35.8
    unit: pct
    period: FY2024
    source: "10-K:page35"
    retrieved_at: 2026-09-11
    note: "[DEDUCTED] (19,930-12,802)/19,930 from sec166 income statement"
  - entity: PH
    metric: diversified_industrial_segment_operating_margin_pct
    value: 22.0
    unit: pct
    period: FY2024
    source: "10-K:page67"
    retrieved_at: 2026-09-11
    note: "[DEDUCTED] 3,176/14,458 from sec166 segment table"
  - entity: PH
    metric: motion_systems_share_of_di_revenue_pct
    value: 24.8
    unit: pct
    period: FY2026
    source: "10-K:page44"
    retrieved_at: 2026-09-11
    note: "[DEDUCTED] 3,580/14,438; derived arithmetic on map metrics"
citations:
  - {citation_id: sec166, page: 3, url: "https://agentii.ai/v/PH/sec166/3"}
  - {citation_id: sec166, page: 5, url: "https://agentii.ai/v/PH/sec166/5"}
  - {citation_id: sec166, page: 10, url: "https://agentii.ai/v/PH/sec166/10"}
  - {citation_id: sec166, page: 11, url: "https://agentii.ai/v/PH/sec166/11"}
  - {citation_id: sec166, page: 12, url: "https://agentii.ai/v/PH/sec166/12"}
  - {citation_id: sec166, page: 23, url: "https://agentii.ai/v/PH/sec166/23"}
  - {citation_id: sec166, page: 25, url: "https://agentii.ai/v/PH/sec166/25"}
  - {citation_id: sec166, page: 35, url: "https://agentii.ai/v/PH/sec166/35"}
  - {citation_id: sec166, page: 44, url: "https://agentii.ai/v/PH/sec166/44"}
  - {citation_id: sec166, page: 67, url: "https://agentii.ai/v/PH/sec166/67"}
  - {citation_id: ect72, page: 1, url: "https://agentii.ai/v/PH/ect72/1"}
  - {citation_id: ect72, page: 2, url: "https://agentii.ai/v/PH/ect72/2"}
  - {citation_id: ect72, page: 5, url: "https://agentii.ai/v/PH/ect72/5"}
  - {citation_id: ect72, page: 6, url: "https://agentii.ai/v/PH/ect72/6"}
pillars_addressed: [PIL-1, PIL-2]
claim_state: pinned
key_metrics:
  motion_systems_revenue_fy2026_usd: 3580000000
  diversified_industrial_operating_margin_fy2026_pct: 23.8
  consolidated_gross_margin_fy2026_pct: 37.7
  consolidated_gross_margin_fy2025_pct: 36.9
  consolidated_gross_margin_fy2024_pct: 35.8
  total_backlog_jun2026_usd: 12800000000
  diversified_industrial_backlog_jun2026_usd: 4332000000
  adjusted_segment_operating_margin_fy2026_pct: 27.3
  fy2031_adjusted_segment_operating_margin_target_pct: 30
  apac_revenue_fy2026_usd: 2711000000
  us_revenue_fy2026_usd: 13819000000
  rd_expense_fy2026_usd: 267000000
  iiepa_tariff_refund_fy2026_usd: 84000000
conclusions:
  - "Motion Systems is PH's smallest DI platform ($3.58B, 24.8% of DI revenue) and the only one still below its FY2024 revenue level; pricing power evidence is strong at the segment level but the platform-level margin is not disclosed."
  - "PH's disclosed competitive set in motion/control is entirely non-Chinese (Bosch Rexroth, SMC, Festo, Danfoss, IMI/Norgren, etc.); China appears in filings as a trade-policy risk and supply risk (rare earths), not as a named competitive threat — PIL-2 falsifier cannot be tested from filing evidence alone."
  - "Barriers rest on application engineering, distribution reach, aftermarket content, and breadth of interconnected technologies — explicitly NOT on patents, which the company states are not material to any extent."
facts_count: 57
deducted_count: 11
views_count: 3
citation_count: 14
---

# PH — Competitive Positioning (mode: default, affix: competitive-structure)

## Executive Summary

Parker-Hannifin's motion/control layer shows durable pricing power: consolidated gross margin rose to 37.7% in FY2026 from 36.9% (FY2025) and 35.8% (FY2024) ([FACT] https://agentii.ai/v/PH/sec166/23; [DEDUCTED] https://agentii.ai/v/PH/sec166/35), with Diversified Industrial (DI) segment operating margin at 23.8%, up 100 bps, "primarily driven by favorable pricing" ([FACT] https://agentii.ai/v/PH/sec166/25). Motion Systems — the actuation platform — is $3.58B (24.8% of DI), up 7.2% YoY but still below FY2024 ([FACT]/[DEDUCTED] https://agentii.ai/v/PH/sec166/44). Barriers are engineering-, distribution- and aftermarket-based; patents are explicitly non-material ([FACT] https://agentii.ai/v/PH/sec166/5). On import substitution: PH's named competitors are entirely non-Chinese, China appears only as trade-policy/supply risk, and Asia Pacific grew +16% organically in Q4 ([FACT] https://agentii.ai/v/PH/sec166/5, https://agentii.ai/v/PH/ect72/2) — no filing evidence of Chinese motion-control displacement, but the PIL-2 falsifier is untestable from filings alone. Management raised the margin target 300 bps to 30% by FY2031 after hitting the FY2029 target early ([FACT] https://agentii.ai/v/PH/ect72/1).

## Core Analysis

### PIL-1 — Motion layer's barriers to substitution (durability evidence)

**Competitive structure of the motion/actuation layer.** PH's DI segment ($14,438M FY2026, 67% of total $21,499M sales) ([FACT] https://agentii.ai/v/PH/sec166/44, https://agentii.ai/v/PH/sec166/3) disaggregates into three technology platforms: Motion Systems $3,580M, Flow & Process Control $4,810M, and Filtration & Engineered Materials $6,048M ([FACT] https://agentii.ai/v/PH/sec166/44). Motion Systems is the smallest platform at 24.8% of DI revenue ([DEDUCTED] 3,580/14,438 from https://agentii.ai/v/PH/sec166/44). Its trajectory is the weakest of the three: $3,341M in FY2025 and $3,706M in FY2024 means +7.2% YoY in FY2026 but still -3.4% below FY2024 ([DEDUCTED] arithmetic from https://agentii.ai/v/PH/sec166/44) — a slower recovery than siblings, consistent with transportation/off-highway softness called out in MD&A ([FACT] https://agentii.ai/v/PH/sec166/25).

**Market position.** PH asserts it is "one of the market leaders in most of the major markets for our most significant Diversified Industrial Segment products" and that "no single competitor competes with the Company with respect to all the products we manufacture and sell" ([FACT] https://agentii.ai/v/PH/sec166/5). Named primary DI competitors are: Bosch Rexroth AG, Copeland, Danaher, Danfoss, Donaldson, Emerson/ASCO, Festo, Freudenberg-NOK, Gates, IMI/Norgren, SMC, Swagelok, Trelleborg ([FACT] https://agentii.ai/v/PH/sec166/5). Competition factors are "product quality and innovation, customer experience, manufacturing and distribution capability, aftermarket support, and price competitiveness" ([FACT] https://agentii.ai/v/PH/sec166/5). Notably, the named competitor set is US/EU/Japan only — no Chinese motion suppliers appear in PH's own disclosure of primary competitors.

**Barriers.** The moat is not IP: "We do not depend on any single patent, trademark, copyright, trade secret or license or group of patents... to any material extent" ([FACT] https://agentii.ai/v/PH/sec166/5). Barriers are instead: (a) application-engineering content and "interconnected technologies" (hydraulics, pneumatics, electromechanical, filtration, fluid & gas handling, process control, engineered materials, climate control) ([FACT] https://agentii.ai/v/PH/sec166/5); (b) distribution scale — "several hundred thousand OEMs and distribution customer locations" ([FACT] https://agentii.ai/v/PH/sec166/3); (c) aftermarket content — the FGC acquisition is framed as increasing "filtration aftermarket by 500 basis points" ([FACT] https://agentii.ai/v/PH/ect72/1); and (d) decentralized application engineering paired with customer co-development ("deep partnerships with our customers to develop innovative products") ([FACT] https://agentii.ai/v/PH/sec166/5). R&D expense was $267M in FY2026 ([FACT] XBRL FY2026 10-K via get_company_financials), only 1.2% of sales ([DEDUCTED] 267/21,499) — the engineering barrier is in application engineering and field content, not central R&D. Switching-cost evidence is moderate: backlog is short-cycle — "approximately 70% of our backlog at June 30, 2026 is scheduled for delivery in the succeeding twelve months" ([FACT] https://agentii.ai/v/PH/sec166/5) — so customers are not locked in for multi-year periods in the industrial layer; retention must come from specification wins and aftermarket, not contract lock.

**Pricing power.** Three lines of evidence. (1) Margin resilience through an inflationary cycle: consolidated GM 37.7% (FY26) vs 36.9% (FY25) vs 35.8% (FY24) ([FACT] https://agentii.ai/v/PH/sec166/23; [DEDUCTED] FY2024 from https://agentii.ai/v/PH/sec166/35). Caveat: FY2026 GM includes a one-time $84M IEEPA tariff refund that reduced cost of sales ([FACT] https://agentii.ai/v/PH/sec166/23) — ex-refund GM is ~37.3%, still +40 bps YoY ([DEDUCTED]). (2) DI segment margin expansion of 100 bps was "primarily driven by favorable pricing and benefits from prior year divestitures, partially offset by unfavorable product mix, increased material costs and higher intangible amortization" — i.e., price more than offset material-cost inflation ([FACT] https://agentii.ai/v/PH/sec166/25); International margin +90 bps "primarily driven by favorable mix and pricing" ([FACT] https://agentii.ai/v/PH/sec166/25). (3) Management's own pricing read: industrial "back to a more normal pricing environment" while aerospace has "still pricing opportunity... there's still some opportunity in aerospace", and North American industrial growth in the FY2027 guide "is all volume" — implying prior price increases are being held, not given back ([FACT] https://agentii.ai/v/PH/ect72/5). Q4 FY2026 incrementals were 40% and adjusted segment operating margin hit a record 28.0% ([FACT] https://agentii.ai/v/PH/ect72/2). The FY2029 adjusted segment operating margin target was achieved early (FY2026: 27.3%, +120 bps), and the target was raised 300 bps to 30% by FY2031 ([FACT] https://agentii.ai/v/PH/ect72/1). Record backlog of $12.8B total ([FACT] https://agentii.ai/v/PH/sec166/5) and DI backlog of $4,332M (vs $3,655M, +18.5% ([DEDUCTED] arithmetic from https://agentii.ai/v/PH/sec166/25)) provide demand-side support for price maintenance.

[VIEW] PH's actuation-layer pricing power is segment-level evidence, not platform-level: Motion Systems margin is not disclosed, and Motion Systems is the only DI platform still below FY2024 revenue, so the motion-specific durability inference is weaker than the DI-level inference.

### PIL-2 — Import-substitution dynamics (Chinese motion-control competition)

**China as trade-policy risk, not named competitor.** PH's China disclosure is confined to risk factors: "possible restrictions on trade and/or obstacles to conducting business in China" and "uncertainty about the future relationship between the U.S. and China, including with respect to trade policies, treaties, government regulations and tariffs" ([FACT] https://agentii.ai/v/PH/sec166/10); "Any increased trade barriers or restrictions on global trade, including trade with China or among North American trading partners, could adversely impact our business" ([FACT] https://agentii.ai/v/PH/sec166/11). The tariff environment is live: in February 2026 the U.S. Supreme Court ruled IEEPA tariffs unauthorized, and PH recognized the $84M refund in Q4 FY2026 ([FACT] https://agentii.ai/v/PH/sec166/23).

**Supply-side exposure.** PH "rel[ies] on a limited number of suppliers for certain critical components, such as specialty electronics, rare earths, specialty chemicals, aerospace super alloys and filtration media" ([FACT] https://agentii.ai/v/PH/sec166/11) — rare earths being the most China-concentrated input class; and raw-material price pass-through has friction: "we may be unable to increase the prices of our products due to pricing pressure, contract terms (including fixed-price contracts) or other factors" ([FACT] https://agentii.ai/v/PH/sec166/11). The competitive risk factor cites only "increased competition in the markets we serve" generically ([FACT] https://agentii.ai/v/PH/sec166/12).

**Geographic footprint.** Non-US selling locations = ~36% of net sales in each of FY2024-26 ([FACT] https://agentii.ai/v/PH/sec166/10). Asia Pacific revenue was $2,711M in FY2026 ([FACT] https://agentii.ai/v/PH/sec166/44), 12.6% of consolidated ([DEDUCTED]); US revenue was $13,819M and "No country other than the United States represents greater than 10% of consolidated sales" ([FACT] https://agentii.ai/v/PH/sec166/67). Asia Pacific organic growth was +16% in Q4 FY2026 — the strongest region — driven by electronics/semiconductor and in-plant demand ([FACT] https://agentii.ai/v/PH/ect72/2), i.e., PH is currently gaining share in Asia rather than being displaced there.

[VIEW] On the evidence PH itself publishes, Chinese motion-control suppliers do not yet register as primary competitors in its markets (the full named-competitor list is non-Chinese), and China shows up as trade-policy and input-supply risk. However, this is consistent with both (a) genuine competitive insulation via certification/specification barriers and (b) disclosure lag on emerging entrants. The PIL-2 falsifier (non-China/China humanoid BOM cost ratio ≥ 2.0) cannot be tested from PH filings — no BOM/teardown data exists in the corpus; per the thesis map this stays proxy-only with a Deviation Register entry.

[VIEW] Certifications — often the strongest import-substitution barrier in motion/control (safety ratings, OEM qualification) — are barely discussed in PH's 10-K outside aerospace (FAA/ITAR context on https://agentii.ai/v/PH/sec166/16, not deep-read here). The absence of industrial-layer certification narrative in the filings is itself a coverage gap for PIL-1/PIL-2 barrier quantification.

### Adjacent competitive-structure signals (FY2026 10-K + Q4 call)

- Portfolio reshaping toward longer-cycle, higher-margin platforms: aerospace + engineered materials + filtration ≈ 65% of pro forma sales post-FGC ([FACT] https://agentii.ai/v/PH/ect72/1).
- CIRCOR A&D pending acquisition (~$270M CY26E revenue, >40% adjusted EBITDA margin pre-synergies, ~10%/ $26M synergies, 80% OEM, 50/50 commercial/defense) — "highest growth, highest margin acquisition to date" ([FACT] https://agentii.ai/v/PH/ect72/6).
- ~$15B capital deployed in FY2026 (Curtis $1.0B completed; ~$12B announced for FGC + CIRCOR) ([FACT] https://agentii.ai/v/PH/ect72/1, https://agentii.ai/v/PH/ect72/2).
- Data center exposure ≈1.5% of sales, growing (liquid-cooling hoses, couplings, manifolds) ([FACT] https://agentii.ai/v/PH/ect72/6).
- Aerospace segment (the counterexample of concentrated, certified competition): record $1.9B Q4 sales, +13.4% organic, 29.8% Q4 margin, backlog $8.5B ([FACT] https://agentii.ai/v/PH/ect72/2) — the certified end-market shows higher margins than industrial, supporting the certification-barrier thesis.

## Key Metrics

| Metric | FY2026 | FY2025 | FY2024 | Source |
|---|---|---|---|---|
| Motion Systems revenue ($M) | 3,580 | 3,341 | 3,706 | [FACT] https://agentii.ai/v/PH/sec166/44 |
| DI segment operating margin (%) | 23.8 | 22.8 | ~22.0 | [FACT]/[DEDUCTED] https://agentii.ai/v/PH/sec166/25, https://agentii.ai/v/PH/sec166/67 |
| Consolidated gross margin (%) | 37.7 | 36.9 | ~35.8 | [FACT]/[DEDUCTED] https://agentii.ai/v/PH/sec166/23, https://agentii.ai/v/PH/sec166/35 |
| Consolidated net sales ($M) | 21,499 | 19,850 | 19,930 | [FACT] https://agentii.ai/v/PH/sec166/35 |
| Total backlog, June 30 ($B) | 12.8 | 11.0 | — | [FACT] https://agentii.ai/v/PH/sec166/5 |
| DI backlog, June 30 ($M) | 4,332 | 3,655 | — | [FACT] https://agentii.ai/v/PH/sec166/25 |
| Adjusted segment operating margin (%) | 27.3 (record) | — | — | [FACT] https://agentii.ai/v/PH/ect72/1 |
| Q4 FY26 adjusted segment op margin (%) | 28.0 (+110 bps); incrementals 40% | — | — | [FACT] https://agentii.ai/v/PH/ect72/2 |
| FY2031 margin target (%) | 30 (+300 bps) | — | — | [FACT] https://agentii.ai/v/PH/ect72/1 |
| Asia Pacific revenue ($M) | 2,711 | 2,364 | 2,278 | [FACT] https://agentii.ai/v/PH/sec166/44 |
| US revenue ($M) | 13,819 | 12,853 | 12,862 | [FACT] https://agentii.ai/v/PH/sec166/67 |
| IEEPA tariff refund ($M) | 84 (Q4 FY26) | — | — | [FACT] https://agentii.ai/v/PH/sec166/23 |
| R&D expense ($M) | 267 | 240 | 253 | [FACT] XBRL via get_company_financials (FY2026 10-K) |
| Q4 FY26 orders (3-month comp) | NA +16%, Intl +24%, Aero +18% | — | — | [FACT] https://agentii.ai/v/PH/ect72/2 |
| Data center exposure (% of sales) | ~1.5 | ~1.0 | — | [FACT] https://agentii.ai/v/PH/ect72/6 |

## Coverage Gaps & Citations

**Coverage gaps**
1. Motion Systems platform-level margin/profitability is not disclosed (only DI-segment level) — platform durability cannot be measured directly.
2. No quantification of Chinese motion-control suppliers' market share, no BOM/teardown data in the corpus — PIL-2 falsifier (`nonchina_to_china_humanoid_bom_cost_ratio` ≥ 2.0) untestable from PH filings; proxy-only (per thesis map, Deviation Register).
3. Industrial-layer certification/specification barriers (UL, safety, OEM qualification) are not described in the FY2026 10-K — aerospace certification context exists but was not deep-read this run.
4. 10-K risk factors are generic on competition; no scenario quantification for import substitution.

**Citations index (all /v/ links used above)**
- https://agentii.ai/v/PH/sec166/3 — business overview, segments, distribution scale
- https://agentii.ai/v/PH/sec166/5 — competition, competitors, patents non-material, backlog
- https://agentii.ai/v/PH/sec166/10 — international risk, 36% non-US sales, China trade risk
- https://agentii.ai/v/PH/sec166/11 — China trade barriers, rare earths, price pass-through risk
- https://agentii.ai/v/PH/sec166/12 — competition/demand risk factors
- https://agentii.ai/v/PH/sec166/23 — consolidated results, GM 37.7%/36.9%, IEEPA $84M
- https://agentii.ai/v/PH/sec166/25 — DI segment results, margin drivers, backlog
- https://agentii.ai/v/PH/sec166/35 — 3-year income statement
- https://agentii.ai/v/PH/sec166/44 — revenue disaggregation (Motion Systems $3,580M; geography)
- https://agentii.ai/v/PH/sec166/67 — segment reporting, US sales, geographic note
- https://agentii.ai/v/PH/ect72/1 — FY2026 records, 30% FY2031 target, $15B deployment
- https://agentii.ai/v/PH/ect72/2 — Q4 segment detail, orders, backlog, FCF, FY27 guide
- https://agentii.ai/v/PH/ect72/5 — pricing commentary, NA industrial all-volume
- https://agentii.ai/v/PH/ect72/6 — data center, CIRCOR metrics

## Verification

| # | Claim | Type | Retrieved from | Verified |
|---|---|---|---|---|
| 1 | Motion Systems FY26 revenue $3,580M | FACT | read_source_pages sec166 page44 | PASS — table row |
| 2 | DI segment op margin 23.8% FY26 | FACT | read_source_pages sec166 page25 | PASS — table row |
| 3 | Consolidated GM 37.7% FY26 / 36.9% FY25 | FACT | read_source_pages sec166 page23 | PASS — MD&A table |
| 4 | GM 3-year trend (35.8% FY24) | DEDUCTED | page35 net sales/cost of sales (19,930/12,802) | PASS — arithmetic cross-check; FY26 implied 37.69% ≈ stated 37.7% |
| 5 | DI margin FY24 ~22.0% | DEDUCTED | page67 3,176/14,458 | PASS — arithmetic |
| 6 | Motion Systems share of DI 24.8% | DEDUCTED | page44 3,580/14,438 | PASS — arithmetic |
| 7 | Backlog $12.8B / DI $4,332M | FACT | page5, page25 | PASS — both tables read |
| 8 | IEEPA refund $84M, Feb-2026 SCOTUS ruling | FACT | page23 | PASS — MD&A text |
| 9 | Pricing commentary ("normal pricing environment" industrial; aerospace opportunity) | FACT | ect72 page5 | PASS — Q&A text |
| 10 | FY31 target 30% (+300 bps), FY29 hit early | FACT | ect72 page1 | PASS — prepared remarks |
| 11 | Q4: +8% organic, 28.0% margin, 40% incrementals, orders +19%/+12% | FACT | ect72 page2 | PASS — prepared remarks |
| 12 | APAC +16% organic Q4; APAC FY26 revenue $2,711M | FACT | ect72 page2 / page44 | PASS — both read |
| 13 | Rare earths among critical components | FACT | page11 | PASS — risk factor text |
| 14 | No Chinese suppliers in named primary competitors | FACT | page5 | PASS — full competitor list read |
| 15 | R&D $267M FY26, capex target 2.5% of sales | FACT | get_company_financials XBRL / ect72 page5 | PASS — XBRL fact + Q&A text |
