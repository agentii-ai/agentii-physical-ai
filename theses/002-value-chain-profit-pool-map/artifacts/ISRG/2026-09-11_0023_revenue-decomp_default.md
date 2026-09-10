---
artifact_id: "002-ISRG-revenue-decomp-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: ISRG
skill: revenue-decomp
mode: default
affix: revenue-mix
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "037b396ab004"
as_of: 2026-09-11
entity_claims:
  - entity: ISRG
    metric: instruments_accessories_revenue_usd
    value: 6018900000
    unit: USD
    period: FY2025
    source: "10-K:page77"
    retrieved_at: 2026-09-11
    note: "proposed map addition — dispatcher to confirm"
  - entity: ISRG
    metric: systems_revenue_usd
    value: 2473700000
    unit: USD
    period: FY2025
    source: "10-K:page77"
    retrieved_at: 2026-09-11
    note: "proposed map addition — dispatcher to confirm"
  - entity: ISRG
    metric: service_revenue_usd
    value: 1572100000
    unit: USD
    period: FY2025
    source: "10-K:page77"
    retrieved_at: 2026-09-11
    note: "proposed map addition — dispatcher to confirm"
  - entity: ISRG
    metric: recurring_revenue_share_pct
    value: 84
    unit: pct
    period: FY2025
    source: "10-K:page78"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: recurring_revenue_share_pct
    value: 85
    unit: pct
    period: Q2-2026
    source: "10-Q:page40"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: installed_base_units
    value: 12101
    unit: units
    period: FY2025
    source: "10-K:page69"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: installed_base_units
    value: 12806
    unit: units
    period: Q2-2026
    source: "10-Q:page32"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: product_gross_margin_pct
    value: 66.3
    unit: pct
    period: FY2025
    source: "10-K:page79"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: revenue_per_procedure_usd
    value: 1852
    unit: USD
    period: Q2-2026
    source: "10-Q:page32;10-Q:page38"
    retrieved_at: 2026-09-11
    note: "[DEDUCTED] I&A revenue 1,734.9M / (da Vinci 889,000 + Ion 47,900) procedures"
  - entity: ISRG
    metric: model_layer_revenue_per_deployed_unit_usd
    value: 0
    unit: USD
    period: FY2025
    source: "10-K:page77"
    retrieved_at: 2026-09-11
    note: "[DEDUCTED] digital-solutions/software revenue immaterial per 10-K; falsifier threshold is 5,000"
citations:
  - citation_id: sec166
    page: page69
    label: "FY2025 10-K operational highlights (filed 2026-02-03): installed base, procedures, gross margin"
  - citation_id: sec166
    page: page77
    label: "FY2025 10-K revenue decomposition table FY2023-FY2025, pricing ranges, digital solutions immateriality"
  - citation_id: sec166
    page: page78
    label: "FY2025 10-K recurring revenue table, operating lease revenue, lease buyouts, da Vinci ASP"
  - citation_id: sec166
    page: page79
    label: "FY2025 10-K product and service gross profit margins"
  - citation_id: sec166
    page: page10
    label: "FY2025 10-K learning technology portfolio (Case Insights, SimNow, Intuitive Learning)"
  - citation_id: sec166
    page: page11
    label: "FY2025 10-K digital solutions (My Intuitive, My Intuitive+, 3D Models), service incl. software upgrades"
  - citation_id: sec172
    page: page32
    label: "Q2 2026 10-Q operational highlights (filed 2026-07-21): installed base 11,710/1,096, procedures, gross margin 67.8%"
  - citation_id: sec172
    page: page38
    label: "Q2 2026 10-Q revenue decomposition table Q2/H1 2026, pricing ranges, digital solutions immateriality"
  - citation_id: sec172
    page: page40
    label: "Q2 2026 10-Q recurring revenue table (85%), operating lease revenue, ASP"
  - citation_id: sec172
    page: page37
    label: "Q2 2026 10-Q installed base under operating leases (da Vinci 3,425; Ion 397)"
pillars_addressed: [PIL-3]
claim_state: pinned
key_metrics:
  fy2025_revenue_total_usd: 10064700000
  fy2025_ia_revenue_usd: 6018900000
  fy2025_systems_revenue_usd: 2473700000
  fy2025_service_revenue_usd: 1572100000
  fy2025_ia_share_pct: 59.8
  fy2025_systems_share_pct: 24.6
  fy2025_service_share_pct: 15.6
  fy2025_recurring_revenue_usd: 8465300000
  fy2025_recurring_share_pct: 84
  fy2025_operating_lease_revenue_usd: 874300000
  fy2025_installed_base_units: 12101
  fy2025_recurring_per_installed_unit_usd: 699553
  fy2025_ia_per_installed_unit_usd: 497389
  fy2025_service_per_installed_unit_usd: 129915
  fy2025_service_contract_annual_fee_range_usd: [95000, 225000]
  fy2025_ia_per_procedure_range_usd: [900, 3700]
  fy2025_product_gross_margin_pct: 66.3
  fy2025_service_gross_margin_pct: 64.6
  q2_2026_revenue_total_usd: 2892300000
  q2_2026_ia_revenue_usd: 1734900000
  q2_2026_systems_revenue_usd: 685000000
  q2_2026_service_revenue_usd: 472400000
  q2_2026_recurring_revenue_usd: 2469100000
  q2_2026_recurring_share_pct: 85
  q2_2026_installed_base_units: 12806
  q2_2026_ia_per_procedure_usd: 1852
  software_subscription_revenue: immaterial
  model_layer_revenue_per_deployed_unit_usd: 0
conclusions:
  - "FY2025 revenue decomposition reconciles exactly to the T-001 baseline: I&A 59.8% / systems 24.6% / service 15.6%; recurring 84% (rising to 85% in Q2/H1 2026)."
  - "The software/subscription layer (My Intuitive+, Case Insights/Advanced Insights Suite, My Intuitive, SimNow, 3D Models) generates immaterial revenue; software monetizes as features bundled into hardware sales and service contracts, not as a standalone model layer."
  - "PIL-3 NOT falsified: model-layer revenue per deployed unit is approximately zero vs the >$5,000 falsification threshold; per-unit recurring revenue (~$700K) is dominated by disposables and maintenance, not software."
  - "Residual: falsification would require only ~$60.5M/yr of undisclosed software revenue, and amounts up to ~1% of revenue (~$100.6M) could hide under immateriality — a narrow unresolved zone."
facts_count: 42
deducted_count: 14
views_count: 4
citation_count: 10
---

# ISRG Revenue Decomposition — PIL-3 Model-Layer Test Input

## Executive Summary

Intuitive Surgical's FY2025 revenue decomposition is retrieved fresh from the FY2025 10-K (sec166, filed 2026-02-03) and the Q2 2026 10-Q (sec172, filed 2026-07-21) and reconciles **exactly** to the T-001 baseline: instruments & accessories $6,018.9M (59.8%), systems $2,473.7M (24.6%), service $1,572.1M (15.6%), total $10,064.7M [FACT](https://agentii.ai/v/ISRG/sec166/page77). Recurring revenue (I&A + service + operating leases) is $8,465.3M = 84% of revenue [FACT](https://agentii.ai/v/ISRG/sec166/page78), rising to 85% in Q2/H1 2026 [FACT](https://agentii.ai/v/ISRG/sec172/page40). Installed base: 11,106 da Vinci + 995 Ion = 12,101 at FY2025 [FACT](https://agentii.ai/v/ISRG/sec166/page69); 12,806 at Q2 2026 [FACT](https://agentii.ai/v/ISRG/sec172/page32). Recurring revenue per deployed unit is ~$700K/yr — dominated by disposables (~$497K) and maintenance (~$130K). The software/subscription layer (My Intuitive+, Case Insights, My Intuitive, SimNow, 3D Models) generates **immaterial** revenue: "We do not currently generate material revenue from these offerings" [FACT](https://agentii.ai/v/ISRG/sec166/page77). Model-layer revenue per deployed unit ≈ $0 vs the $5,000 falsification threshold — **PIL-3 not falsified**.

## Data Sources

| Source | Citation | Retrieval |
|---|---|---|
| FY2025 10-K (2025-12-31), accession 0001035267-26-000010 | sec166 | read_source_pages: page69, page77, page78, page79, page10, page11 |
| Q2 2026 10-Q (2026-06-30), accession 0001035267-26-000058 | sec172 | read_source_pages: page32, page37, page38, page40 |
| XBRL us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax | XBRL facts | search_xbrl_facts, multi-period FY2021–H1 2026 (is_primary=true) |
| Keyword checks (Intuitive Hub, subscription) | sec166 | search_keyword_in_source |

XBRL cross-check [FACT]: the primary revenue fact for the year ended 2025-12-31 is $10,064.7M (source_authority 3, 10-K), matching the page77 table total; H1 2026 fact $5,663.1M and Q2 2026 fact $2,892.3M match the page38 table totals. Filing dates confirm ISRG is a calendar-year filer (periods 2025-01-01 → 2025-12-31), notwithstanding the MCP company-registry field `fiscal_year_end_month: 1`.

## Analysis

### 1. Revenue decomposition (FY2023–FY2025)

Revenue by category for FY2025 is: I&A $6,018.9M, systems $2,473.7M, product $8,492.6M, service $1,572.1M, total $10,064.7M; U.S. $6,815.8M (68%) and OUS $3,248.9M (32%) [FACT](https://agentii.ai/v/ISRG/sec166/page77). FY2024 was I&A $5,079.0M / systems $1,966.0M / service $1,307.1M / total $8,352.1M; FY2023 was $4,276.6M / $1,679.7M / $1,167.8M / $7,124.1M [FACT](https://agentii.ai/v/ISRG/sec166/page77). Derived shares: I&A 59.8% / 24.6% / 15.6% in FY2025; 60.8% / 23.5% / 15.6% in FY2024; 60.0% / 23.6% / 16.4% in FY2023 [DEDUCTED] from the page77 table. The mix has been remarkably stable: hardware (systems) is a stable ~24%, consumables (I&A) ~60%, service ~16% [VIEW].

| Category ($M) | FY2025 | FY2024 | FY2023 |
|---|---|---|---|
| Instruments & accessories | 6,018.9 | 5,079.0 | 4,276.6 |
| Systems | 2,473.7 | 1,966.0 | 1,679.7 |
| Total product | 8,492.6 | 7,045.0 | 5,956.3 |
| Service | 1,572.1 | 1,307.1 | 1,167.8 |
| Total revenue | 10,064.7 | 8,352.1 | 7,124.1 |

Q2 2026: I&A $1,734.9M, systems $685.0M, product $2,419.9M, service $472.4M, total $2,892.3M; H1 2026: $3,421.3M / $1,335.7M / $4,757.0M / $906.1M / $5,663.1M [FACT](https://agentii.ai/v/ISRG/sec172/page38). Q2 2026 shares: 60.0% / 23.7% / 16.3% [DEDUCTED] from the page38 table.

### 2. Recurring revenue and the per-unit math

Recurring revenue = I&A + service + operating lease revenue [FACT](https://agentii.ai/v/ISRG/sec166/page78). FY2025: $6,018.9M + $1,572.1M + $874.3M = **$8,465.3M = 84%** of total revenue; FY2024 84%, FY2023 83% [FACT](https://agentii.ai/v/ISRG/sec166/page78). Operating lease revenue was $874M FY2025 (of which $531M variable, usage-based) with lease buyouts of $130M; da Vinci ASP (ex-operating-lease, ex-Ion, ex-trade-ins) was ~$1.60M FY2025 vs ~$1.50M FY2024 [FACT](https://agentii.ai/v/ISRG/sec166/page78).

Q2 2026 recurring: I&A $1,734.9M + service $472.4M + operating lease $261.8M = **$2,469.1M = 85%**; H1 2026 $4,839.4M = 85% [FACT](https://agentii.ai/v/ISRG/sec172/page40). H1 2026 operating lease revenue $512.0M ($326M variable), buyouts $108M, ASP ~$1.66M [FACT](https://agentii.ai/v/ISRG/sec172/page40).

Installed base: ~11,106 da Vinci (vs ~9,902) and ~995 Ion (vs ~805) at 2025-12-31 [FACT](https://agentii.ai/v/ISRG/sec166/page69); ~11,710 da Vinci and ~1,096 Ion at 2026-06-30 [FACT](https://agentii.ai/v/ISRG/sec172/page32). Combined: 12,101 (FY2025) and 12,806 (Q2 2026) [DEDUCTED] — the 12,101 reconciles exactly to T-001's "12,101 installed".

Per-deployed-unit recurring revenue [DEDUCTED] from pages 69/78:

| Per unit (FY2025, $K/yr) | Value |
|---|---|
| Total recurring ÷ 12,101 | ~699.6 |
| I&A ÷ 12,101 | ~497.4 |
| Service ÷ 12,101 | ~129.9 |
| Operating lease ÷ 12,101 | ~72.3 |

Q2 2026 cross-check [DEDUCTED]: H1 2026 recurring annualized ($4,839.4M × 2) ÷ 12,806 = ~$755.8K/unit/yr, consistent with growing utilization (+3% procedures/system [FACT](https://agentii.ai/v/ISRG/sec172/page32)).

Unit-economics anchors [FACT](https://agentii.ai/v/ISRG/sec166/page77): da Vinci systems sell for $0.7M–$3.1M; I&A revenue is $900–$3,700 per procedure; da Vinci service contracts $95K–$225K/yr; Ion systems $500K–$815K with $55K–$70K/yr service. Q2 2026 computed I&A per procedure: $1,734.9M ÷ (889,000 da Vinci + 47,900 Ion) = ~$1,852 [DEDUCTED] from page32/page38 procedure and revenue facts — consistent with the entities-map ~$1.83K anchor.

### 3. The software/subscription slice (model layer)

The digital portfolio is: My Intuitive (free app), **My Intuitive+ ("a digital subscription package available with the da Vinci 5 platform")**, 3D Models, and the Advanced Insights Suite (Case Insights, Insights Engine), SimNow, Intuitive Learning [FACT](https://agentii.ai/v/ISRG/sec166/page10) [FACT](https://agentii.ai/v/ISRG/sec166/page11). "Intuitive Hub" is not separately named in the FY2025 10-K digital portfolio [FACT — keyword search, sec166]. Software upgrades and updates are delivered **inside service plans** ("Maintenance support... includes service care plans, support teams, OnSite monitoring, software upgrades and updates") [FACT](https://agentii.ai/v/ISRG/sec166/page11).

Decisive disclosure, stated twice (FY2025 10-K and Q2 2026 10-Q): "as part of our ecosystem of products and services, we provide a portfolio of learning offerings and digital solutions. **We do not currently generate material revenue from these offerings**" [FACT](https://agentii.ai/v/ISRG/sec166/page77) [FACT](https://agentii.ai/v/ISRG/sec172/page38). No software/subscription line exists in the revenue table or XBRL decomposition.

**PIL-3 falsifier test** [DEDUCTED]: model_layer_revenue_per_deployed_unit_usd ≈ $0 vs the >$5,000 falsification threshold — not falsified, decisively. The model layer at ISRG monetizes as features bundled into hardware ASP and service contracts, not as a standalone subscription stream [VIEW]. Sensitivity [DEDUCTED]: the $5,000/unit threshold on 12,101 units corresponds to only ~$60.5M/yr of software revenue; "immaterial" could conceal up to ~1% of revenue (~$100.6M). The zone $60.5M–$100.6M is not directly observable from filings — a narrow, low-probability residual risk to the PIL-3 input [VIEW]. Attribution cross-check [DEDUCTED]: under the most hostile attribution (treating all service revenue — $472.4M in Q2 2026 — as software), per-unit software revenue would be ~$147.6K/yr, far above threshold; the falsifier therefore hinges entirely on the immateriality disclosure, which pins disclosed software at ≈$0/unit [FACT](https://agentii.ai/v/ISRG/sec166/page77).

### 4. Margin anchors

Product gross margin FY2025 66.3% (FY2024 67.2%, FY2023 65.7%); service gross margin FY2025 64.6% (FY2024 69.0%, FY2023 69.8%) [FACT](https://agentii.ai/v/ISRG/sec166/page79). Consolidated gross profit % FY2025 66.0% [FACT](https://agentii.ai/v/ISRG/sec166/page69); Q2 2026 67.8% [FACT](https://agentii.ai/v/ISRG/sec172/page32). Leased-unit exposure: 3,425 da Vinci and 397 Ion systems were under operating leases at 2026-06-30 (1,903 da Vinci usage-based) [FACT](https://agentii.ai/v/ISRG/sec172/page37).

## Key Metrics

| Metric | Value | Period | Tag | Citation |
|---|---|---|---|---|
| Total revenue | $10,064.7M | FY2025 | FACT | sec166/page77 |
| I&A / Systems / Service | $6,018.9M / $2,473.7M / $1,572.1M | FY2025 | FACT | sec166/page77 |
| Mix shares | 59.8% / 24.6% / 15.6% | FY2025 | DEDUCTED | sec166/page77 |
| Recurring revenue | $8,465.3M (84%) | FY2025 | FACT | sec166/page78 |
| Recurring share | 85% (Q2 $2,469.1M; H1 $4,839.4M) | Q2/H1 2026 | FACT | sec172/page40 |
| Installed base | 12,101 (dv 11,106 + Ion 995) | FY2025 | FACT/DEDUCTED | sec166/page69 |
| Installed base | 12,806 (dv 11,710 + Ion 1,096) | Q2 2026 | FACT/DEDUCTED | sec172/page32 |
| Recurring per deployed unit | ~$699.6K/yr | FY2025 | DEDUCTED | sec166/page69, page78 |
| I&A per procedure | ~$1,852 | Q2 2026 | DEDUCTED | sec172/page32, page38 |
| I&A per procedure (disclosed range) | $900–$3,700 | FY2025 | FACT | sec166/page77 |
| Service contract fee | $95K–$225K/yr (dv); $55K–$70K (Ion) | FY2025 | FACT | sec166/page77 |
| Product / Service gross margin | 66.3% / 64.6% | FY2025 | FACT | sec166/page79 |
| Software/subscription revenue | immaterial (≈$0 per unit) | FY2025 | FACT | sec166/page77 |

## Coverage Gaps & Citations

Gaps:
1. No standalone software/subscription revenue line exists in the revenue tables or XBRL — only the immateriality statement; the exact software $ cannot be retrieved (by design, it is below disclosure materiality).
2. "Intuitive Hub" is not named in the FY2025 10-K (it appeared in prior-year filings); the current named portfolio is My Intuitive / My Intuitive+ / Advanced Insights Suite (Case Insights) / SimNow / Intuitive Learning / 3D Models.
3. get_ticker_coverage reports `data_freshness_tier: "missing"` for several sources despite populated record counts (metadata quirk; earnings_calendar is "fresh" through 2026-10-20). sec_filings source shows 0 records, but filings were retrievable via search_sec_filings/search_documents.
4. MCP fiscal-calendar labels (`fiscal_year_end_month: 1`) mislabel ISRG quarters; retrieved fact period labels (2025-01-01 → 2025-12-31) confirm the calendar-year convention used by T-001.
5. No price data used (audit mandate).
6. Proposed map additions flagged in entity_claims (instruments_accessories_revenue_usd, systems_revenue_usd, service_revenue_usd) await dispatcher confirmation per entities.md §2 discipline.

Citations (all inline via https://agentii.ai/v/ISRG/{citation_id}/{page}):

| # | Citation | Page | Content |
|---|---|---|---|
| 1 | sec166 | page69 | FY2025 highlights: revenue, procedures, installed base, gross margin |
| 2 | sec166 | page77 | Revenue table FY2023–FY2025; pricing; digital-solutions immateriality |
| 3 | sec166 | page78 | Recurring revenue table; op-lease; buyouts; ASP |
| 4 | sec166 | page79 | Product/service gross margins |
| 5 | sec166 | page10 | Learning tech: Case Insights, SimNow, Intuitive Learning |
| 6 | sec166 | page11 | My Intuitive / My Intuitive+ / 3D Models; software upgrades in service |
| 7 | sec172 | page32 | Q2 2026 highlights: installed base 11,710/1,096, procedures, 67.8% GM |
| 8 | sec172 | page38 | Q2/H1 2026 revenue table; immateriality statement |
| 9 | sec172 | page40 | Q2/H1 2026 recurring table (85%); ASP $1.66M |
| 10 | sec172 | page37 | Installed base under operating leases |

## Verification (T-001 reconciliation + PIL-3)

| Item | T-001 baseline | Fresh retrieval | Δ | Verdict | Citation |
|---|---|---|---|---|---|
| I&A revenue FY2025 | $6,018.9M (59.8%) | $6,018.9M; 59.8% | 0 | Confirmed | sec166/page77 |
| Systems revenue FY2025 | $2,473.7M (24.6%) | $2,473.7M; 24.6% | 0 | Confirmed | sec166/page77 |
| Service revenue FY2025 | $1,572.1M (15.6%) | $1,572.1M; 15.6% | 0 | Confirmed | sec166/page77 |
| Total revenue FY2025 | (sum) $10,064.7M | $10,064.7M (XBRL fact matches) | 0 | Confirmed | sec166/page77 |
| Recurring share | 84% | 84% FY2025; **85%** Q2/H1 2026 | 0 (+1pp) | Confirmed | sec166/page78; sec172/page40 |
| Installed base | 12,101 | 12,101 (11,106 dv + 995 Ion) | 0 | Confirmed | sec166/page69 |
| PIL-3: model-layer revenue per deployed unit | threshold: >$5,000 falsifies | ≈$0 (software/subscription immaterial) | — | **Not falsified** | sec166/page77 |

Verification summary: all seven reconciliation items confirmed with zero delta; the T-001 numbers are exact retrievals from sec166 page77/page78/page69. The recurring share has since ticked up to 85% (Q2 2026). PIL-3's direct test input resolves decisively against the falsifier: ISRG's model layer is a bundled feature, not a revenue line.
