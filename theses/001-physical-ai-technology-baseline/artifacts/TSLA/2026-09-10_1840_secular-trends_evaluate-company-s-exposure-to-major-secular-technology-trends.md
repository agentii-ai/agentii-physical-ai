---
artifact_id: "001-TSLA-secular-trends-evaluate-company-s-exposure-to-major-secular-technology-trends-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: TSLA
skill: secular-trends
mode: evaluate-company-s-exposure-to-major-secular-technology-trends
affix: tech-trends
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "e6b41dbb2426"
as_of: 2026-09-10
entity_claims:
  - "TSLA_CAPEX_2026: capex >$25B in 2026, driven by AI initiatives (compute, data centers, AI-enabled fleet)"
  - "TSLA_OPTIMUS_COMMERCIAL: zero commercial Bots revenue as of FY2025 10-K; Optimus production expected to start late 2026"
  - "TSLA_ROBOTAXI: robotaxi live in 7 US metros; 380,000+ unsupervised miles, zero notable incidents"
  - "TSLA_FSD_SUBS: 1.48M active FSD subscriptions as of Q2 2026"
citations: []
pillars_addressed: [PIL-1, PIL-3, PIL-4]
claim_state: pinned
key_metrics:
  revenue_fy2025_usd_m: 94827
  revenue_q2_2026_usd_m: 28236
  rd_expense_fy2025_usd_m: 6411
  rd_expense_q2_2026_usd_m: 2371
  capex_fy2025_usd_m: 8530
  capex_h1_2026_usd_m: 8282
  capex_2026_guidance_usd_b: ">25"
  active_fsd_subscriptions_q2_2026_m: 1.48
  cumulative_fsd_miles_b: "~17.2"
  unsupervised_robotaxi_miles: "380,000+"
  ai_training_compute_mw: "~250 (Cortex 1+2; ~400 planned Dec-2026)"
conclusions:
  - "TSLA has direct, disclosed, and rapidly scaling exposure to the AI, embodied-AI, data-flywheel, AI-compute, and AI-energy secular trends; robotics is the only trend where commercial revenue is still zero."
  - "The company's own filings calibrate Optimus expectations down: 'nascent industry that has yet to develop commercially' and a flat initial S-curve; all unit-volume claims are promotional [VIEW]."
  - "Reliability, not model capability, is the disclosed binding constraint on robotaxi scaling ('March of 9s'); no humanoid MTBF disclosure exists because no commercial fleet exists."
facts_count: 24
deducted_count: 4
views_count: 3
citation_count: 20
---

# TSLA — Evaluate Company's Exposure to Major Secular Technology Trends

**Mode**: evaluate-company-s-exposure-to-major-secular-technology-trends
**Chain**: TSLA × secular-trends — artifact 1 of 3
**Thesis pillars served**: PIL-1 (embodied AI is data-bound), PIL-3 (manipulation reliability gates deployment), PIL-4 (GPT-3.5 moment 2027-Q4–2028)

## Executive Summary

Tesla's own filings describe its purpose as "bringing artificial intelligence into the real world" through FSD (Supervised), Robotaxi, and "AI robots (including Optimus)" ([FACT] https://agentii.ai/v/TSLA/sec253/36). Exposure to the major secular technology trends is direct, disclosed, and accelerating: FY2025 revenues of $94.83B ([FACT] https://agentii.ai/v/TSLA/sec253/36) with Q2 2026 revenue of $28,236M, +26% YoY ([FACT] https://agentii.ai/v/TSLA/sec258/7); R&D at $6,411M in FY2025, +41% YoY, 7% of revenue ([FACT] https://agentii.ai/v/TSLA/sec253/44) rising to $2,371M in Q2 2026 ([FACT] https://agentii.ai/v/TSLA/sec258/30); and 2026 capex guided "in excess of $25 billion... driven by our AI initiatives, including investments in compute infrastructure and data centers" ([FACT] https://agentii.ai/v/TSLA/sec259/30). The one trend where exposure is strategic but revenue is zero is humanoid robotics: the FY2025 10-K states Bots "is in a nascent industry that has yet to develop commercially" ([FACT] https://agentii.ai/v/TSLA/sec253/20). Management explicitly calibrates the Optimus ramp as a "flat and long" initial S-curve ([VIEW] https://agentii.ai/v/TSLA/ect61/1), consistent with PIL-4's late-2027/2028 inflection timing. This chain treats all humanoid unit-count and capability statements as promotional claims triangulated against filings.

## Core Analysis: Trend Exposure Matrix

| Trend | Exposure | Evidence (as filed) | Pillar |
|---|---|---|---|
| AI — autonomous driving (FSD, Robotaxi, Cybercab) | HIGH — monetizing | 1.48M active FSD subscriptions, +56% YoY ([FACT] https://agentii.ai/v/TSLA/sec258/8); Robotaxi live in 7 US metros ([FACT] https://agentii.ai/v/TSLA/ect61/2); cumulative FSD (Supervised) miles ~17.2B ([FACT] https://agentii.ai/v/TSLA/sec258/11) | PIL-1, PIL-3 |
| AI — embodied robotics (Optimus) | HIGH strategically, ZERO commercial | "We have yet to commercialize Bots" ([FACT] https://agentii.ai/v/TSLA/sec253/21); Fremont first-gen lines installed, "production later this year" ([FACT] https://agentii.ai/v/TSLA/sec258/6) | PIL-3, PIL-4 |
| Data flywheel — real-world AI data | HIGH — core strategic asset | "capitalizing on our strengths in real-world AI data to advance the development of Optimus" ([FACT] https://agentii.ai/v/TSLA/sec253/37) | PIL-1 |
| AI compute infrastructure | HIGH — doubling | Cortex 1 >90 MW + Cortex 2 >115 MW ([FACT] https://agentii.ai/v/TSLA/sec258/10); training-capacity ramp ~250 MW Jun-2026 → ~400 MW planned Dec-2026 ([FACT] https://agentii.ai/v/TSLA/sec258/10); AI infrastructure PP&E $10,823M vs $6,816M six months earlier ([FACT] https://agentii.ai/v/TSLA/sec259/18) | PIL-1 (counterfactual check) |
| AI silicon — vertical integration | HIGH — emerging | $1.95B AI hardware company acquisition in Q2 2026 ([FACT] https://agentii.ai/v/TSLA/sec259/17); Austin semiconductor fab under construction ([FACT] https://agentii.ai/v/TSLA/sec258/11); AI5 taped out ([FACT] https://agentii.ai/v/TSLA/ect60/1) | PIL-1 |
| Energy for AI (storage powering data centers) | MEDIUM-HIGH — growing | 13.5 GWh storage deployed Q2 2026 ([FACT] https://agentii.ai/v/TSLA/ect61/2); xAI purchased $430M of Megapacks in FY2025 ([FACT] https://agentii.ai/v/TSLA/sec253/97) | PIL-1 (indirect) |

### Trend 1 — AI / Autonomy: the monetizing core

The Robotaxi service has operated since its June 2025 launch ([FACT] https://agentii.ai/v/TSLA/sec253/20) and by Q2 2026 had driven "more than 380,000 miles of unsupervised robotaxi... zero notable incidents" across six cities and two states ([FACT] https://agentii.ai/v/TSLA/ect61/3). FSD is the disclosed primary demand driver: ~55% of North American Q2 deliveries had FSD subscription enabled at delivery ([FACT] https://agentii.ai/v/TSLA/ect61/2), and FSD-related deferred revenue stands at $4.05B as of June 30, 2026 ([FACT] https://agentii.ai/v/TSLA/sec259/10). FSD/robotaxi is the clearest "AI with a revenue line" at TSLA.

### Trend 2 — Embodied AI: exposure without revenue

Optimus exposure is disclosed and deliberate but pre-revenue. The FY2025 10-K (filed January 2026) risk factors state Bots development "requires significant cash investments" and "we have yet to commercialize Bots" ([FACT] https://agentii.ai/v/TSLA/sec253/21). The 2025 CEO Performance Award embeds "1 million bots delivered" and "1 million Robotaxis in commercial operation" among its 12 operational milestones, gated by market-cap milestones of $2.0T–$8.5T ([FACT] https://agentii.ai/v/TSLA/sec253/86) — a compensation target, not a forecast [VIEW]. The Q2 2026 deck states Fremont's first-generation Optimus lines "will be used in our Optimus Academy for training data collection" ([FACT] https://agentii.ai/v/TSLA/sec258/9) — i.e., even the first builds are for data, not deployment [DEDUCTED]. Management: "the initial portion of the S-curve will be quite flat and long" ([VIEW] https://agentii.ai/v/TSLA/ect61/1). PIL-4 timing is corroborated by TSLA's own disclosures.

### Trend 3 — Data flywheel

TSLA's unique disclosed asset is the real-world data flywheel: ~17.2B cumulative FSD (Supervised) miles, of which ~16.0B on v12+ stacks ([FACT] https://agentii.ai/v/TSLA/sec258/11). The same data loop is the disclosed basis for Optimus: "a broad fleet of humans giving us data from all of the workers at our factory" plus a dedicated data-collection team plus Internet video, then a robot-practice RL loop ("Optimus Academy") ([FACT] https://agentii.ai/v/TSLA/ect61/3). This is the PIL-1 embodied-data mechanism, disclosed in the company's own words.

### Trend 4 — AI compute and silicon

Compute exposure is the fastest-moving line: onsite Texas training compute "more than doubled... during the first half of 2026" ([FACT] https://agentii.ai/v/TSLA/sec258/10); Cortex 2 "supports the development of both vehicle and humanoid robot autonomy software" ([FACT] https://agentii.ai/v/TSLA/sec258/10). Capex more than doubled sequentially in Q2 2026 to $5,789M ([FACT] https://agentii.ai/v/TSLA/sec258/7; H1 total $8,282M [FACT] https://agentii.ai/v/TSLA/sec259/28), and management cites Terafab — in-house logic/memory/packaging fabs — as necessary because "we simply won't have enough AI chips" to scale Optimus ([VIEW] https://agentii.ai/v/TSLA/ect61/1). Note for PIL-1: TSLA's ~250 MW of training compute ([FACT] https://agentii.ai/v/TSLA/sec258/10) is being built to run a data-flywheel training loop; the company is compute-hungry but data-differentiated [DEDUCTED].

### Validation

- **Quantitative support**: revenue, R&D, capex, deferred revenue, subscriber counts, and compute capacity all retrieved from filings/decks (XBRL cross-check: FY2025 Revenues $94,827M and Q2-2026 Revenues $28,236M match filing text exactly; get_company_financials confirms R&D and capex values).
- **Source diversity**: 10-K (sec253), 10-Q (sec259), 8-K deck (sec258), two earnings transcripts (ect60, ect61), XBRL facts.
- **Temporal coverage**: FY2023–FY2025 financials in 10-K tables; quarterly metrics FY2024 Q1–FY2026 Q2 via get_company_financials; management commentary Apr 2026 and Jul 2026.

## Coverage Gaps & Citations

**Coverage gaps** (unretrievable or not attempted within budget):
1. No Optimus unit-cost, per-unit BOM, or unit-volume guidance exists in any retrieved filing — unit-cost triangulation is deferred to TSLA × unit-economics.
2. No humanoid MTBF/reliability disclosure exists because no commercial humanoid fleet exists; PIL-3 is currently assessed via the robotaxi "March of 9s" analogue only.
3. XBRL `DeferredRevenue` concept returns empty for TSLA; FSD deferred revenue taken from 10-Q Note 1 text (sec259/10).
4. `search_sec_filings` source shows 0 records for TSLA in coverage metadata; Layer 1 discovery used `search_documents`/`list_sources` instead.
5. Q3 FY2026 transcript (2025-10-22) and Q1 FY2027 8-K deck not deep-read (rate-limit budget); timeline mid-points inferred from Q1/Q2 FY2027 calls.
6. FSD cumulative-miles chart values post-Jun-2024 are flagged by the extraction layer as visually estimated — treat ~17.2B as approximate.
7. No price data used (market_data_stage: none). Market cap $1.43T appears only as registry metadata from search_companies (not a market-data source).

**Citations (roll-up index — inline /v/ links are primary):**
1. sec253/36 — FY2025 highlights, revenues $94.83B, capex $8.53B (10-K FY2025)
2. sec253/20 — Bots "nascent industry that has yet to develop commercially" (10-K risk factor)
3. sec253/21 — "We have yet to commercialize Bots" (10-K risk factor)
4. sec253/37 — real-world AI data → Optimus (10-K MD&A)
5. sec253/44 — R&D $6,411M, +41% (10-K)
6. sec253/86 — 2025 CEO Performance Award milestones (bots/robotaxis/FSD subs)
7. sec253/97 — xAI related-party $430M Megapack revenue; $2B xAI investment
8. sec258/6 — Q2 highlights, Fremont Optimus construction (8-K deck)
9. sec258/7 — Q2 financial summary, capex $5,789M (8-K deck)
10. sec258/8 — 1.48M active FSD subscriptions (8-K deck)
11. sec258/9 — Optimus Academy; robotics capacity "Construction" (8-K deck)
12. sec258/10 — Cortex 1/2 MW, training ramp table (8-K deck)
13. sec258/11 — FSD cumulative miles ~17.2B; Austin fab (8-K deck)
14. sec259/10 — FSD deferred revenue $4.05B (10-Q)
15. sec259/17 — $1.95B AI hardware acquisition (10-Q)
16. sec259/18 — AI infrastructure PP&E $10,823M (10-Q)
17. sec259/28 — H1-2026 capex $8.28B, Q2 revenue (10-Q)
18. sec259/30 — capex >$25B guidance, Cortex expansion (10-Q)
19. ect61/1-3 — Optimus S-curve, no-supply-chain, 380K unsupervised miles, Optimus data flywheel (Q2 FY2027 call)
20. ect60/1 — AI5 tape-out; Optimus production timing; Fremont starter production (Q1 FY2027 call)

## Verification (call trace)

| # | Tool | Target | Result |
|---|---|---|---|
| 1 | search_companies | TSLA | Tesla, Inc., CIK 0001318605, market cap registry metadata $1.43T |
| 2 | get_ticker_coverage | TSLA | xbrl_facts 63,523; transcripts 19; sec_filings 0 |
| 3 | get_company_fiscal_calendar | TSLA | FY end Jan-31; latest closed quarter FY2027 Q2 (ends 2026-07-31) |
| 4 | search_documents | 10-K / transcripts / keywords | 5 10-Ks; 19 transcripts; keyword filter non-discriminating |
| 5 | list_sources | TSLA | 92 sources; source_ids + accessions resolved |
| 6 | read_source_outline | ect61 (Q2-26 call), sec253 (10-K), sec258 (8-K), sec259 (10-Q), ect60 (Q1-26 call) | citation_ids + page maps |
| 7 | read_source_pages | ect61/1-6; sec253/20,21,36,37,38,44,45,46,86,97; sec258/6-13; sec259/10,17,18,28,29,30; ect60/1,3,5 | page content retrieved |
| 8 | list_xbrl_concepts | PaymentsToAcquire*, R&D, DeferredRevenue | concept names confirmed |
| 9 | search_xbrl_facts | Revenues FY2025 FY / FY2026 Q2; R&D FY2026 Q2; PP&E capex FY2026 | $94,827M / $28,236M / $2,371M / $8,282M H1 |
| 10 | search_keyword_in_source | sec253 "Optimus" | 7 pages incl. risk factors 20-21 |
| 11 | get_company_financials | TSLA FY2026 | 12-quarter metrics; R&D trajectory confirmed |
| 12 | Bash (date, mkdir) | timestamp | 2026-09-10_1840 |

All material numbers above trace to retrieval calls listed in this table. No number is reproduced from memory.
