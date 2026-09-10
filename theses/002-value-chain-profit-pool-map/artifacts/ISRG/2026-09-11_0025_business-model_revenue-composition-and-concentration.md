---
artifact_id: "002-ISRG-business-model-revenue-composition-and-concentration-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: ISRG
skill: business-model
mode: revenue-composition-and-concentration
affix: ""
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "9479220eef91"
as_of: 2026-09-11
entity_claims:
  - entity: ISRG
    metric: product_gross_margin_pct
    value: 66.3
    unit: pct
    period: FY2025
    source: "10-K:page79"
    retrieved_at: 2026-09-11
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
    source: "10-Q:page32 + 10-Q:page35"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: revenue_per_procedure_usd
    value: 1826
    unit: USD
    period: FY2025
    source: "derived: 10-K:page69 + 10-K:page77"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: revenue_per_procedure_usd
    value: 1852
    unit: USD
    period: Q2-2026
    source: "derived: 10-Q:page32 + 10-Q:page38"
    retrieved_at: 2026-09-11
citations:
  - "sec166 (FY2025 10-K, filed 2026-02-03)"
  - "sec172 (Q2-2026 10-Q, filed 2026-07-21)"
  - "XBRL isrg-20251231.htm / isrg-20260630.htm"
pillars_addressed: [PIL-3]
claim_state: pinned
key_metrics:
  ia_share_of_revenue_pct_fy2025: 59.8
  us_share_of_revenue_pct_fy2025: 68
  recurring_revenue_usd_fy2025: 8465300000
  service_revenue_per_installed_unit_usd_fy2025: 129900
  recurring_revenue_per_installed_unit_usd_fy2025: 699600
  remaining_performance_obligations_usd: 3400000000
conclusions:
  - "Concentration: Instruments & Accessories = 59.8% of FY2025 revenue and U.S. = 68% — both >20% concentration flags; 84% of revenue is recurring, an unusually high attach-rate structure for a 'product' company."
  - "PIL-3 direct test input: disclosed software-subscription revenue (My Intuitive+) is not material (~$0/unit), BUT the per-unit subscription-bearing service contract ($95K-$225K/system/year; realized $129.9K/system FY2025) exceeds the $5,000/unit falsification threshold by ~26x — under the pillar's 'INCLUDES per-unit software/subscription revenue' definition, the subscription case falsifies PIL-3 unless model-layer revenue is restricted to standalone digital subscriptions."
facts_count: 13
deducted_count: 4
views_count: 3
citation_count: 31
---

# ISRG — Revenue Composition & Concentration (mode 1_3)

## Executive Summary

FY2025 revenue of $10,064.7M decomposes into Instruments & Accessories $6,018.9M (59.8%), Systems $2,473.7M (24.6%), and Service $1,572.1M (15.6%) [DEDUCTED] [https://agentii.ai/v/ISRG/sec166/page77]. Geography: U.S. $6,815.8M (68%), OUS $3,248.9M (32%) — both the product line (I&A) and region (U.S.) exceed the 20% concentration flag [https://agentii.ai/v/ISRG/sec166/page77]. Recurring revenue — I&A + service + operating-lease revenue — is $8,465.3M = 84% of total, rising to 85% in Q2-2026 [FACT] [https://agentii.ai/v/ISRG/sec166/page78], [https://agentii.ai/v/ISRG/sec172/page40]. **PIL-3 test input**: the standalone software/subscription slice (My Intuitive+) is disclosed as not material; however, the per-system subscription-bearing service contract realizes ~$129.9K per installed unit per year — ~26x the $5,000 falsification threshold — while total recurring per unit is ~$699.6K [DEDUCTED]. Under the pillar's own "includes per-unit software/subscription revenue" definition, the ISRG subscription case is a falsification signal for PIL-3.

## Mode 1_3 — Revenue Composition & Concentration

**By product line (FY2025)** [FACT, table] [https://agentii.ai/v/ISRG/sec166/page77]:

| Line | FY2025 | FY2024 | FY2023 | % of FY2025 |
|---|---|---|---|---|
| Instruments & Accessories | $6,018.9M | $5,079.0M | $4,276.6M | 59.8% |
| Systems | $2,473.7M | $1,966.0M | $1,679.7M | 24.6% |
| Total product | $8,492.6M | $7,045.0M | $5,956.3M | 84.4% |
| Service | $1,572.1M | $1,307.1M | $1,167.8M | 15.6% |
| **Total** | **$10,064.7M** | $8,352.1M | $7,124.1M | — |

(XBRL cross-check: identical values from RevenueFromContractWithCustomerExcludingAssessedTax, isrg-20251231.htm, source_authority 3.) [https://agentii.ai/v/ISRG/sec166/page77]

**By geography (FY2025)**: U.S. 68% / OUS 32% (2023: 66/34; 2024: 67/33) — U.S. share *rising* [FACT] [https://agentii.ai/v/ISRG/sec166/page77]. ~24% of revenue is foreign-currency-denominated [FACT] [https://agentii.ai/v/ISRG/sec166/page77]. Q2-2026: U.S. 67% / OUS 33% [FACT] [https://agentii.ai/v/ISRG/sec172/page38].

**By user type**: 100% B2B — hospitals, healthcare facilities, IDN groups; no consumer revenue [FACT] [https://agentii.ai/v/ISRG/sec166/page14].

**By end market (procedures)**: FY2025 — 3,153,000 da Vinci procedures (+18%): U.S. +15%, OUS +23%; 144,100 Ion procedures (+51%) [FACT] [https://agentii.ai/v/ISRG/sec166/page69], [https://agentii.ai/v/ISRG/sec166/page78]. Largest growth: general surgery (cholecystectomy, hernia repair, appendectomy, colorectal), gynecology, urology; U.S. bariatric declined high-single-digits [FACT] [https://agentii.ai/v/ISRG/sec166/page78]. Q2-2026: 889,000 da Vinci (+15%) and 47,900 Ion (+36%) procedures [FACT] [https://agentii.ai/v/ISRG/sec172/page32].

**Concentration risk matrix**:
| Dimension | Largest exposure | Share | >20%? |
|---|---|---|---|
| Product line | Instruments & Accessories | 59.8% | YES [https://agentii.ai/v/ISRG/sec166/page77] |
| Geography | U.S. | 68% | YES [https://agentii.ai/v/ISRG/sec166/page77] |
| Customer | not disclosed | — | Coverage gap |

**Temporal comparison**: Q2-2026 total revenue $2,892.3M (+19% YoY); I&A $1,734.9M (+18%); Systems $685.0M (+19%); Service $472.4M (+21%) [FACT] [https://agentii.ai/v/ISRG/sec172/page38]. Contracted backlog visibility: remaining performance obligations $3.0B at 12/31/2025 → $3.4B at 6/30/2026, ~half recognized within 12 months [FACT] [https://agentii.ai/v/ISRG/sec166/page108], [https://agentii.ai/v/ISRG/sec172/page12].

## PIL-3 Direct Test Input — Software/Subscription Slice per Deployed Unit

PIL-3 falsifier: `model_layer_revenue_per_deployed_unit_usd > 5000` (model-layer revenue **includes** per-unit software/subscription revenue).

**Disclosed subscription-bearing per-unit fees** [FACT]:
- Service contracts (attach at system sale/lease): $95,000–$225,000 per system per year, "maintenance support ... includes service care plans ... **software upgrades and updates**, as well as a customer portal" [https://agentii.ai/v/ISRG/sec166/page77], [https://agentii.ai/v/ISRG/sec166/page11]. Ion service: $55,000–$70,000/year [https://agentii.ai/v/ISRG/sec166/page77].
- My Intuitive+ digital subscription (da Vinci 5): "digital subscription package" — but "we do not currently generate material revenue from these offerings" [FACT] [https://agentii.ai/v/ISRG/sec166/page11], [https://agentii.ai/v/ISRG/sec166/page77].
- Usage-based operating leases: per-procedure system+service pricing, $531M variable lease revenue FY2025 [FACT] [https://agentii.ai/v/ISRG/sec166/page78].

**Per deployed unit (installed base 12,101 at 12/31/2025)** [DEDUCTED]:
- Service revenue per unit: $1,572.1M ÷ 12,101 = **$129.9K/year** [components: sec166 page77 + page69]
- Recurring revenue per unit: $8,465.3M ÷ 12,101 = **$699.6K/year** [sec166 page78 + page69]
- Q2-2026 (12,806 units): service $472.4M → $36.9K/quarter (~$147.6K annualized); recurring $2,469.1M → $192.8K/quarter [sec172 page40 + page32]
- I&A per procedure: FY2025 $1,826; Q2-2026 $1,852 [DEDUCTED] [https://agentii.ai/v/ISRG/sec166/page69], [https://agentii.ai/v/ISRG/sec172/page32]

**[VIEW]** Under PIL-3's own definition (model-layer revenue INCLUDES per-unit software/subscription revenue), ISRG falsifies the pillar: even the narrowest subscription-bearing slice (service contracts, which bundle software upgrades) is $95K–$225K/unit/year — 19x–45x the $5,000 threshold; realized $129.9K. **[VIEW]** If "model layer" is instead restricted to standalone digital subscriptions (My Intuitive+, Case Insights, 3D Models), ISRG supports PIL-3 — that slice is immaterial (~$0/unit). The pillar cannot hold under its inclusive definition for the subscription case; the synthesis must resolve the boundary. **[VIEW]** The disclosed non-materiality of digital-subscription revenue shows ISRG monetizes model-layer compute indirectly (system ASP $1.60M FY2025 → $1.66M H1-2026) rather than via per-unit software fees [https://agentii.ai/v/ISRG/sec166/page78], [https://agentii.ai/v/ISRG/sec172/page40].

## Coverage Gaps & Citations

- **Customer-level concentration**: no single-customer or top-10-customer revenue disclosure in 10-K/10-Q.
- **Digital-subscription dollars**: "not material" — no quantified My Intuitive+ pricing or revenue.
- **Service contract split**: hardware maintenance vs software-upgrade share of the $95K–$225K fee not disclosed.
- **Product-line operating margins**: only gross margins disclosed (product 66.3%, service 64.6% FY2025) [https://agentii.ai/v/ISRG/sec166/page79].

**Citations (roll-up)**: sec166 pages 11, 14, 69, 77, 78, 79, 108; sec172 pages 12, 32, 38, 40; XBRL isrg-20251231.htm.

## Verification Table (number → tool call)

| Number | Value | Tool call |
|---|---|---|
| FY2025 revenue | $10,064.7M | search_xbrl_facts + sec166 page77 |
| I&A share | 59.8% | sec166 page77 (derived) |
| U.S. / OUS share | 68% / 32% | sec166 page77 |
| Recurring FY2025 / Q2-2026 | $8,465.3M (84%) / $2,469.1M (85%) | sec166 page78; sec172 page40 |
| Op-lease revenue FY2025 | $874.3M ($530.9M variable) | sec166 page109 |
| Installed base | 12,101 (12/31/25); 12,806 (6/30/26) | sec166 page69; sec172 page32 |
| I&A per procedure | $1,826 FY2025; $1,852 Q2-2026 | derived, cited above |
| Service per unit | $129.9K/year | derived, cited above |
| Service contract fee range | $95K–$225K/system/year | sec166 page77 |
| RPO | $3.0B (12/31/25); $3.4B (6/30/26) | sec166 page108; sec172 page12 |
| Digital solutions revenue | not material | sec166 page77 |
