---
artifact_id: "001-ISRG-secular-trends-deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: ISRG
skill: secular-trends
mode: deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure
affix: tech-trends
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "e6b41dbb2426"
as_of: 2026-09-10
entity_claims:
  - "ISRG digital solutions are powered by a vast network of connected surgical systems (sec166/page11)"
  - "ISRG recurring revenue was $8,465.3M = 84% of FY2025 revenue, the financial embodiment of its data/consumables flywheel (sec166/page78)"
  - "ISRG tracks da Vinci I&A revenue per procedure ($1.83k in Q2 2026), the unit of data-linked monetization (ect75/page2)"
  - "My Intuitive+ digital subscription had zero opt-outs in its first renewal wave (ect75/page2)"
citations: []
pillars_addressed: [PIL-1, PIL-3, PIL-4]
claim_state: pinned
key_metrics:
  connected_fleet_2025: 12101
  da_vinci_procedures_2025_m: 3.153
  ion_procedures_2025_k: 144.1
  recurring_revenue_fy2025_usd_m: 8465.3
  recurring_revenue_pct: 84
  i_and_a_revenue_per_procedure_q2_2026_usd: 1830
  cumulative_ion_procedures_q2_2026_k: 400
conclusions:
  - "ISRG's data flywheel — procedures, consumables, connected-system telemetry, insights, training — is the company's primary moat, valued at 84% of revenue on a recurring basis."
  - "The 10,000x compute upgrade in da Vinci 5 was directed at data capture and insight products, not autonomy — empirical support for PIL-1 (embodied AI is data-bound, not compute-bound)."
  - "Per-system data economics (~$762k recurring revenue per system-year) define the reference unit economics for embodied-AI fleets."
facts_count: 36
deducted_count: 5
views_count: 3
citation_count: 11
---

# ISRG — Deep-Dive Data Value Trend Assessment (Mode 3)

## Executive Summary

ISRG is a data company wrapped in a surgical-robot company. Its digital solutions are explicitly "powered by our vast network of connected surgical systems" [FACT] (https://agentii.ai/v/ISRG/sec166/page11): a fleet of 11,106 da Vinci and 995 Ion systems at end-2025 [FACT] (https://agentii.ai/v/ISRG/sec166/page69) generating approximately 3,153,000 da Vinci and 144,100 Ion procedures in 2025 [FACT] (https://agentii.ai/v/ISRG/sec166/page69), with cumulative procedure counts exceeding 13 million on da Vinci Xi [FACT] (https://agentii.ai/v/ISRG/ect75/page1) and 400 thousand on Ion [FACT] (https://agentii.ai/v/ISRG/ect75/page1). The financial embodiment of the data flywheel is 84% recurring revenue ($8,465.3M of $10,064.7M in FY2025) [FACT] (https://agentii.ai/v/ISRG/sec166/page78). Data products are monetizing today — My Intuitive+ subscriptions with AI-driven Case Insights saw zero opt-outs in their first renewal wave [FACT] (https://agentii.ai/v/ISRG/ect75/page2). [VIEW] ISRG is the thesis's cleanest evidence that embodied-AI economics are data-bound (PIL-1): the compute upgrade was spent on data capture and insight products, not autonomy.

## 1. Data Asset Inventory

- **Fleet telemetry**: 12,101 connected systems at 2025-12-31 (11,106 da Vinci + 995 Ion) [FACT] (https://agentii.ai/v/ISRG/sec166/page69); "almost 13 thousand systems installed worldwide" by Q2 2026 exit [FACT] (https://agentii.ai/v/ISRG/ect75/page1). The fleet "enables Intuitive to proactively monitor product performance with high uptime reliability, as well as to provide timely software updates" [FACT] (https://agentii.ai/v/ISRG/sec166/page11).
- **Procedure data**: 3,153,000 da Vinci procedures in 2025 (+18%) [FACT] (https://agentii.ai/v/ISRG/sec166/page69), 144,100 Ion procedures (+51%) [FACT] (https://agentii.ai/v/ISRG/sec166/page69). [DEDUCTED] At 3.15M procedures/year across 11,106 systems, each system generates approximately 284 procedures per year — a per-unit data stream of roughly one procedure per working day [DEDUCTED] (computed from https://agentii.ai/v/ISRG/sec166/page69).
- **Clinical evidence corpus**: 25+ years of published studies; Q2 2026 call cites appendectomy (66% decreased complication risk vs laparoscopy) and force-feedback nephrectomy studies [FACT] (https://agentii.ai/v/ISRG/ect75/page3).

## 2. Data Infrastructure & Capture

The da Vinci 5 "incorporates an OR informatics platform that integrates multiple applications and data sets to help orchestrate medical procedure workflows and powers data insights to Intuitive customers" [FACT] (https://agentii.ai/v/ISRG/sec166/page11). Capture happens at the edge: Intuitive Hub edge-computing system [FACT] (https://agentii.ai/v/ISRG/sec166/page8), supported by the >10,000x compute step over Xi [FACT] (https://agentii.ai/v/ISRG/sec166/page8). Products are "secure-by-design, cloud-enabled" [FACT] (https://agentii.ai/v/ISRG/sec166/page11). [DEDUCTED] ISRG's architecture — edge capture, cloud aggregation, secure-by-design — is the exact pattern PIL-1 predicts for embodied-AI fleets: compute follows data, and data is captured at the point of physical work.

## 3. Data Products

- **My Intuitive**: mobile/web app giving customers "individual or program-level data… comparisons of those insights with anonymized national benchmarks" [FACT] (https://agentii.ai/v/ISRG/sec166/page11). The benchmark value scales with fleet data — a network effect.
- **My Intuitive+**: digital subscription for da Vinci 5 — surgical video and data "collected to objectively understand their surgical performance" [FACT] (https://agentii.ai/v/ISRG/sec166/page11); CFO confirms "AI driven case insights" in the bundle [FACT] (https://agentii.ai/v/ISRG/ect75/page2).
- **Case Insights / Insights Engine**: the "computational observer" and the Advanced Insights Suite [FACT] (https://agentii.ai/v/ISRG/sec166/page8).
- **Custom Hospital Analytics**: integration of data sources so "individual health institutions can analyze their data in their own environment" [FACT] (https://agentii.ai/v/ISRG/sec166/page11).
- **SimNow**: cloud-enabled simulation with "quantitative assessment of user performance" and real-time performance tracking dashboards [FACT] (https://agentii.ai/v/ISRG/sec166/page10).
- **Intuitive 3D Models**: augmented-reality product; CT/MR scans run "through segmentation algorithms" with technician revision and radiologist review [FACT] (https://agentii.ai/v/ISRG/sec166/page11). [VIEW] The human-in-the-loop (radiologist review) in the AI pipeline is the same safety pattern the thesis predicts will gate humanoid deployment (PIL-3).

## 4. Data Monetization

Recurring revenue (instruments & accessories + service + operating leases) reached $8,465.3M in 2025, 84% of total revenue, up from $7,040.3M (84%) in 2024 [FACT] (https://agentii.ai/v/ISRG/sec166/page78). Components: I&A $6,018.9M; service $1,572.1M (+20%); operating lease revenue $874.3M, of which $531M was usage-based variable lease revenue [FACT] (https://agentii.ai/v/ISRG/sec166/page78). In Q2 2026 recurring revenue hit 85% of total [FACT] (https://agentii.ai/v/ISRG/ect75/page2). The per-procedure data-linked unit is tracked quarterly: da Vinci I&A revenue per procedure ≈ $1.83 thousand [FACT] (https://agentii.ai/v/ISRG/ect75/page2). [DEDUCTED] Recurring revenue per installed da Vinci system ≈ $762 thousand per year ($8,465.3M ÷ 11,106 systems; sources https://agentii.ai/v/ISRG/sec166/page78 and https://agentii.ai/v/ISRG/sec166/page69) — a reference unit-economics figure for embodied-AI fleet monetization.

## 5. Data-Driven Decisions

- **Market intelligence**: US Ion penetration of lung biopsies is "approaching the halfway point of all lung biopsies performed," which shifted customer focus from capacity to utilization [FACT] (https://agentii.ai/v/ISRG/sec166/page73).
- **Product strategy from internal data**: the 2027 extended-use instrument program was validated by re-examining the 2020 program — "we have had the time to assess the impact of that both in our own data trends and in feedback from customers" [FACT] (https://agentii.ai/v/ISRG/ect75/page3).
- **Utilization as the KPI**: da Vinci utilization (procedures/system/year) +3% in 2025 [FACT] (https://agentii.ai/v/ISRG/sec166/page69); Ion +11% and US SP +25% in Q2 2026 [FACT] (https://agentii.ai/v/ISRG/ect75/page2). [DEDUCTED] ISRG manages its fleet like a data-product company manages DAU — utilization, not shipments, is the disclosed health metric.

## 6. Data Moat & Governance

The training flywheel (Intuitive Learning, SimNow, remote proctoring) [FACT] (https://agentii.ai/v/ISRG/sec166/page10) compounds data value: every trained surgeon adds procedure volume that adds benchmark data. Governance is costed and disclosed: GDPR automated-decision-making scope expansion via CJEU case law, plus HIPAA/CCPA-style data-privacy regimes [FACT] (https://agentii.ai/v/ISRG/sec166/page39); product-defect and recall risk around software failures [FACT] (https://agentii.ai/v/ISRG/sec166/page37); China provincial pricing limits on instruments & accessories [FACT] (https://agentii.ai/v/ISRG/sec166/page37). [VIEW] The data moat is durable because it is anchored in physical-world reliability and regulatory trust, not just dataset size.

## Coverage Gaps & Citations

Coverage gaps:
- No disclosure retrieved quantifying dataset sizes (hours of surgical video, procedure-recording volume) — the data corpus is evidenced indirectly via procedure counts and product descriptions.
- 10-Q citation_ids not surfaced; quarterly data cited via ect75 transcript and XBRL facts (10-Q accession 0001035267-26-000058).
- No price/market data used (market_data_stage: none).
- Second revenue concept (us-gaap:Revenues, RevenueFromContractWithCustomerIncludingAssessedTax) returned zero facts for ISRG; verification done XBRL vs income statement (sec166/page91) vs MD&A (sec166/page69).

Citations (roll-up index):
1. https://agentii.ai/v/ISRG/sec166/page8 — da Vinci 5 compute, Case Insights, Intuitive Hub
2. https://agentii.ai/v/ISRG/sec166/page10 — SimNow, Advanced Insights Suite, learning technology
3. https://agentii.ai/v/ISRG/sec166/page11 — digital solutions, My Intuitive(+), 3D Models, connected fleet
4. https://agentii.ai/v/ISRG/sec166/page37 — defect risk; China provincial pricing
5. https://agentii.ai/v/ISRG/sec166/page39 — GDPR/AI governance
6. https://agentii.ai/v/ISRG/sec166/page69 — 2025 highlights (procedures, fleet, utilization)
7. https://agentii.ai/v/ISRG/sec166/page73 — placements, Ion penetration estimate
8. https://agentii.ai/v/ISRG/sec166/page78 — recurring revenue detail
9. https://agentii.ai/v/ISRG/ect75/page1 — Q2 2026 CEO remarks (fleet ~13k, cumulative procedures)
10. https://agentii.ai/v/ISRG/ect75/page2 — Q2 2026 CFO remarks (My Intuitive+, per-procedure I&A, utilization)
11. https://agentii.ai/v/ISRG/ect75/page3 — data-driven extended-use rationale; clinical studies

## Verification (call trace)

| Material number | Value | Tool call that produced it |
|---|---|---|
| Fleet at 2025-12-31 | 11,106 da Vinci + 995 Ion | read_source_pages sec166 page69 |
| Fleet at Q2 2026 exit | ~13,000 | read_source_pages ect75 page1 |
| FY2025 procedures | 3,153,000 da Vinci; 144,100 Ion | read_source_pages sec166 page69 |
| Cumulative procedures | >13M Xi; >400k Ion | read_source_pages ect75 page1 |
| Recurring revenue FY2025 | $8,465.3M (84%) | read_source_pages sec166 page78 |
| Usage-based lease revenue | $531M (2025) | read_source_pages sec166 page78 |
| I&A revenue per procedure Q2 2026 | $1.83k | read_source_pages ect75 page2 |
| Utilization | da Vinci +3% (2025); Ion +11%, US SP +25% (Q2 2026) | read_source_pages sec166 page69; ect75 page2 |
| My Intuitive+ opt-outs | 0 | read_source_pages ect75 page2 |
| Ion US penetration estimate | approaching halfway point | read_source_pages sec166 page73 |
| Service revenue | $1,572.1M FY2025 | read_source_pages sec166 page78 |
