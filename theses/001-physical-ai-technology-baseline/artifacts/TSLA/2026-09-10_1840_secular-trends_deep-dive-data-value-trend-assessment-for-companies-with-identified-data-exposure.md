---
artifact_id: "001-TSLA-secular-trends-deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: TSLA
skill: secular-trends
mode: deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure
affix: tech-trends
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "e6b41dbb2426"
as_of: 2026-09-10
entity_claims:
  - "TSLA_FSD_DATA: ~17.2B cumulative FSD (Supervised) miles, ~16.0B on v12+ stacks (company deck, chart-approximate)"
  - "TSLA_FSD_MONETIZATION: 1.48M active FSD subscriptions; $4.05B FSD-related deferred revenue; $962M recognized next 12 months"
  - "TSLA_OPTIMUS_DATA: Optimus data loop = factory-human observation + dedicated demo team + internet video + Optimus Academy RL"
  - "TSLA_CYBERCAB_DATA_GATE: Cybercab chassis-specific data accumulation required before fleet scaling"
citations: []
pillars_addressed: [PIL-1, PIL-3, PIL-4]
claim_state: pinned
key_metrics:
  cumulative_fsd_miles_b: "~17.2 (~16.0 on v12+)"
  cumulative_paid_robotaxi_miles_m: "~2.5"
  unsupervised_robotaxi_miles: "380,000+"
  active_fsd_subscriptions_m: 1.48
  fsd_attach_rate_na_pct: ">55"
  fsd_deferred_revenue_jun2026_usd_b: 4.05
  fsd_deferred_12mo_recognition_usd_m: 962
  fsd_deferred_recognized_h1_2026_usd_m: 468
conclusions:
  - "TSLA operates the largest disclosed real-world driving-data asset in its own filings: ~17.2B cumulative FSD miles, monetized through 1.48M subscriptions and a $4.05B deferred-revenue balance — the data flywheel is real and revenue-linked."
  - "The Optimus data strategy is explicitly a fleet-data play adapted to embodied tasks (factory humans, dedicated demos, Optimus Academy RL), but the company discloses no embodied-data volumes — the PIL-1 3-orders-of-magnitude test cannot be measured from TSLA disclosures alone."
  - "Data accumulation, not just validation, gates deployment: Cybercab needs chassis-specific miles before scaling, and AI3 hardware's memory bandwidth caps unsupervised capability on the installed fleet — evidence that data AND its compute substrate both bind."
  - "No disclosure monetizes data externally (no data licensing revenue line); data value is internal flywheel value only."
facts_count: 24
deducted_count: 5
views_count: 2
citation_count: 20
---

# TSLA — Deep Dive: Data Value Trend Assessment (identified data exposure)

**Mode**: deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure
**Chain**: TSLA × secular-trends — artifact 3 of 3

## Executive Summary

TSLA's data exposure is the thesis's PIL-1 case study. The company discloses a real-world AI data asset of ~17.2B cumulative FSD (Supervised) miles, of which ~16.0B on v12-and-beyond stacks ([FACT] https://agentii.ai/v/TSLA/sec258/11), grown from ~0.1B v12+ miles in Jun-2023 ([FACT] https://agentii.ai/v/TSLA/sec258/11). That asset is directly monetized: 1.48M active FSD subscriptions (+56% YoY) ([FACT] https://agentii.ai/v/TSLA/sec258/8) and $4.05B of FSD-related deferred revenue ([FACT] https://agentii.ai/v/TSLA/sec259/10). For embodied AI, TSLA discloses the same flywheel logic transplanted to robots — "just like FSD, we have access to a broad fleet of humans giving us data from all of the workers at our factory," plus a dedicated high-quality demonstration team, internet video, and an "Optimus Academy" reinforcement-learning loop ([FACT] https://agentii.ai/v/TSLA/ect61/3) — and the first Optimus production units are earmarked for training-data collection rather than sale ([FACT] https://agentii.ai/v/TSLA/sec258/9). The catch for PIL-1: TSLA discloses zero embodied-data volumes (no hours, no episodes, no tokens), so the falsifier's 3-orders-of-magnitude gap cannot be directly measured here; and two retrieved disclosures show data-substrate constraints biting (Cybercab chassis-specific miles [FACT] https://agentii.ai/v/TSLA/ect61/5; AI3 memory bandwidth [FACT] https://agentii.ai/v/TSLA/ect60/3).

## Core Analysis

### 1. The disclosed data asset: fleet-scale driving data

The Q2 2026 deck publishes a cumulative FSD-miles ledger: ~0.9B total in Jun-2023 → ~17.2B in Jun-2026, with the v12+ component compounding ~3x per year over the last two years (~5.0B Sep-2024 → ~11.2B Jun-2025 → ~17.2B Jun-2026; extraction-flagged approximate) ([FACT] https://agentii.ai/v/TSLA/sec258/11). Layered on top: ~2.5M cumulative paid robotaxi miles by Jun-2026 ([FACT] https://agentii.ai/v/TSLA/sec258/12), 380,000+ unsupervised miles ([FACT] https://agentii.ai/v/TSLA/ect61/3), and robotaxi miles growing "more than 10% a week" ([FACT] https://agentii.ai/v/TSLA/ect61/1). Region-expansion data is explicitly additive: EU approvals brought >50M km of additional FSD data in new countries ([FACT] https://agentii.ai/v/TSLA/sec258/12), and Ashok Elluswamy states the same architecture + local data is the expansion recipe ([FACT] https://agentii.ai/v/TSLA/ect60/3). The 10-K frames the strategic position: "capitalizing on our strengths in real-world AI data to advance the development of Optimus" ([FACT] https://agentii.ai/v/TSLA/sec253/37), repeated in the Q2 10-Q ([FACT] https://agentii.ai/v/TSLA/sec259/29).

### 2. Data monetization mechanics

FSD monetization disclosures: active subscriptions 1.48M, of which 55% upfront purchases and 45% recurring subscriptions; NA attach >55% of Q2 deliveries; management expects "the bulk of the growth in FSD monetization... from subscriptions as we removed the purchase option in most markets" ([FACT] https://agentii.ai/v/TSLA/ect61/2). Accounting for the data-product value: deferred revenue tied to "internet connectivity, access to our Full Self-Driving (FSD) (Supervised) features and their ongoing maintenance, free Supercharging programs and over-the-air software updates" is $4.05B at Jun-30-2026 vs $3.87B at Dec-31-2025 ([FACT] https://agentii.ai/v/TSLA/sec259/10); $962M of it is expected to be recognized in the next 12 months, and $468M was recognized from prior balances in H1 2026 ([FACT] https://agentii.ai/v/TSLA/sec259/10). The company also added a user-facing "Self-Driving Stats" dashboard, making the data loop social and viral ([FACT] https://agentii.ai/v/TSLA/sec258/11). There is no disclosed external data-licensing revenue line — data value is internal flywheel value, monetized through software features and services ([DEDUCTED] from revenue-by-source tables, https://agentii.ai/v/TSLA/sec259/10).

### 3. The embodied-data strategy for Optimus (PIL-1 mechanism)

The most thesis-relevant disclosure in the corpus is the Optimus data-collection stack ([FACT] https://agentii.ai/v/TSLA/ect61/3):
1. **Human-observation data at fleet scale** — "a broad fleet of humans giving us data from all of the workers at our factory"; Gen 3's human form factor is explicitly designed so "having the human form factor and function allows us to learn from humans" ([FACT] https://agentii.ai/v/TSLA/ect61/3).
2. **Small high-quality demonstration set** — "a dedicated data collection team who can provide a relatively small amount, but of very high-quality demonstrations to do the post-training" ([FACT] https://agentii.ai/v/TSLA/ect61/3).
3. **Internet pretraining** — "training we can do off of the entire Internet of data" ([FACT] https://agentii.ai/v/TSLA/ect61/3).
4. **Robot-practice RL loop** — the "Optimus Academy" where "the data from the bots experiencing the task themselves" closes form-factor gaps and feeds a success/failure reinforcement loop ([FACT] https://agentii.ai/v/TSLA/ect61/3).

The deployment sequencing makes the data-first orientation explicit: "The initial Optimus builds will be used in our Optimus Academy for training data collection and further functionality development" ([FACT] https://agentii.ai/v/TSLA/sec258/9). First units are data-collection instruments, not revenue units [DEDUCTED] — consistent with PIL-4's late-2027 deployment timing.

**PIL-1 measurement caveat**: TSLA discloses no embodied-data quantities (hours of demonstration, episodes, tokens). The wrong_if metric (embodied-data gap >3 orders of magnitude vs LLM pretrain) cannot be computed from TSLA sources; this artifact contributes the mechanism (fleet-human + small-demo + RL) but not the magnitude [DEDUCTED]. The compute side, by contrast, is quantified precisely (~250 MW → ~400 MW planned) ([FACT] https://agentii.ai/v/TSLA/sec258/10) — TSLA's disclosures are compute-rich and data-poor in units.

### 4. Data-substrate constraints: where data value hits hardware walls

Two disclosures show the flywheel is bounded by substrate, not just by quantity of examples:
- **Cybercab chassis data**: "we need to accumulate driving data that is specific to the Cybercab before we can put a lot of them on the road" — new-platform data accumulation gates fleet scaling even though the software stack is shared ([FACT] https://agentii.ai/v/TSLA/ect61/5).
- **AI3 memory bandwidth**: Hardware 3 "has only 1/8 of the memory bandwidth of hardware 4... memory bandwidth is one of the key elements needed for unsupervised FSD" ([FACT] https://agentii.ai/v/TSLA/ect60/3); the fleet's older data-producing vehicles cannot run unsupervised FSD, requiring a hardware-upgrade program. The data fleet itself needs upgrading to stay valuable [DEDUCTED].

### 5. Adjacent data-value trends

- **Energy/power telemetry for AI**: management positions Megapack as the solution for AI data-center power smoothing ("during a training run, the power consumption can drop by 70% for 100 milliseconds") ([VIEW] https://agentii.ai/v/TSLA/ect61/6); xAI bought $430M of Megapacks in FY2025 ([FACT] https://agentii.ai/v/TSLA/sec253/97).
- **Connectivity data infrastructure**: Starlink integration into Cybercab/all vehicles is justified by data-availability needs ("we can't have robotaxis getting stuck in these... lack of cellular connectivity") ([VIEW] https://agentii.ai/v/TSLA/ect61/4).
- **LLM-adjacent data**: Grok in-vehicle and as Optimus orchestrator ties the embodied loop to an external model provider in which TSLA invested ~$2B ([FACT] https://agentii.ai/v/TSLA/sec253/97).

### 6. Data value vs. thesis pillars

- **PIL-1**: TSLA is the strongest single-company exhibit that fleet data is the strategic moat (10-K language, Optimus Academy design, Cybercab data gate). But its compute disclosures (25x ramp in 3 years, $10.8B AI-infrastructure PP&E, Terafab chip-supply rationale) show the same company treats compute as a co-binding constraint — the honest reading is "data-differentiated, compute-intensive," not purely data-bound [DEDUCTED].
- **PIL-3**: the disclosed reliability gate ("March of 9s") sits on top of the data asset; more data does not automatically buy deployment — validation and reliability do [DEDUCTED].
- **PIL-4**: data-loop-first Optimus sequencing (units → Optimus Academy, not customers) is consistent with no commercial humanoid fleet before 2027-Q4 [DEDUCTED].

## Coverage Gaps & Citations

**Coverage gaps:**
1. No embodied-data volumes (demonstration hours, episodes, teleoperation minutes) disclosed anywhere in the corpus — the PIL-1 magnitude test requires industry-technical sources beyond TSLA filings.
2. No per-mile or per-subscription unit economics disclosed for FSD (no churn, no MRR, no per-unit cost of data collection).
3. FSD cumulative-miles chart values post-Jun-2024 are extraction-flagged as visually estimated (~ approximations).
4. XBRL `DeferredRevenue` concept returns empty for TSLA; deferred-revenue figures taken from 10-Q Note 1 text.
5. No disclosure of what fraction of the ~17.2B miles is usable training data vs. noisy fleet logs; no data-retention or privacy-cap quantification retrieved.

**Citations (roll-up index):**
1. sec253/37 — "real-world AI data to advance... Optimus" (10-K)
2. sec253/97 — xAI $2B investment; $430M Megapack revenue (10-K)
3. sec258/8 — 1.48M active FSD subscriptions, +56% (8-K deck)
4. sec258/9 — initial Optimus builds for Optimus Academy data collection (8-K deck)
5. sec258/10 — training compute 250→400 MW (8-K deck)
6. sec258/11 — FSD cumulative miles ledger; Self-Driving Stats (8-K deck)
7. sec258/12 — paid robotaxi miles ~2.5M; EU 31M miles (8-K deck)
8. sec259/10 — FSD deferred revenue $4.05B; $962M 12-mo; $468M recognized (10-Q)
9. sec259/29 — real-world AI data, Optimus large-scale production prep (10-Q)
10. ect60/1 — robotaxi validation limiting factor (Q1 FY2027 call)
11. ect60/3 — AI3 1/8 memory bandwidth; local-data expansion recipe (Q1 FY2027 call)
12. ect60/5 — robotaxi operational (non-safety) failure modes (Q1 FY2027 call)
13. ect61/1 — robotaxi >10%/week miles growth (Q2 FY2027 call)
14. ect61/2 — FSD monetization mix, 55/45, attach >55% (Q2 FY2027 call)
15. ect61/3 — Optimus four-layer data strategy; 380K unsupervised miles (Q2 FY2027 call)
16. ect61/4 — Starlink connectivity rationale; March of 9s (Q2 FY2027 call)
17. ect61/5 — Cybercab chassis-specific data accumulation gate (Q2 FY2027 call)
18. ect61/6 — AI training power 70%/100ms claim; Megapack demand (Q2 FY2027 call)
19. search_xbrl_facts — Revenues FY2025 FY ($94,827M), Q2-2026 ($28,236M) cross-checks
20. get_company_financials — 12-quarter revenue/R&D series

## Verification (call trace)

| # | Tool | Target | Result |
|---|---|---|---|
| 1 | search_companies | TSLA | entity resolution |
| 2 | get_ticker_coverage | TSLA | source inventory |
| 3 | get_company_fiscal_calendar | TSLA | fiscal alignment |
| 4 | search_documents | TSLA forms/transcripts | Layer 1 discovery |
| 5 | list_sources | TSLA | 92 sources, ids resolved |
| 6 | read_source_outline | sec253, sec258, sec259, ect60, ect61 | page maps |
| 7 | read_source_pages | sec253/37,97; sec258/8,9,10,11,12; sec259/10,29; ect60/1,3,5; ect61/1-6 | content |
| 8 | list_xbrl_concepts | revenue/capex/deferred concepts | confirmed |
| 9 | search_xbrl_facts | Revenues FY2025/FY2026 Q2; R&D; capex | cross-checks |
| 10 | search_keyword_in_source | sec253 "Optimus" | page map |
| 11 | get_company_financials | TSLA | 12-quarter series |
| 12 | Bash | timestamp/mkdir | 2026-09-10_1840 |

Every number above was retrieved in this run; none are from memory or market price data (market_data_stage: none).
