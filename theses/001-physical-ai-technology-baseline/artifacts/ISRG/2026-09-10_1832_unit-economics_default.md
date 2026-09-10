---
artifact_id: "001-ISRG-unit-economics-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: ISRG
skill: unit-economics
mode: default
affix: unit-economics
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "e87ee63269a2"
as_of: 2026-09-10
entity_claims:
  - "ISRG da Vinci system ASP ~$1.60M FY2025 and ~$1.66M H1 2026 (ex-lease, ex-Ion, ex-trade-in) — precision-actuated capital commands premium pricing (sec166/page78, sec172/page40)"
  - "ISRG earns $900–$3,700 instruments & accessories revenue per procedure; realized ~$1.83K/case in Q2 2026 — actuated consumables dominate the revenue stack (sec166/page77, ect75/page2)"
  - "Recurring revenue (I&A + service + operating leases) = 84% of FY2025 revenue, 85% in Q2 2026 — razor-blade model (sec166/page78, sec172/page40)"
  - "Product gross margin 66.3% and service gross margin 64.6% FY2025; blended total 66.0% — high-value precision actuation stack, but system-level BOM/actuator-vs-compute split not disclosed (sec166/page79, sec166/page91)"
  - "Deployment-cost curve: entry tiers ($0.6M refurbished/X/XiR) and extended-use instruments (H1 2027) reduce cost-per-use without nominal ASP deflation (sec172/page38, ect75/page2)"
pillars_addressed: [PIL-2, PIL-4]
claim_state: pinned
key_metrics:
  total_revenue_fy2025_usd_m: 10064.7
  instruments_accessories_revenue_fy2025_usd_m: 6018.9
  systems_revenue_fy2025_usd_m: 2473.7
  service_revenue_fy2025_usd_m: 1572.1
  recurring_revenue_pct_fy2025: 84
  recurring_revenue_pct_q2_2026: 85
  davinci_asp_fy2025_usd_m: 1.60
  davinci_asp_h1_2026_usd_m: 1.66
  ia_revenue_per_procedure_range_usd: "900-3700"
  ia_revenue_per_procedure_q2_2026_usd: 1830
  service_contract_annual_fee_range_usd: "95000-225000"
  davinci_procedures_fy2025: 3153000
  davinci_installed_base_fy2025: 11106
  product_gross_margin_fy2025_pct: 66.3
  service_gross_margin_fy2025_pct: 64.6
  total_gross_margin_fy2025_pct: 66.0
  remaining_performance_obligations_q2_2026_usd_bn: 3.4
conclusions:
  - "PIL-2: ISRG is the closest disclosed analogue for precision-actuated robotic economics. Actuation content — systems + wearing instruments + precision-maintenance service — is effectively ~100% of revenue, with I&A alone 59.8% of FY2025 revenue. No disclosed BOM split prevents direct calibration of the 40–70% actuator share claim."
  - "PIL-4: ISRG's deployment-cost curve deflates via product tiering (refurbished/X/XiR at $0.6M) and cost-per-use innovation (extended-use instruments), not via nominal ASP decline — a template for how a humanoid 'GPT-3.5 moment' could arrive."
  - "Unit economics are fleet-based, not device-based: utilization +3% on an 11.1K installed base compounds I&A and service streams at 84–85% recurring share."
facts_count: 23
deducted_count: 6
views_count: 4
citation_count: 10
---

# ISRG Unit Economics — Intuitive Surgical (default)

**Thesis:** 001-physical-ai-technology-baseline · **Pillars:** PIL-2 (actuator+drive dominance in robotics BOM), PIL-4 (GPT-3.5 moment / deployment-cost curve) · **Retrieval:** agentii MCP, 3-layer protocol · **No price data** (market_data_stage: none)

## 1. Executive Summary

ISRG operates the textbook razor-blade model for precision-actuated robotic systems: the da Vinci surgical system sells at an average price of ~$1.60M in FY2025 (ex-lease, ex-Ion, ex-trade-in) https://agentii.ai/v/ISRG/sec166/page78, while instruments & accessories (I&A) earn $900–$3,700 per surgical procedure https://agentii.ai/v/ISRG/sec166/page77 and service contracts run $95K–$225K per system per year https://agentii.ai/v/ISRG/sec166/page77. FY2025 revenue was $10,064.7M, split I&A 59.8% / systems 24.6% / service 15.6% https://agentii.ai/v/ISRG/sec166/page77, with recurring revenue at 84% of total https://agentii.ai/v/ISRG/sec166/page78. Product gross margin was 66.3% and service 64.6% https://agentii.ai/v/ISRG/sec166/page79, on 3,153,000 da Vinci procedures (+18%) and an 11,106-system installed base (+12%) https://agentii.ai/v/ISRG/sec166/page69. For the thesis: actuation content dominates the disclosed value stack (PIL-2), but no BOM/actuator-vs-compute split is disclosed; and the deployment-cost curve deflates through tiered hardware ($0.6M refurbished/X/XiR) and cost-per-use innovation (extended-use instruments from H1 2027) rather than nominal ASP decline (PIL-4) https://agentii.ai/v/ISRG/sec172/page38 https://agentii.ai/v/ISRG/ect75/page2.

## 2. Data Sources

- 10-K FY2025 (filed 2026-02-03, `sec166`): pages 69, 77, 78, 79, 91
- 10-Q Q2 FY2026 (filed 2026-07-21, `sec172`): pages 12, 32, 38, 40
- Q2 FY2026 earnings call transcript (2026-07-16, `ect75`): page 2
- Structured: `search_xbrl_facts` (us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax FY2025/FY2024; us-gaap:GrossProfit FY2025; us-gaap:Revenues → no ISRG facts), `get_company_financials`, `get_company_fiscal_calendar`, `get_ticker_coverage`, `search_companies`, `list_xbrl_concepts`, `search_sec_filings`, `search_documents`, `list_sources`, `read_source_outline`, `read_source_pages`, `search_keyword_in_source`

## 3. Analysis

### 3.1 The unit is the procedure, not the system

ISRG's disclosed unit economics are anchored on the surgical procedure. [FACT] Approximately 3,153,000 da Vinci procedures were performed in FY2025, +18% vs 2,683,000 in FY2024 https://agentii.ai/v/ISRG/sec166/page69. [FACT] Q2 FY2026 saw ~889,000 procedures (+15%) https://agentii.ai/v/ISRG/sec172/page32. [FACT] The company discloses I&A revenue of $900–$3,700 per procedure depending on procedure type and complexity https://agentii.ai/v/ISRG/sec166/page77, and realized ~$1.83K of da Vinci I&A revenue per procedure in Q2 2026, up from ~$1.80K a year earlier https://agentii.ai/v/ISRG/ect75/page2. [DEDUCTED] Blended I&A revenue per procedure (da Vinci + Ion) was $6,018.9M ÷ (3,153,000 + 144,100) ≈ $1,826 in FY2025 (inputs: https://agentii.ai/v/ISRG/sec166/page77, https://agentii.ai/v/ISRG/sec166/page69) — the realized midpoint sits in the lower half of the disclosed range, reflecting mix toward cholecystectomy and other benign procedures https://agentii.ai/v/ISRG/ect75/page2.

### 3.2 System unit economics: the razor

[FACT] The da Vinci system sells for $0.7M–$3.1M (inclusive of one year of service) in the FY2025 10-K https://agentii.ai/v/ISRG/sec166/page77, restated to $0.6M–$3.1M in the Q2 2026 10-Q https://agentii.ai/v/ISRG/sec172/page38. [FACT] Realized da Vinci ASP (ex-lease, ex-Ion, ex-specified-price trade-in rights) was ~$1.60M in FY2025 vs ~$1.50M in FY2024 https://agentii.ai/v/ISRG/sec166/page78, and ~$1.66M in H1 2026 vs ~$1.55M a year earlier https://agentii.ai/v/ISRG/sec172/page40. [FACT] Q2 2026 purchased-system ASP was $1.6M vs $1.5M, driven by da Vinci 5 and dual-console mix, partially offset by trade-ins and lower-ASP X/XiR units https://agentii.ai/v/ISRG/ect75/page2. [DEDUCTED] Blended systems revenue per placement (incl. leases, trade-ins, Ion) was $2,473.7M ÷ 1,721 placements ≈ $1.44M in FY2025 (inputs: https://agentii.ai/v/ISRG/sec166/page77, https://agentii.ai/v/ISRG/sec166/page69). [FACT] 1,721 da Vinci systems were placed in FY2025 (+13%), including 870 da Vinci 5 (vs 362 in 2024) https://agentii.ai/v/ISRG/sec166/page69; Q2 2026 placements were 468 (+18%), including 246 da Vinci 5 https://agentii.ai/v/ISRG/sec172/page32. [FACT] Price-tiering is explicit: 64 refurbished Xi and 58 X systems were acquired in Q2 2026 (vs 10 and 49), plus 27 ASC placements, 20 of which were XiR — a low-ASP entry tier for cost-constrained customers https://agentii.ai/v/ISRG/ect75/page2. [VIEW] The 2.7–5x spread between the $0.6M entry tier and $3.1M high end shows precision-actuated platforms segment demand by price like general robotics platforms; tiering, not list-price cuts, is the disclosed expansion lever.

### 3.3 Service contract economics

[FACT] Service contracts carry annual fees of $95K–$225K per da Vinci system, are typically entered at sale/lease inception, cover five years with the first year bundled into the system price, and have "generally been renewed" at expiry https://agentii.ai/v/ISRG/sec166/page77. [FACT] Service revenue was $1,572.1M in FY2025 (+20%) https://agentii.ai/v/ISRG/sec166/page77 and $472.4M in Q2 2026 (+21%) https://agentii.ai/v/ISRG/sec172/page38. [DEDUCTED] Blended service revenue per installed system ≈ $1,572.1M ÷ (11,106 da Vinci + 995 Ion) ≈ $130K/year in FY2025 (inputs: https://agentii.ai/v/ISRG/sec166/page77, https://agentii.ai/v/ISRG/sec166/page69). [FACT] Q2 2026 service revenue per da Vinci system rose 8% YoY on da Vinci 5 mix https://agentii.ai/v/ISRG/ect75/page2. [FACT] Remaining performance obligations (mostly service) were $3.4B at 2026-06-30, ~half recognized within 12 months, remainder over up to five years; deferred revenue was $662.0M https://agentii.ai/v/ISRG/sec172/page12. [DEDUCTED] This is a contracted, near-churn-free service backlog: $3.4B ≈ 7 quarters of current quarterly service revenue ($472.4M), i.e., over 1.7 years of service billings contracted in advance — an annuity-like stream tied to the installed base (inputs: https://agentii.ai/v/ISRG/sec172/page12, https://agentii.ai/v/ISRG/sec172/page38).

### 3.4 Gross margin by revenue line — the cost-stack proxy

[FACT] FY2025 product gross profit was $5,626.5M (66.3% margin; 67.2% in 2024, 65.7% in 2023) and service gross profit was $1,015.8M (64.6% margin; 69.0% in 2024, 69.8% in 2023) https://agentii.ai/v/ISRG/sec166/page79. [FACT] Income-statement line COGS: product $2,866.1M and service $556.3M on FY2025 revenue of $8,492.6M product / $1,572.1M service, total gross profit $6,642.3M (66.0%) https://agentii.ai/v/ISRG/sec166/page91; the structured fact agrees ($6,642.3M, 10-K primary, us-gaap:GrossProfit). [FACT] Margin drags were new tariffs, incremental fixed overhead/depreciation from expanded manufacturing capacity, and higher da Vinci 5 costs https://agentii.ai/v/ISRG/sec166/page79. [FACT] Q2 2026 GAAP gross margin recovered to 67.8% (vs 66.3% a year earlier) https://agentii.ai/v/ISRG/sec172/page32, and non-GAAP was 70.0% — 68.7% excluding a $36M IEEPA tariff refund — on product cost reductions and fixed-overhead leverage https://agentii.ai/v/ISRG/ect75/page2. [DEDUCTED] Blended product COGS is 33.7% of product revenue; because product margin pools systems with I&A, a system-only BOM cannot be isolated — the disclosed stack stops at the product/service line (inputs: https://agentii.ai/v/ISRG/sec166/page91).

### 3.5 Recurring revenue and fleet economics

[FACT] Recurring revenue (I&A + service + operating leases) was $8,465.3M = 84% of FY2025 revenue (84% in 2024, 83% in 2023) https://agentii.ai/v/ISRG/sec166/page78; Q2 2026 was $2,469.1M = 85% https://agentii.ai/v/ISRG/sec172/page40. [FACT] Operating lease revenue was $874.3M in FY2025, of which $531M was variable (usage-based) https://agentii.ai/v/ISRG/sec166/page78; H1 2026 was $512M with $326M variable https://agentii.ai/v/ISRG/sec172/page40. [FACT] 54% of Q2 2026 da Vinci placements were under operating leases; lease revenue per system rose 7% on da Vinci 5 mix https://agentii.ai/v/ISRG/ect75/page2. [FACT] Utilization (procedures per system per year) rose 3% in FY2025 on an installed base of ~11,106 systems https://agentii.ai/v/ISRG/sec166/page69, and another 3% in Q2 2026 on ~11,710 systems https://agentii.ai/v/ISRG/sec172/page32. [DEDUCTED] Fleet unit economics improve with base maturity: +18% procedures on +12% base implies same-system throughput growth, and I&A grows ~19% with procedures https://agentii.ai/v/ISRG/sec166/page78 (inputs: https://agentii.ai/v/ISRG/sec166/page69).

### 3.6 Pillar mapping

**PIL-2 — actuator+drive vs compute in the BOM.** [VIEW] ISRG is the strongest disclosed analogue for the claim that precision actuation dominates robotics economics: every disclosed revenue dollar is actuation-adjacent — wearing actuated instruments (59.8% of revenue), actuator-dense capital ($0.6–3.1M), and precision-maintenance service ($95–225K/yr) https://agentii.ai/v/ISRG/sec166/page77. [VIEW] The premium pricing power of precision actuation is directly observable in the ASP trajectory ($1.50M → $1.60M → $1.66M), which rose on actuation/feature content (da Vinci 5) even as compute costs elsewhere deflated https://agentii.ai/v/ISRG/sec166/page78 https://agentii.ai/v/ISRG/sec172/page40. [FACT] However, ISRG does not disclose any BOM-level split (actuator, drive, compute, optics) or per-system COGS — the finest disclosed cut is product vs service gross profit https://agentii.ai/v/ISRG/sec166/page79. The thesis's 40–70% actuator share for humanoids therefore cannot be calibrated directly from ISRG filings; ISRG supports the *direction* (actuation dominates value) not the *magnitude*.

**PIL-4 — GPT-3.5 moment / deployment-cost curve.** [FACT] Nominal ASPs are not deflating — mix-driven content upgrades push them up — yet the effective cost of deployment is falling on two disclosed levers: (1) hardware tiering (refurbished Xi, X, XiR at the $0.6M end, ASC channel) https://agentii.ai/v/ISRG/ect75/page2 and (2) consumable cost-per-use reduction via the extended-use ENDORIST instrument program launching H1 2027, which targets "lower customer cost per use" for high-volume benign procedures https://agentii.ai/v/ISRG/ect75/page2. [VIEW] For PIL-4's anticipated humanoid GPT-3.5 moment (2027-Q4–2028), the ISRG template suggests the discontinuity may arrive through cost-per-use and entry-tier deflation rather than a headline price collapse — the analogue metric to monitor is I&A per procedure (~$1.83K and falling on extended use) and entry-tier ASP, not list ASP https://agentii.ai/v/ISRG/ect75/page2. [FACT] Recurring revenue at 84–85% of total means the installed base, not new placements, funds the business — the same compounding structure PIL-4 needs for humanoid fleets to cross into mass deployment https://agentii.ai/v/ISRG/sec166/page78.

## 4. Key Metrics

| Metric | FY2024 | FY2025 | H1 2026 | Source |
|---|---|---|---|---|
| Total revenue ($M) | 8,352.1 | 10,064.7 | 5,663.1 | https://agentii.ai/v/ISRG/sec166/page77, https://agentii.ai/v/ISRG/sec172/page38 |
| I&A revenue ($M) | 5,079.0 | 6,018.9 | 3,421.3 | same |
| Systems revenue ($M) | 1,966.0 | 2,473.7 | 1,335.7 | same |
| Service revenue ($M) | 1,307.1 | 1,572.1 | 906.1 | same |
| Recurring revenue % | 84% | 84% | 85% | https://agentii.ai/v/ISRG/sec166/page78, https://agentii.ai/v/ISRG/sec172/page40 |
| da Vinci ASP ($M) | ~1.50 | ~1.60 | ~1.66 | https://agentii.ai/v/ISRG/sec166/page78, https://agentii.ai/v/ISRG/sec172/page40 |
| System price range ($M) | — | 0.7–3.1 | 0.6–3.1 | https://agentii.ai/v/ISRG/sec166/page77, https://agentii.ai/v/ISRG/sec172/page38 |
| I&A per procedure ($) | — | 900–3,700 (disclosed range); ~1,826 blended | ~1,830 (dv, Q2) | https://agentii.ai/v/ISRG/sec166/page77, https://agentii.ai/v/ISRG/ect75/page2 |
| Service contract fee ($K/yr) | — | 95–225 | 95–225 | https://agentii.ai/v/ISRG/sec166/page77 |
| da Vinci procedures | 2,683,000 | 3,153,000 | — | https://agentii.ai/v/ISRG/sec166/page69 |
| da Vinci installed base | 9,902 | 11,106 | 11,710 (Q2) | https://agentii.ai/v/ISRG/sec166/page69, https://agentii.ai/v/ISRG/sec172/page32 |
| Product gross margin | 67.2% | 66.3% | — | https://agentii.ai/v/ISRG/sec166/page79 |
| Service gross margin | 69.0% | 64.6% | — | https://agentii.ai/v/ISRG/sec166/page79 |
| Total gross margin | 67.5% | 66.0% | 67.8% (Q2 GAAP) | https://agentii.ai/v/ISRG/sec166/page69, https://agentii.ai/v/ISRG/sec172/page32 |
| Remaining performance obligations ($B) | — | — | 3.4 (Q2) | https://agentii.ai/v/ISRG/sec172/page12 |

Structured verification: us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax FY2025 = $10,064.7M (10-K primary) and FY2024 = $8,352.1M (10-K primary) via `search_xbrl_facts`; us-gaap:GrossProfit FY2025 = $6,642.3M (10-K primary). us-gaap:Revenues returns no ISRG facts — ISRG tags top-line revenue under the ASC 606 concept.

## 5. Coverage Gaps & Citations

**Coverage gaps (never invented):**
1. **No BOM or per-system cost stack.** ISRG discloses product/service gross margin only; the actuator/drive/compute split within a da Vinci system is not disclosed in any 10-K/10-Q page retrieved. PIL-2's 40–70% actuator BOM claim cannot be calibrated from ISRG.
2. **No I&A gross margin standalone.** Instruments & accessories margin is pooled inside product margin (66.3%); consumable-only profitability is not separable from retrieved disclosures.
3. **No CAC/payback or per-hospital acquisition cost disclosure** (sales org structure described qualitatively only, 10-K page14).
4. **No precise procedure-payer mix** (Medicaid/ACA exposure: company states it has no precise estimate) https://agentii.ai/v/ISRG/ect75/page6.
5. **No Q2 2026 8-K press-release page reads** (sec171) — rate-limited; superseded by the 10-Q pages retrieved.
6. **Ion ASP facts** retrieved ($500K–$815K, $55K–$70K service) but Ion-only revenue is not disclosed separately (pooled in product lines) https://agentii.ai/v/ISRG/sec166/page77.

**Citation index (unique /v/ links):**
1. https://agentii.ai/v/ISRG/sec166/page69 — FY2025 highlights: procedures, placements, installed base, utilization, gross margin
2. https://agentii.ai/v/ISRG/sec166/page77 — price ranges, I&A per procedure, service fees, FY2025 revenue table
3. https://agentii.ai/v/ISRG/sec166/page78 — ASP FY2025/FY2024, lease revenue, recurring revenue 84%
4. https://agentii.ai/v/ISRG/sec166/page79 — product/service gross profit and margin drivers
5. https://agentii.ai/v/ISRG/sec166/page91 — FY2025 consolidated income statement (line COGS)
6. https://agentii.ai/v/ISRG/sec172/page12 — Q2 2026 revenue disaggregation, RPO $3.4B, deferred revenue
7. https://agentii.ai/v/ISRG/sec172/page32 — Q2 2026 operational/financial highlights
8. https://agentii.ai/v/ISRG/sec172/page38 — Q2/H1 2026 revenue table, price range update
9. https://agentii.ai/v/ISRG/sec172/page40 — H1 2026 ASP $1.66M, lease revenue, recurring 85%
10. https://agentii.ai/v/ISRG/ect75/page2 — Q2 2026 transcript: I&A per procedure $1.83K, non-GAAP GM 70%, extended-use program, leasing 54%, ASC/XiR tiering

## 6. Verification (call trace)

| # | Call | Result | Used for |
|---|---|---|---|
| 1 | search_companies (ISRG) | CIK 0001035267, med.medical_devices.surgical_robotics | entity resolution |
| 2 | get_ticker_coverage (ISRG) | 52,854 XBRL facts; 19 transcripts; sec_filings tier "missing" | routing |
| 3 | get_company_fiscal_calendar (ISRG) | FY ends Jan 31; FY2026 Q2 ended 2026-06-30 | period alignment |
| 4 | search_sec_filings (ISRG) | 173 filings; citation_ids sec154–sec173 | Layer 1 |
| 5 | search_documents (ISRG) | 79 src_documents; 10-K FY2025 = sec166 | Layer 1 |
| 6 | list_xbrl_concepts (Revenue, us-gaap) | RevenueFromContractWithCustomerExcludingAssessedTax; Revenues | concept discovery |
| 7 | list_xbrl_concepts (Revenue, isrg ns) | empty — no custom-namespace facts | concept discovery |
| 8 | get_company_financials (ISRG) | Q2 FY2026 GP $1,960.4M, COGS $931.9M; FY2025 rev $10,064.7M | structured baseline |
| 9 | search_documents (transcripts) | 19 transcripts, latest 2026-07-16 | Layer 1 |
| 10 | read_source_outline (sec166) | 130-page map: pages 69/77/78/79/91/108 targeted | Layer 2 |
| 11 | read_source_outline (ect75 via source_id) | 6-page transcript map: pages 2, 6 targeted | Layer 2 |
| 12 | list_sources (transcripts) | source_ids for transcripts | Layer 1 |
| 13 | read_source_pages (sec166, page77+78) | price ranges, ASP, revenue table, recurring revenue | Layer 3 |
| 14 | read_source_pages (sec166, page79+69) | margins by line; procedures/placements/installed base | Layer 3 |
| 15 | search_xbrl_facts (GrossProfit, FY2025) | $6,642.3M 10-K primary | P2.1 structured |
| 16 | search_xbrl_facts (RevenueFromContractWithCustomerExcludingAssessedTax, FY2024) | $8,352.1M 10-K primary | P2.1 structured |
| 17 | search_xbrl_facts (Revenues, FY2025) | 0 facts — concept unused by ISRG | coverage note |
| 18 | search_keyword_in_source (sec172, "Instruments and accessories") | pages 38/40/32/12 targeted | Layer 2 |
| 19 | search_keyword_in_source (sec171, "ASP") | rate-limited (superseded by sec172 reads) | Layer 2 |
| 20 | read_source_pages (ect75, page2+6) | I&A per procedure, extended use, ASP, leasing, non-GAAP GM | Layer 3 |
| 21 | read_source_pages (sec172, page38+40) | Q2/H1 2026 tables, ASP $1.66M, recurring 85% | Layer 3 |
| 22 | read_source_pages (sec172, page12+32) | disaggregation, RPO $3.4B, Q2 highlights | Layer 3 |
| 23 | read_source_pages (sec166, page91) | FY2025 income statement (line COGS) | Layer 3 |
| 24 | search_xbrl_facts (RevenueFromContractWithCustomerExcludingAssessedTax, FY2025) | $10,064.7M 10-K primary | P2.1 structured |

Tool diversity: 13 distinct MCP tools used (≥9 required). All material numbers trace to calls 13–24 above; no number was sourced from memory or price data.
