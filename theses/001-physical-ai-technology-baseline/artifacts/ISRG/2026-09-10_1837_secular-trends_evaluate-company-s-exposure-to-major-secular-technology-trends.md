---
artifact_id: "001-ISRG-secular-trends-evaluate-company-s-exposure-to-major-secular-technology-trends-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: ISRG
skill: secular-trends
mode: evaluate-company-s-exposure-to-major-secular-technology-trends
affix: tech-trends
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "e6b41dbb2426"
as_of: 2026-09-10
entity_claims:
  - "ISRG da Vinci installed base was approximately 11,106 systems as of 2025-12-31, +12% YoY (sec166/page69)"
  - "ISRG performed approximately 3,153,000 da Vinci procedures in calendar 2025, +18% YoY (sec166/page69)"
  - "ISRG recurring revenue was 84% of total revenue in 2025, $8.47B of $10.06B (sec166/page78)"
  - "ISRG exited Q2 2026 with almost 13 thousand installed systems worldwide (ect75/page1)"
citations: []
pillars_addressed: [PIL-1, PIL-3, PIL-4]
claim_state: pinned
key_metrics:
  revenue_fy2025_usd_b: 10.06
  recurring_revenue_pct_fy2025: 84
  da_vinci_procedures_fy2025_m: 3.153
  da_vinci_installed_base_2025: 11106
  da_vinci_placements_fy2025: 1721
  ion_installed_base_2025: 995
  r_and_d_fy2025_usd_m: 1311.8
conclusions:
  - "ISRG is the canonical reference curve for embodied-AI-at-scale deployment: ~12.1k systems, ~3.15M annual procedures, 84% recurring revenue."
  - "AI/data exposure is HIGH but is deployed as augmentation of a teleoperated platform, not as autonomy."
  - "Adoption is procedure-driven (utilization +3%) more than unit-driven, with capital placements as the lagging variable."
facts_count: 41
deducted_count: 4
views_count: 3
citation_count: 14
---

# ISRG — Exposure to Major Secular Technology Trends (Mode 1)

## Executive Summary

Intuitive Surgical (ISRG) is the robotic-reliability benchmark for the physical-AI thesis: the only US-listed company with a decade-plus of surgical-robot deployment disclosure. FY2025 revenue reached $10.1B, up 21% [FACT] (https://agentii.ai/v/ISRG/sec166/page69), on approximately 3,153,000 da Vinci procedures, +18% [FACT] (https://agentii.ai/v/ISRG/sec166/page69), with an installed base of approximately 11,106 da Vinci systems (+12%) and 995 Ion systems (+24%) [FACT] (https://agentii.ai/v/ISRG/sec166/page69). Recurring revenue is 84% of total [FACT] (https://agentii.ai/v/ISRG/sec166/page78). ISRG's exposure to AI and data-platform trends is HIGH and increasing (da Vinci 5 carries >10,000x the compute of Xi and an AI-driven Case Insights layer [FACT] (https://agentii.ai/v/ISRG/sec166/page8)), while GLP-1-driven bariatric decline and China domestic-robot competition are measurable headwinds [FACT] (https://agentii.ai/v/ISRG/sec166/page71). The company invests across AI/ML as one of several technology domains — not as a stand-alone strategy [FACT] (https://agentii.ai/v/ISRG/ect75/page1). [VIEW] ISRG's utilization-led growth profile (procedures per system per year +3% [FACT] (https://agentii.ai/v/ISRG/sec166/page69)) is the closest published analogue to how embodied-AI unit economics will actually scale.

## Trend Exposure Matrix

| Secular trend | Exposure | Core evidence (all cited inline) |
|---|---|---|
| Embodied AI / surgical robotics | **Core business** | 11,106-system installed base, 1,721 placements in 2025 incl. 870 da Vinci 5 units [FACT] (https://agentii.ai/v/ISRG/sec166/page69) |
| AI & machine-learning software | **High, rising** | da Vinci 5 "more than 10,000 times the computing power of da Vinci Xi" enabling Case Insights (computational observer) [FACT] (https://agentii.ai/v/ISRG/sec166/page8); management names AI and ML among domains receiving "sustained investment" [FACT] (https://agentii.ai/v/ISRG/ect75/page1) |
| Data platforms & analytics | **High** | Digital Solutions "powered by our vast network of connected surgical systems" [FACT] (https://agentii.ai/v/ISRG/sec166/page11); My Intuitive offers anonymized national benchmarks [FACT] (https://agentii.ai/v/ISRG/sec166/page11) |
| Cloud & edge computing | **Medium** | Intuitive Hub edge-computing system [FACT] (https://agentii.ai/v/ISRG/sec166/page8); cloud-enabled SimNow simulation [FACT] (https://agentii.ai/v/ISRG/sec166/page10) |
| VR simulation / digital training | **Medium** | SimNow provides quantitative performance assessment of skills exercises [FACT] (https://agentii.ai/v/ISRG/sec166/page10) |
| Telepresence / remote collaboration | **Medium** | Telepresence technology and dual-surgeon consoles [FACT] (https://agentii.ai/v/ISRG/sec166/page10); My Intuitive+ bundles telepresence, simulation, AI-driven Case Insights [FACT] (https://agentii.ai/v/ISRG/ect75/page2) |
| Pharmacologic substitution (GLP-1) | **Negative headwind** | US bariatric procedures declined high-single digits in 2025 [FACT] (https://agentii.ai/v/ISRG/sec166/page71); continued in Q2 2026 [FACT] (https://agentii.ai/v/ISRG/ect75/page2) |
| China industrial policy / domestic robots | **Negative headwind** | Governance campaign + domestic competition cut placements below expectations in 2025 [FACT] (https://agentii.ai/v/ISRG/sec166/page73); only 2 systems placed in China in Q2 2026 [FACT] (https://agentii.ai/v/ISRG/ect75/page2) |

## Core Analysis

### 1. The deployment curve (pillar context: PIL-4)
2025: 1,721 da Vinci systems placed (+13% vs 1,526), of which 870 were next-generation da Vinci 5 (vs 362 in 2024) [FACT] (https://agentii.ai/v/ISRG/sec166/page69). Ion placements fell 28% to 195 as US customers "shifted from increasing capacity to increasing utilization" [FACT] (https://agentii.ai/v/ISRG/sec166/page73). By Q2 2026 the combined fleet was "almost 13 thousand systems installed worldwide" [FACT] (https://agentii.ai/v/ISRG/ect75/page1). [DEDUCTED] A single-vendor, capital-constrained, hospital-procured robot platform took ~25 years to reach ~12-13k units; annual incremental deployments are ~1.7-2.0k/year — this is the empirical floor-rate reference against which any claim of >10,000 general-purpose humanoid units deployed by 2027-Q4 (PIL-4 wrong_if) must be stress-tested.

### 2. Utilization, not units, is the adoption engine
da Vinci system utilization (procedures per system per year) rose 3% in 2025 [FACT] (https://agentii.ai/v/ISRG/sec166/page69); Ion utilization +11% in Q2 2026 [FACT] (https://agentii.ai/v/ISRG/ect75/page2). [DEDUCTED] Approximate procedures per installed da Vinci system ≈ 284 per year in 2025 (3,153k procedures ÷ 11,106 systems, both from https://agentii.ai/v/ISRG/sec166/page69). [VIEW] Embodied-AI adoption is a utilization-led, procedure-data flywheel first and a hardware-shipment story second; ISRG's 84% recurring revenue mix [FACT] (https://agentii.ai/v/ISRG/sec166/page78) is the financial proof.

### 3. R&D capacity and AI regulation posture
R&D expense was $1,311.8M in 2025 vs $1,145.3M in 2024, 13.0% of revenue [FACT] (https://agentii.ai/v/ISRG/sec166/page91), and management states R&D is intentionally growing faster than SG&A [FACT] (https://agentii.ai/v/ISRG/ect75/page2). Headcount was 17,021 at fiscal-year-end [FACT] (https://agentii.ai/v/ISRG/sec166/page25). The 10-K dedicates a full risk factor to AI regulation: EU AI Act substantive requirements apply from August 2, 2026 with fines up to 7% of worldwide annual turnover, plus a revised EU Product Liability Directive and US state-level AI laws (Colorado, California, Connecticut; Illinois and New York for health AI) [FACT] (https://agentii.ai/v/ISRG/sec166/page39). [DEDUCTED] ISRG is already operating inside the AI-governance regime that general-purpose humanoids will face in the EU from 2026.

### 4. Revenue and margin trajectory
Total revenue $10,064.7M in 2025 vs $8,352.1M in 2024 vs $7,124.1M in 2023 (income statement) [FACT] (https://agentii.ai/v/ISRG/sec166/page91); XBRL fact RevenueFromContractWithCustomerExcludingAssessedTax matches exactly at $10,064.7M for FY2025 [FACT] (search_xbrl_facts, verified against https://agentii.ai/v/ISRG/sec166/page91). Q2 2026 revenue rose 19% to $2.89B with recurring revenue 85% of total [FACT] (https://agentii.ai/v/ISRG/ect75/page2). da Vinci ASP ≈ $1.60M in 2025 vs $1.50M in 2024 [FACT] (https://agentii.ai/v/ISRG/sec166/page78). GAAP gross margin 66.0% in 2025 [FACT] (https://agentii.ai/v/ISRG/sec166/page69); non-GAAP 70% in Q2 2026 (68.7% ex one-time tariff refund) [FACT] (https://agentii.ai/v/ISRG/ect75/page2). [VIEW] 66-70% gross margin on a robotic hardware+razor/blade model demonstrates the pricing power an embodied-AI platform earns once reliability and procedure data compound.

### 5. Trend headwinds
US bariatric procedure decline (GLP-1 substitution) [FACT] (https://agentii.ai/v/ISRG/sec166/page71); China tender delays, provincial pricing limits, and domestic competition [FACT] (https://agentii.ai/v/ISRG/sec166/page73). Product-defect risk disclosure underscores that electromechanical reliability failures carry clinical consequences — ISRG voluntarily recalled products in the past [FACT] (https://agentii.ai/v/ISRG/sec166/page37). [DEDUCTED] Even the reliability benchmark discloses defect and recall risk; for humanoids (PIL-3) the reliability gate is the binding constraint, not unit economics.

## Coverage Gaps & Citations

Coverage gaps:
- 10-Q citation_ids were not surfaced by search_documents; Q2 2026 quarterly figures are therefore cited via the earnings-call transcript (ect75) and XBRL facts (source: 10-Q accession 0001035267-26-000058).
- Second-revenue-concept verification (P2.1): us-gaap `Revenues` and `RevenueFromContractWithCustomerIncludingAssessedTax` returned zero facts for ISRG; verification performed XBRL fact vs. 10-K income statement (page91) vs. MD&A highlights (page69) instead.
- No market-price data used (market_data_stage: none).
- search_by_analogue returned no entries tagged for robotics/technology-adoption analogues.

Citations (roll-up index):
1. https://agentii.ai/v/ISRG/sec166/page69 — 2025 operational & financial highlights
2. https://agentii.ai/v/ISRG/sec166/page71 — da Vinci procedures by region/specialty 2023-2025
3. https://agentii.ai/v/ISRG/sec166/page72 — OUS procedures, Ion procedures & installed base
4. https://agentii.ai/v/ISRG/sec166/page73 — placements by region 2023-2025
5. https://agentii.ai/v/ISRG/sec166/page78 — systems revenue, ASP, recurring revenue
6. https://agentii.ai/v/ISRG/sec166/page8 — da Vinci 5 architecture, Case Insights, Intuitive Hub
7. https://agentii.ai/v/ISRG/sec166/page10 — learning technologies, SimNow, Advanced Insights Suite
8. https://agentii.ai/v/ISRG/sec166/page11 — digital solutions, My Intuitive, connected fleet
9. https://agentii.ai/v/ISRG/sec166/page25 — human capital (headcount 17,021)
10. https://agentii.ai/v/ISRG/sec166/page37 — product defect/reliability risk factor
11. https://agentii.ai/v/ISRG/sec166/page39 — AI regulatory landscape (EU AI Act, US EOs, state laws)
12. https://agentii.ai/v/ISRG/sec166/page91 — consolidated income statements 2023-2025
13. https://agentii.ai/v/ISRG/ect75/page1 — Q2 2026 CEO remarks
14. https://agentii.ai/v/ISRG/ect75/page2 — Q2 2026 CFO remarks

## Verification (call trace)

| Material number | Value | Tool call that produced it |
|---|---|---|
| FY2025 revenue | $10,064.7M | search_xbrl_facts (RevenueFromContractWithCustomerExcludingAssessedTax, FY2025) + read_source_pages sec166 page91 |
| FY2025 procedures | 3,153,000 | read_source_pages sec166 page69/page71 |
| Installed base 2025-12-31 | 11,106 da Vinci; 995 Ion | read_source_pages sec166 page69/page73 |
| 2025 placements | 1,721 (870 da Vinci 5); 195 Ion | read_source_pages sec166 page69/page73 |
| Utilization growth | +3% da Vinci (2025); +11% Ion (Q2 2026) | read_source_pages sec166 page69; ect75 page2 |
| Recurring revenue | $8,465.3M = 84% (2025) | read_source_pages sec166 page78 |
| ASP | $1.60M (2025) | read_source_pages sec166 page78 |
| FY2025 R&D | $1,311.8M | search_xbrl_facts (ResearchAndDevelopmentExpense) + read_source_pages sec166 page91 |
| Q2 2026 revenue | $2,892.3M (+19%) | search_xbrl_facts + get_company_financials + read_source_pages ect75 page2 |
| Q2 2026 placements | 468 da Vinci, 55 Ion | read_source_pages ect75 page1 |
| Fleet at Q2 2026 exit | ~13,000 systems | read_source_pages ect75 page1 |
| Headcount | 17,021 | read_source_outline sec166 page25 |
| Gross margin | 66.0% GAAP FY2025; 70% non-GAAP Q2 2026 | read_source_pages sec166 page69; ect75 page2 |
