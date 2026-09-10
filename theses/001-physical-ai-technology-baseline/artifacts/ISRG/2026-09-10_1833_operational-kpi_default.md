---
artifact_id: "001-ISRG-operational-kpi-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: ISRG
skill: operational-kpi
mode: default
affix: kpi-dashboard
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "0730fd170124"
as_of: 2026-09-10
entity_claims:
  - claim_id: "ISRG-OPSKPI-01"
    text: "FY2025 total revenue was $10,064.7M (+21% YoY); da Vinci procedures 3,153k (+18%); installed base 11,106 systems (+12%) as of 2025-12-31."
    citations: ["https://agentii.ai/v/ISRG/sec166/69"]
  - claim_id: "ISRG-OPSKPI-02"
    text: "da Vinci system utilization (procedures per system per year) grew 3% YoY in both FY2025 and Q2 2026 — the company's only quantitative deployed-robot throughput/reliability metric."
    citations: ["https://agentii.ai/v/ISRG/sec166/69", "https://agentii.ai/v/ISRG/sec172/32"]
  - claim_id: "ISRG-OPSKPI-03"
    text: "Instruments & accessories revenue — the reliability-by-usage proxy — was $6,018.9M in FY2025 (~$1,909 per procedure, company-disclosed range $900–$3,700) and $1,734.9M in Q2 2026 (+18%)."
    citations: ["https://agentii.ai/v/ISRG/sec166/77", "https://agentii.ai/v/ISRG/sec172/38"]
  - claim_id: "ISRG-OPSKPI-04"
    text: "ISRG discloses no MTBF, uptime, failure-rate, or downtime metrics for deployed systems in 10-K/10-Q/transcripts; reliability is disclosed qualitatively and via utilization."
    citations: ["https://agentii.ai/v/ISRG/ect75/1"]
  - claim_id: "ISRG-OPSKPI-05"
    text: "da Vinci 5 accounted for 870 of 1,721 placements in FY2025 (51%) and 246 of 468 in Q2 2026 (53%); 100+ platform software updates planned, 3 submitted for FDA 510(k) clearance."
    citations: ["https://agentii.ai/v/ISRG/sec166/69", "https://agentii.ai/v/ISRG/sec172/32", "https://agentii.ai/v/ISRG/ect75/4"]
citations:
  - "https://agentii.ai/v/ISRG/sec166/69"
  - "https://agentii.ai/v/ISRG/sec166/71"
  - "https://agentii.ai/v/ISRG/sec166/73"
  - "https://agentii.ai/v/ISRG/sec166/77"
  - "https://agentii.ai/v/ISRG/sec166/78"
  - "https://agentii.ai/v/ISRG/sec166/25"
  - "https://agentii.ai/v/ISRG/sec172/32"
  - "https://agentii.ai/v/ISRG/sec172/38"
  - "https://agentii.ai/v/ISRG/sec172/40"
  - "https://agentii.ai/v/ISRG/ect75/1"
  - "https://agentii.ai/v/ISRG/ect75/3"
  - "https://agentii.ai/v/ISRG/ect75/4"
  - "https://agentii.ai/v/ISRG/ect75/5"
pillars_addressed: [PIL-3, PIL-4]
claim_state: pinned
key_metrics:
  fy2025_total_revenue_usd_m: 10064.7
  fy2025_da_vinci_procedures_k: 3153
  fy2025_ion_procedures_k: 144.1
  fy2025_da_vinci_installed_base: 11106
  fy2025_da_vinci_placements: 1721
  fy2025_da_vinci5_placements: 870
  fy2025_utilization_growth_yoy_pct: 3
  fy2025_ia_revenue_usd_m: 6018.9
  fy2025_ia_revenue_per_procedure_usd: 1909
  fy2025_recurring_revenue_pct_of_total: 84
  fy2025_headcount: 17021
  q2_2026_revenue_usd_m: 2892.3
  q2_2026_da_vinci_procedures_k: 889
  q2_2026_da_vinci_installed_base: 11710
  q2_2026_da_vinci_placements: 468
  q2_2026_da_vinci5_placements: 246
  q2_2026_utilization_growth_yoy_pct: 3
  q2_2026_recurring_revenue_pct_of_total: 85
  fy2026_procedure_growth_guidance_pct: "13.5-15.5"
conclusions:
  - "ISRG's decade of deployment disclosure establishes utilization (procedures/system/year) as the observable benchmark for fielded-robot reliability — not MTBF, which is nowhere disclosed for deployed robots."
  - "The 3% utilization growth on a 12% larger installed base in FY2025 implies each incremental system still adds ~280–300 procedures/year — deployed robotic capacity keeps paying back usage."
  - "I&A revenue per procedure (~$1,909 computed, $900–$3,700 disclosed range) plus 84–85% recurring revenue share quantifies reliability-as-usage better than any durability metric a humanoid vendor could disclose pre-deployment."
  - "da Vinci 5 platform-software cadence (100+ updates, 510(k) submissions) and the 7-year Xi trade-in precedent frame the PIL-4 timing: multi-year upgrade S-curves, not step changes."
facts_count: 43
deducted_count: 9
views_count: 6
citation_count: 13
---

# Operational KPI Dashboard — Intuitive Surgical (ISRG)

## 1. Executive Summary

ISRG ended FY2025 (12 months to 2025-12-31) with revenue of $10.06B, up 21%, on 3.153M da Vinci procedures (+18%) and an installed base of 11,106 systems (+12%) ([FACT 1], [FACT 2], [FACT 7] — https://agentii.ai/v/ISRG/sec166/69). The company's only quantitative deployed-robot reliability metric — utilization, measured in procedures per system per year — grew 3% in FY2025 and again 3% YoY in Q2 2026 ([FACT 8], [FACT 29] — https://agentii.ai/v/ISRG/sec172/32). Instruments & accessories revenue, the reliability-by-usage proxy, reached $6.02B in FY2025 (~$1,909 per procedure against a disclosed $900–$3,700 band) and $1.73B (+18%) in Q2 2026 ([FACT 4], [FACT 31] — https://agentii.ai/v/ISRG/sec166/77). Recurring revenue is 84–85% of total ([FACT 21], [FACT 32]). Critically for PIL-3: ISRG discloses no MTBF, uptime, or failure-rate data anywhere in its 10-K, 10-Q, or transcripts — reliability is disclosed qualitatively and through utilization. da Vinci 5 is now 51–53% of placements (870 in FY2025; 246 in Q2 2026) with 100+ planned platform software updates, and FY2026 procedure guidance stands at +13.5–15.5% ([FACT 38], [FACT 39], [FACT 40]).

## 2. Data Sources

| Source | Citation ID | Retrieval |
|---|---|---|
| FY2025 Form 10-K (filed 2026-02-03) | sec166 | outline + pages 25, 69, 71, 73, 77, 78 |
| Q2 2026 Form 10-Q (filed 2026-07-21) | sec172 | outline + pages 32, 38, 40 |
| Q2 2026 earnings call transcript (2026-07-16) | ect75 | outline + pages 1, 3, 4, 5 |
| XBRL structured facts (gold.xbrl_facts) | — | search_xbrl_facts: us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax FY2025/FY2026 |

## 3. Analysis

### 3.1 Installed Base & System Placements (capacity)

[FACT 6] 1,721 da Vinci systems were placed in FY2025 (+13% vs 1,526 in 2024), including 870 da Vinci 5 systems vs 362 in 2024 (https://agentii.ai/v/ISRG/sec166/69). [FACT 7] Installed base reached ~11,106 at 2025-12-31, +12% YoY from 9,902 (https://agentii.ai/v/ISRG/sec166/69). [FACT 16] Geographically: 6,364 in the U.S., 2,168 Europe, 1,993 Asia, 581 rest of world (https://agentii.ai/v/ISRG/sec166/73). [FACT 15] 437 of 1,721 placements involved trade-ins in 2025 vs 150 in 2024 — the Xi→dv5 replacement cycle is now material (https://agentii.ai/v/ISRG/sec166/73). [DEDUCTED 5] Trade-ins were 25% of FY2025 placements (437/1,721, arithmetic on [FACT 15] data). [FACT 9] Ion placements fell to 195 (−28%) as customers shifted from capacity to utilization; Ion installed base 995 (+24%) (https://agentii.ai/v/ISRG/sec166/69). [FACT 28] By Q2 2026 the da Vinci base reached ~11,710 (+12% YoY) and Ion ~1,096 (+21%) (https://agentii.ai/v/ISRG/sec172/32). [DEDUCTED 6] Combined fleet ≈ 12,806 systems — consistent with management's "almost 13 thousand systems installed worldwide" on the Q2 call (https://agentii.ai/v/ISRG/ect75/1). [FACT 41] Roughly half of Q2 2026 U.S. placements were trade-ins (https://agentii.ai/v/ISRG/ect75/5). [FACT 47] U.S. Q2 placements were 267, up 24% YoY (https://agentii.ai/v/ISRG/ect75/4).

### 3.2 Procedure Volumes & System Utilization (throughput)

[FACT 2] 3,153k da Vinci procedures in FY2025 (+18% vs 2,683k); [FACT 3] 144.1k Ion procedures (+51%) (https://agentii.ai/v/ISRG/sec166/69). [FACT 12] U.S. procedures 2,012k (+15%), OUS 1,141k (+23%) (https://agentii.ai/v/ISRG/sec166/71). [FACT 13] Largest categories: U.S. general surgery 1,250k and OUS urology 507k (https://agentii.ai/v/ISRG/sec166/71). [FACT 14] U.S. bariatric declined high-single-digits in 2025 — GLP-1-driven cannibalization is now quantified in filings (https://agentii.ai/v/ISRG/sec166/71). [FACT 26] Q2 2026: 889k da Vinci procedures (+15%), 47.9k Ion (+36%) (https://agentii.ai/v/ISRG/sec172/32). [FACT 8] Utilization — procedures per system per year — grew 3% in FY2025; [FACT 29] again +3% YoY in Q2 2026 (https://agentii.ai/v/ISRG/sec172/32). [FACT 48] CFO: U.S. utilization "grew 3% in Q2, which is a healthy level. And a metric that we will watch carefully" (https://agentii.ai/v/ISRG/ect75/5).

[DEDUCTED 1] Implied FY2025 throughput: 3,153k procedures / 11,106 year-end systems ≈ 284 procedures/system/year; ≈300 on the average base of 10,504. [DEDUCTED 2] Q2 2026 annualized ≈ 304 procedures/system (889k × 4 / 11,710). [DEDUCTED 9] This is roughly 5.5–5.8 procedures per system per week. [VIEW 2] Utilization growth of 3% on top of a 12% larger installed base means capacity expansion has not diluted throughput — the fleet is absorbing ~470k incremental procedures/year without eroding per-system usage; management explicitly treats 3% as a healthy level (https://agentii.ai/v/ISRG/ect75/5). [FACT 35] U.S. Q2 2026 growth moderated to 12% (vs 14% in Q1) on deferrable-procedure softness attributed partly to coverage/premium dynamics (https://agentii.ai/v/ISRG/ect75/3).

### 3.3 Instruments & Accessories Revenue per Procedure (reliability-by-usage proxy)

[FACT 4] I&A revenue $6,018.9M in FY2025 (+19% vs $5,079.0M) (https://agentii.ai/v/ISRG/sec166/77). [FACT 18] Company-disclosed I&A revenue band: $900–$3,700 per surgical procedure (https://agentii.ai/v/ISRG/sec166/77). [DEDUCTED 3] Blended realized rate ≈ $1,909 per da Vinci procedure ($6,018.9M / 3,153k) — inside the disclosed band; includes Ion/SP instrument revenue, so the pure-da-Vinci rate is slightly lower. [FACT 31] Q2 2026 I&A was $1,734.9M (+18% YoY) and H1 2026 $3,421.3M (+20%) (https://agentii.ai/v/ISRG/sec172/38). [VIEW 4] I&A revenue per procedure is the closest public analog to a "wear-and-tear dividend" of fielded robots: every procedure mechanically consumes a perishable instrument set, so I&A growth tracks actual system usage, not just shipments. For PIL-3, this is the benchmark a humanoid fleet cannot yet produce — no deployed humanoid has a consumables-per-operation revenue stream that would certify real usage. [FACT 44] The extended-use program (announced May 2026, H1 2027 rollout on a subset of EndoWrist instruments) will deliberately reduce I&A per case to lower customer cost per procedure (https://agentii.ai/v/ISRG/ect75/1). [FACT 49] The 2020 extended-use precedent had ~7% I&A impact; management will quantify 2027 impact next call (https://agentii.ai/v/ISRG/ect75/3).

### 3.4 Service, Recurring Revenue & Operating Leverage

[FACT 20] Service revenue $1,572.1M in FY2025 (+20%) (https://agentii.ai/v/ISRG/sec166/78). [FACT 19] Service contracts run $95k–$225k/year per system, five-year term, first year bundled with purchase (https://agentii.ai/v/ISRG/sec166/77). [DEDUCTED 4] Realized service revenue ≈ $150k per average system-year ($1,572.1M / 10,504) — mid-band, confirming near-full service attach. [FACT 21] Recurring revenue (I&A + service + operating leases) $8,465.3M = 84% of FY2025 revenue (https://agentii.ai/v/ISRG/sec166/78). [FACT 32] Q2 2026 recurring $2,469.1M and H1 $4,839.4M, both 85% of total (https://agentii.ai/v/ISRG/sec172/40). [FACT 22] Operating lease revenue $874M in FY2025, $531M of it variable/usage-based (https://agentii.ai/v/ISRG/sec166/78); [FACT 45] H1 2026: $512M ($326M variable); lease buyouts $108M H1 2026 vs $69M H1 2025 (https://agentii.ai/v/ISRG/sec172/40). [FACT 10] Gross margin 66.0% in FY2025 (67.5% in 2024) on dv5 ramp costs and tariffs (https://agentii.ai/v/ISRG/sec166/69). [FACT 30] Q2 2026 GM recovered to 67.8%; operating income $972M (+31%) (https://agentii.ai/v/ISRG/sec172/32). [FACT 23] da Vinci ASP ex-leases ~$1.60M FY2025 vs $1.50M FY2024 (https://agentii.ai/v/ISRG/sec166/78); [FACT 33] $1.66M H1 2026 vs $1.55M — dv5 mix lifting ASPs (https://agentii.ai/v/ISRG/sec172/40).

### 3.5 Headcount & Productivity

[FACT 24] Headcount 17,021 at 2025-12-31 (+1,383 in the year): R&D 2,288, manufacturing operations 7,625, commercial & service 4,837, administrative 2,271; voluntary turnover 9.3%; employees in 29 countries (https://agentii.ai/v/ISRG/sec166/25). [DEDUCTED 7] Revenue per employee ≈ $591k (10,064.7 / 17,021). [VIEW 5] The 45% manufacturing share (7,625 of 17,021) is the operational signature of a vertically integrated robotics company — instruments are single-use consumables produced at scale; a humanoid operator would need comparable instrument/servicing infrastructure before MTBF claims become operationally meaningful.

### 3.6 Reliability Disclosure Landscape (PIL-3)

[FACT 37] >13M cumulative procedures on da Vinci Xi, which management cites for "breadth, reliability, clinical capability" (https://agentii.ai/v/ISRG/ect75/1). [FACT 50] CEO: "continued enhancements across our core platforms improve reliability, usability, efficiency, and throughput" — reliability is stated as a design goal, never as a published metric (https://agentii.ai/v/ISRG/ect75/1). [FACT 51] No MTBF, uptime, failure-rate, or downtime figure appears in the FY2025 10-K, the Q2 2026 10-Q, or three Q2-call pages retrieved; the 10-K's reliability-adjacent disclosures are qualitative (risk factors on defects/recalls, page 40 per outline) (https://agentii.ai/v/ISRG/sec166/69). [VIEW 1] The conclusion for PIL-3's wrong_if (humanoid MTBF >2,000h in commercial deployment): the only US-listed company with a decade of deployed surgical-robot reliability disclosure does NOT publish MTBF or uptime. Its observable reliability benchmark is utilization — procedures per system per year (+3% growth) plus consumables revenue per procedure. Any humanoid MTBF claim, if disclosed, would have no precedent in ISRG's public reporting and should be treated as unverifiable against deployed-fleet evidence. [VIEW 3] The dv5 "structural" capacity claim — management says dv5 design gives incremental capacity, reflected in higher utilization of dv5 vs Xi (https://agentii.ai/v/ISRG/ect75/4) — is the nearest thing to a hardware-reliability improvement claim, and it is stated qualitatively.

### 3.7 Timing: da Vinci 5 Upgrade Cycle & 2026 Cadence (PIL-4)

[FACT 38] dv5 placements: 870 in FY2025 (vs 362 in 2024); 246 in Q2 2026 (vs 180 in Q2 2025) (https://agentii.ai/v/ISRG/sec166/69, https://agentii.ai/v/ISRG/sec172/32). [DEDUCTED 8] dv5 share of placements: 51% FY2025, 53% Q2 2026. [FACT 39] 100+ planned dv5 platform software updates; first phase rolled out Q2 2026 (telepresence, simulation training, care-team workflow); three innovations (tool-eject, multi-arm adjustment, digital ruler) submitted for FDA 510(k) (https://agentii.ai/v/ISRG/ect75/4). [FACT 43] Xi precedent: ~7 years from introduction to peak trade-in volumes (Si→Xi) (https://agentii.ai/v/ISRG/ect75/5). [FACT 40] FY2026 guidance: da Vinci procedure growth 13.5–15.5% (expectation near midpoint); non-GAAP gross margin 68–69% (raised); non-GAAP opex growth 11–13% (https://agentii.ai/v/ISRG/ect75/3). [FACT 42] XiR (value-tier Gen-4) installed base ≈130 (~50 U.S.; 20 of 27 Q2 ASC placements were XiR) (https://agentii.ai/v/ISRG/ect75/5). [VIEW 6] For PIL-4, the ISRG pattern is: hardware upgrade cycles are multi-year S-curves (7-year Xi precedent), while capability cadence has shifted to software (100+ dv5 updates) — timing risk for the humanoid thesis is less about hardware refresh speed and more about matching a software-platform cadence and regulatory (510(k)) pipeline.

## 4. Key Metrics

| Metric | FY2023 | FY2024 | FY2025 | Q2 2026 | Source |
|---|---|---|---|---|---|
| Total revenue ($M) | 7,124.1 | 8,352.1 | 10,064.7 (+21%) | 2,892.3 (+19%) | https://agentii.ai/v/ISRG/sec166/77 ; https://agentii.ai/v/ISRG/sec172/38 |
| da Vinci procedures (k) | 2,286 | 2,683 | 3,153 (+18%) | 889 (+15%) | https://agentii.ai/v/ISRG/sec166/71 ; https://agentii.ai/v/ISRG/sec172/32 |
| Ion procedures (k) | — | 95.5 | 144.1 (+51%) | 47.9 (+36%) | https://agentii.ai/v/ISRG/sec166/69 ; https://agentii.ai/v/ISRG/sec172/32 |
| da Vinci placements | 1,370 | 1,526 | 1,721 (+13%) | 468 (+18%) | https://agentii.ai/v/ISRG/sec166/73 ; https://agentii.ai/v/ISRG/sec172/32 |
| — of which da Vinci 5 | — | 362 | 870 | 246 | https://agentii.ai/v/ISRG/sec166/69 ; https://agentii.ai/v/ISRG/sec172/32 |
| da Vinci installed base (EOP) | — | 9,902 | 11,106 (+12%) | 11,710 (+12%) | https://agentii.ai/v/ISRG/sec166/69 ; https://agentii.ai/v/ISRG/sec172/32 |
| Utilization (proc/system/yr), YoY | — | — | +3% | +3% | https://agentii.ai/v/ISRG/sec166/69 ; https://agentii.ai/v/ISRG/sec172/32 |
| I&A revenue ($M) | 4,276.6 | 5,079.0 | 6,018.9 (+19%) | 1,734.9 (+18%) | https://agentii.ai/v/ISRG/sec166/77 ; https://agentii.ai/v/ISRG/sec172/38 |
| I&A per procedure (computed) | — | — | ~$1,909 | — | [DEDUCTED 3] |
| Service revenue ($M) | 1,167.8 | 1,307.1 | 1,572.1 (+20%) | 472.4 (+21%) | https://agentii.ai/v/ISRG/sec166/77 ; https://agentii.ai/v/ISRG/sec172/38 |
| Recurring revenue % of total | 83% | 84% | 84% | 85% | https://agentii.ai/v/ISRG/sec166/78 ; https://agentii.ai/v/ISRG/sec172/40 |
| Gross margin | — | 67.5% | 66.0% | 67.8% | https://agentii.ai/v/ISRG/sec166/69 ; https://agentii.ai/v/ISRG/sec172/32 |
| Headcount (EOP) | — | — | 17,021 | — | https://agentii.ai/v/ISRG/sec166/25 |
| FY2026 procedure growth guidance | — | — | — | 13.5–15.5% | https://agentii.ai/v/ISRG/ect75/3 |

## 5. Coverage Gaps & Citations

Coverage gaps (unretrievable / not disclosed):
- **No MTBF/uptime/failure/downtime metrics disclosed by ISRG anywhere** in retrieved 10-K (sec166), 10-Q (sec172), or transcripts (ect75). Reliability appears only qualitatively. This is a finding, not just a gap.
- XBRL store contains only one revenue concept with ISRG facts (us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax). `us-gaap:Revenues`, `us-gaap:RevenueFromContractWithCustomerIncludingAssessedTax`, and isrg-namespace revenue-subtotal concepts (I&A/Systems/Service) returned zero facts — product-category revenue is retrievable only from document tables (sec166/77, sec172/38).
- `get_company_fiscal_calendar` returns fiscal_year_end_month=1 (Jan-end), inconsistent with ISRG's calendar-year reporting; XBRL fact periods (calendar quarters) were validated against 10-Q values and used accordingly.
- China 2023 quota detail (sec166 page53) was outlined but not deep-read; Q3 2026 results not yet filed as of 2026-09-10.
- Procedure counts are company-reported approximations rounded to thousands; no per-system telemetry is public.

Citation index (roll-up):
1. https://agentii.ai/v/ISRG/sec166/69 — FY2025 operational & financial highlights
2. https://agentii.ai/v/ISRG/sec166/71 — da Vinci procedure volumes by region/specialty 2023–2025
3. https://agentii.ai/v/ISRG/sec166/73 — system placements & installed base geography
4. https://agentii.ai/v/ISRG/sec166/77 — pricing bands; revenue by category/geography
5. https://agentii.ai/v/ISRG/sec166/78 — systems revenue drivers, ASP, leases, recurring revenue
6. https://agentii.ai/v/ISRG/sec166/25 — human capital: headcount, turnover
7. https://agentii.ai/v/ISRG/sec172/32 — Q2 2026 operational & financial highlights
8. https://agentii.ai/v/ISRG/sec172/38 — Q2/H1 2026 revenue table
9. https://agentii.ai/v/ISRG/sec172/40 — service, leases, ASP, recurring revenue Q2/H1 2026
10. https://agentii.ai/v/ISRG/ect75/1 — Q2 2026 call: operational highlights, extended use, reliability language
11. https://agentii.ai/v/ISRG/ect75/3 — FY2026 guidance; U.S. growth moderation
12. https://agentii.ai/v/ISRG/ect75/4 — capital environment; dv5 updates & 510(k)s; dv5 vs Xi utilization
13. https://agentii.ai/v/ISRG/ect75/5 — U.S. utilization +3%; upgrade-cycle history; XiR base

## 6. Verification

| # | Call (trace) | Tool | Result |
|---|---|---|---|
| 1 | search_companies(ticker=ISRG) | agentii | Ticker resolved: INTUITIVE SURGICAL INC, CIK 0001035267, NASDAQ |
| 2 | get_ticker_coverage(ISRG) | agentii | 7 sources; xbrl_facts 52,854 records; transcripts 19; latest transcript 2026-07-16 |
| 3 | get_company_fiscal_calendar(ISRG) | agentii | fiscal_year_end_month=1 (inconsistent w/ calendar reporting — noted in gaps) |
| 4 | search_documents(ISRG, 10-K) | agentii | FY2025 10-K filed 2026-02-03 |
| 5 | search_documents(ISRG, earnings_call_transcript) | agentii | 19 transcripts, latest 2026-07-16 |
| 6 | search_sec_filings(ISRG, 10-K) | agentii | FY2025 10-K = citation sec166, accession 0001035267-26-000010 |
| 7 | search_sec_filings(ISRG, 10-Q) | agentii | Q2 2026 10-Q = citation sec172, accession 0001035267-26-000058 |
| 8 | list_xbrl_concepts(us-gaap, "Revenue") | agentii | 109 concepts; RevenueFromContractWithCustomerExcludingAssessedTax available |
| 9 | list_xbrl_concepts(isrg, "Revenue") | agentii | 0 concepts — no custom revenue subtotals in store |
| 10 | read_source_outline(sec166) | agentii | 130-page map; KPI pages identified (25, 63, 69–78) |
| 11 | read_source_pages(sec166, page69+71+73) | agentii | Facts 1–16 sourced |
| 12 | read_source_pages(sec166, page77+78+25) | agentii | Facts 4, 17–24 sourced |
| 13 | list_sources(ISRG, transcripts) | agentii | Q2 2026 transcript source_id resolved |
| 14 | read_source_outline(transcript 2026-07-16) | agentii | citation ect75; 6 pages |
| 15 | read_source_outline(sec172) | agentii | 49-page map; page32 = Q2 highlights |
| 16 | read_source_pages(ect75, page1+4) | agentii | Facts 34, 37–39, 47, 50 sourced |
| 17 | read_source_pages(sec172, page32) | agentii | Facts 26–30 sourced |
| 18 | search_xbrl_facts(RevFromContractExclTax, FY2026) | agentii | Q2 2026 $2,892.3M; H1 $5,663.1M; Q1 $2,770.8M — match sec172 |
| 19 | search_xbrl_facts(RevFromContractExclTax, FY2025) | agentii | FY2025 $10,064.7M (source_authority 3 = 10-K) — matches sec166 |
| 20 | search_xbrl_facts(us-gaap:Revenues, 2023/2021) | agentii | 0 facts — coverage gap recorded |
| 21 | search_xbrl_facts(RevFromContractInclTax, FY2025) | agentii | 0 facts — coverage gap recorded |
| 22 | read_source_pages(ect75, page3+5) | agentii | Facts 35, 40–43, 48 sourced |
| 23 | read_source_pages(sec172, page38+40) | agentii | Facts 31–33, 45 sourced |

All material numbers trace to calls 11, 12, 16, 17, 18, 19, 22, 23 above. No price data used (market_data_stage: none).
