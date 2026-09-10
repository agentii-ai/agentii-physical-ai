---
artifact_id: "001-NVDA-secular-trends-deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: NVDA
skill: secular-trends
mode: deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure
affix: tech-trends
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "e6b41dbb2426"
as_of: 2026-09-10
entity_claims:
  - entity: NVDA
    metric: datacenter_revenue_growth_yoy
    value: 92
    unit: pct
    period: 2027Q1
    source: "10-Q:page21"
    retrieved_at: 2026-09-10
  - entity: NVDA
    metric: datacenter_revenue_growth_yoy
    value: 68
    unit: pct
    period: FY2026
    source: "10-K:page37"
    retrieved_at: 2026-09-10
  - entity: NVDA
    metric: r_and_d_expense_growth_yoy
    value: 58.5
    unit: pct
    period: 2027Q1
    source: "XBRL:us-gaap:ResearchAndDevelopmentExpense (10-Q)"
    retrieved_at: 2026-09-10
  - entity: NVDA
    metric: robotics_and_simulation_revenue_share_of_total_pct
    value: 7.8
    unit: pct
    period: 2027Q1
    source: "10-Q:page21"
    retrieved_at: 2026-09-10
citations:
  - "agentii.ai/v/NVDA/sec169/4"
  - "agentii.ai/v/NVDA/sec169/36"
  - "agentii.ai/v/NVDA/sec169/37"
  - "agentii.ai/v/NVDA/sec169/55"
  - "agentii.ai/v/NVDA/sec173/21"
  - "agentii.ai/v/NVDA/sec173/25"
  - "agentii.ai/v/NVDA/ect81/1"
  - "agentii.ai/v/NVDA/ect81/5"
pillars_addressed: [PIL-1, PIL-3, PIL-4]
claim_state: pinned
key_metrics:
  dc_compute_q1fy2027_usd_b: 60
  dc_networking_q1fy2027_usd_b: 15
  blackwell_rubin_revenue_visibility_2025_2027_usd_t: 1
  ai_infrastructure_spend_decade_end_usd_t: 3-4
  vera_cpu_tam_usd_b: 200
  gross_margin_q1fy2027_pct: 74.9
  fcf_q1fy2027_usd_b: 49
  q2fy2027_revenue_guide_usd_b: 91
conclusions:
  - "AI exposure is total and still inflecting: inference/agentic demand (not just training) now drives revenue, with data-center computing +77% YoY and networking nearly tripling in Q1 FY2027."
  - "NVDA's own disclosures show the binding constraints are power/energy and capital, not data — supporting its role as the compute-boundness counterfactual for PIL-1."
  - "Compute-side readiness for a physical-AI inflection (PIL-4) is concrete (VeraRubin ships Q3 2026; robotics on CUDA/edge platforms), but no humanoid deployment counts are disclosed — the PIL-4 falsifier remains untestable from NVDA sources."
facts_count: 28
deducted_count: 2
views_count: 4
citation_count: 9
---

# NVDA — Deep Dive: AI Trend Assessment (Identified AI Exposure)

**Mode:** deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure
**Thesis:** 001-physical-ai-technology-baseline — NVDA as compute-boundness counterfactual.
**Source set:** FY2026 10-K (sec169), FY2027 Q1 10-Q (sec173), Q1 FY2027 earnings call (ect81, 2026-05-20), XBRL.

## Executive Summary

NVDA's AI exposure is not only dominant — it is still accelerating and broadening from training to inference. Q1 FY2027 revenue was $81.6B (+85% YoY), with Data Center $75.2B (+92%) (https://agentii.ai/v/NVDA/sec173/21). Data-center computing was $60B (+77% YoY) while networking nearly tripled to $15B (https://agentii.ai/v/NVDA/ect81/1). Management quantifies visibility of $1T in Blackwell-and-Rubin revenue over 2025–2027 and frames AI infrastructure spending reaching $3–4T annually by decade-end (https://agentii.ai/v/NVDA/ect81/1). The AI trend is expanding into two adjacent platforms: agentic-AI CPUs (Vera, a new $200B TAM) and physical AI at the edge (robotics, AV, AI-RAN). Meanwhile the binding constraints management names are energy and capital, not data (https://agentii.ai/v/NVDA/sec169/36). NVDA therefore stands as the thesis's compute-boundness counterfactual: the LLM/data-center regime is compute- and energy-bound; the data-boundness claim (PIL-1) applies specifically to embodied AI, where NVDA's own robotics disclosures are qualitative only.

## 1. AI Demand Structure: Training → Inference → Agentic

**[FACT]** "Agentic AI has arrived. AI can now do productive and valuable work. Tokens are now profitable" — Jensen Huang, Q1 FY2027 close (https://agentii.ai/v/NVDA/ect81/5). [FACT] Mainstream AI has transitioned "from 1 shot inference to reasoning and to now agentic" since ChatGPT (https://agentii.ai/v/NVDA/ect81/1).

**[FACT]** Q1 FY2027 data-center computing revenue was $60B (+77% YoY) and data-center networking was $15B, "nearly tripled year over year" (https://agentii.ai/v/NVDA/ect81/1). [DEDUCTED] Networking growth (~3x) outpacing compute growth (+77%) is the signature of inference/agentic scale-out — inference fabrics consume more interconnect per token than training clusters, which corroborates the demand mix shift.

**[FACT]** Blackwell Ultra delivered a 2.7x increase in throughput and a 60% reduction in cost per token on GB300 versus six months prior, sweeping every MLPerf inference benchmark (https://agentii.ai/v/NVDA/ect81/1). [FACT] The price of renting an H100 rose 20% year-to-date, and A100 cloud pricing rose nearly 15% (https://agentii.ai/v/NVDA/ect81/1). [VIEW] Rising rental prices for installed GPUs beyond their depreciable life indicates the residual-value/resale market is monetizing inference demand — a structural support for AI infrastructure spending.

## 2. Platform Cadence and Revenue Visibility

**[FACT]** Product cadence is now annual: Blackwell (majority of Data Center revenue in FY2026 and Q1 FY2027) → Blackwell Ultra/GB300 (shipping Q2 FY2026) → Rubin (https://agentii.ai/v/NVDA/sec169/36) (https://agentii.ai/v/NVDA/sec173/23). [FACT] VeraRubin production shipments commence in the second half of calendar 2026, starting Q3, with demand "already planned," purchase orders in hand, and "almost all of our major customers ready to go" (https://agentii.ai/v/NVDA/ect81/1) (https://agentii.ai/v/NVDA/ect81/5). [FACT] VeraRubin is positioned to deliver up to 35x higher inference throughput and up to 10x greater AI-factory revenue than Blackwell (https://agentii.ai/v/NVDA/ect81/1).

**[FACT]** Management claims "full confidence in $1 trillion in Blackwell and Rubin revenue we foresee from 2025 through calendar 2027" (https://agentii.ai/v/NVDA/ect81/1). [FACT] Vera (agentic-AI CPU) "opens a brand new $200 billion TAM," with "visibility to nearly $20 billion in total CPU revenue this year" (https://agentii.ai/v/NVDA/ect81/1). [VIEW] These are management forward statements, not orders — but the $119B of manufacturing/supply/capacity commitments as of Apr 26, 2026 ($95B payable in the remainder of FY2027) is an audited, balance-sheet-grade demand signal (https://agentii.ai/v/NVDA/sec173/16).

**[FACT]** Ecosystem demand breadth: partner data centers exceeding 10MW nearly doubled in one year to over 80 sites; sovereign revenue grew more than 80% YoY; NVIDIA AI infrastructure is deployed across nearly 40 countries representing $50 trillion in GDP (https://agentii.ai/v/NVDA/ect81/1). [FACT] Analysts now forecast hyperscale CapEx to exceed $1T by 2027 (https://agentii.ai/v/NVDA/ect81/1).

## 3. AI Exposure Risks

**[FACT]** Export controls are the single largest quantified AI-trend risk: a $4.5B H20 inventory/purchase-obligation charge in Q1 FY2026, ~$60M H20 revenue under August 2025 licenses, an H200 license with 25% import tariff, and no China data-center compute revenue included in guidance (https://agentii.ai/v/NVDA/sec169/36) (https://agentii.ai/v/NVDA/sec173/25). [FACT] Q1 FY2027 had zero China Hopper shipments versus $4.6B a year earlier (https://agentii.ai/v/NVDA/sec173/25).

**[FACT]** Competitive risk is disclosed on two fronts: open-source foundation models ("if deployed on our competitors' platforms, it could reduce demand for our products") and custom silicon/ASIC and cloud-internal designs (https://agentii.ai/v/NVDA/sec169/36). [FACT] Management counters: NVIDIA is "the only platform that runs every frontier AI model," with Anthropic newly added alongside OpenAI, xAI, Meta, and Gemini (https://agentii.ai/v/NVDA/ect81/5).

**[FACT]** Energy and data-center capacity are named as the scaling constraint: "Expanding energy capacity to meet demand is a complex, multi-year process that involves significant regulatory, technical, and construction challenges" (https://agentii.ai/v/NVDA/sec169/36). [VIEW] This is the most pillar-relevant sentence in the corpus: NVDA's management itself asserts the AI build-out is bounded by compute inputs (energy, capital, sites), not by data. PIL-1's data-boundness claim must therefore be read as specific to embodied AI, exactly as the thesis frames it.

## 4. Physical AI: NVDA's Third Wave

**[FACT]** Physical AI revenue exceeded $9B over the twelve months to Q1 FY2027 (https://agentii.ai/v/NVDA/ect81/1). [FACT] The Uber partnership will power a robotaxi fleet across nearly 30 cities and 4 continents by 2028 (https://agentii.ai/v/NVDA/ect81/1). [FACT] "In robotics, leading companies across a range of industrial, surgical, and humanoid applications are building on NVIDIA's technology, to develop and deploy at scale" (https://agentii.ai/v/NVDA/ect81/1). [FACT] Edge Computing — the disclosed bucket containing robotics — generated $6.4B in Q1 FY2027, +29% YoY, driven by Blackwell workstations (https://agentii.ai/v/NVDA/sec173/25).

**[FACT]** Jensen Huang's roadmap places robotics as the third platform wave after hyperscale and AI-factory segments: "within the next 5 years, physical AI and robotics segment is gonna grow incredibly fast," and "CUDA extends all the way to the edge. Robotics, autonomous vehicles, embedded medical instruments, AI RAN telco base stations. The next wave is physical AI. With billions of autonomous and robotic systems operating in the physical world" (https://agentii.ai/v/NVDA/ect81/5). [VIEW] This is the clearest management articulation supporting PIL-4's premise of an upcoming physical-AI inflection — but it is directional, undated, and uncounted.

**[FACT]** Software stack for physical AI: Blackwell Ultra is "optimized for agentic, reasoning, and physical AI," and NVDA accelerated release of open model platforms "NVIDIA Nemotron for agentic AI and Cosmos for physical AI" (https://agentii.ai/v/NVDA/sec169/4).

## 5. Financial Validation of AI Exposure

**[FACT]** GAAP gross margin was 74.9% in Q1 FY2027, with Blackwell "the majority of our revenue" (https://agentii.ai/v/NVDA/ect81/1) (https://agentii.ai/v/NVDA/sec173/25). [FACT] Record free cash flow of $49B, up from $35B in Q4 FY2026 (https://agentii.ai/v/NVDA/ect81/1). [FACT] Q2 FY2027 revenue guidance is $91B ±2%, with full-year gross margin expected in the mid-70s (https://agentii.ai/v/NVDA/ect81/1). [FACT] R&D in Q1 FY2027 was $6.3B, +58.5% YoY (XBRL us-gaap:ResearchAndDevelopmentExpense; see Verification), and full-year FY2027 OpEx growth is guided to the upper-40s percent, "driven by higher R&D and acceleration in the usage of AI tools" (https://agentii.ai/v/NVDA/ect81/1).

**[FACT]** FY2026 AI ecosystem investments: $17.5B into private companies and infrastructure funds, including AI model makers that purchase NVDA products directly or through CSPs (https://agentii.ai/v/NVDA/sec169/37). [DEDUCTED] NVDA is financing its own demand (model-maker investments, $3.5B land/power/shell guarantees, $27–30B cloud agreements) — a reinforcing but circular growth loop that concentrates counterparty risk.

## 6. Pillar Implications

- **PIL-1 counterfactual (compute-boundness):** Supported as scoped — NVDA's regime is compute/energy/capital-bound by management's own statement (https://agentii.ai/v/NVDA/sec169/36); no embodied-data disclosures exist to test the embodied-data gap from NVDA sources.
- **PIL-3 (manipulation reliability):** NVDA discloses nothing on robotic manipulation reliability or MTBF; the surgical/humanoid customers named in the call (https://agentii.ai/v/NVDA/ect81/1) are the disclosure owners. Coverage gap for this ticker.
- **PIL-4 (GPT-3.5 moment 2027-Q4–2028):** Compute platform is ready ahead of the falsifier window (VeraRubin ships Q3 2026, physical-AI stack shipping now); no humanoid unit counts disclosed, so the >10,000-units-before-2027-Q4 falsifier cannot be tested from NVDA filings.

## 7. Coverage Gaps & Citations

Coverage gaps:
1. No unit economics for physical AI (no robotics ASPs, no per-system attach rates).
2. No China-specific revenue outlook components beyond "not including any China data center compute revenue."
3. No disclosure of hyperscale capex concentration beyond the 21/17/16% direct-customer split.
4. VeraRubin "35x throughput" and "$1T visibility" are unaudited management statements (transcript-sourced); flagged as [FACT]-of-disclosure, not audited fact.

### Citations (roll-up index)

- https://agentii.ai/v/NVDA/sec169/4 — Blackwell Ultra physical AI optimization; Nemotron/Cosmos
- https://agentii.ai/v/NVDA/sec169/36 — MD&A: Blackwell majority, GB300, $4.5B H20 charge, energy constraint, open-source risk
- https://agentii.ai/v/NVDA/sec169/37 — FY2026 summary; $17.5B private investments
- https://agentii.ai/v/NVDA/sec169/55 — cash flow: OCF $102.7B, capex $6.0B, Groq $13.0B
- https://agentii.ai/v/NVDA/sec173/16 — $119B supply commitments, $30B cloud agreements
- https://agentii.ai/v/NVDA/sec173/21 — DC $75.2B +92%; Hyperscale/ACIE split
- https://agentii.ai/v/NVDA/sec173/25 — Edge Computing incl. robotics; no China Hopper; GM flat sequentially
- https://agentii.ai/v/NVDA/ect81/1 — DC compute $60B / networking $15B; $1T visibility; Vera $200B TAM; physical AI >$9B LTM; Uber; H100 rental +20%; FCF $49B; Q2 guide $91B
- https://agentii.ai/v/NVDA/ect81/5 — closing remarks: agentic AI arrived; physical AI third wave; VeraRubin Q3 ramp

## 8. Verification

| # | Material number | Value | Tool call that produced it |
|---|---|---|---|
| 1 | Q1 FY2027 revenue / Data Center | $81.6B / $75.2B (+85% / +92% YoY) | read_source_pages sec173 page21 (+ XBRL) |
| 2 | DC compute / networking Q1 FY2027 | $60B (+77%) / $15B (~3x) | read_source_pages ect81 page1 |
| 3 | Blackwell share of DC revenue | majority (FY2026 and Q1 FY2027) | read_source_pages sec169 page36, sec173 page25 |
| 4 | H20 charge / H20 revenue under license | $4.5B / ~$60M | read_source_pages sec169 page36 |
| 5 | China Hopper Q1 FY2027 vs FY2026 | $0 vs $4.6B | read_source_pages sec173 page25 |
| 6 | Supply commitments Apr 26, 2026 | $119B ($95B remainder FY2027) | read_source_pages sec173 page16 |
| 7 | Cloud agreements Apr 26, 2026 | $30B | read_source_pages sec173 page16 |
| 8 | Gross margin Q1 FY2027 | 74.9% | read_source_pages ect81 page1 (+ sec173 page25) |
| 9 | FCF Q1 FY2027 | $49B | read_source_pages ect81 page1 |
| 10 | Q2 FY2027 revenue guidance | $91B ±2% | read_source_pages ect81 page1 |
| 11 | Physical AI revenue LTM | >$9B | read_source_pages ect81 page1 |
| 12 | R&D Q1 FY2027 | $6,321M (+58.5% YoY) | search_xbrl_facts ResearchAndDevelopmentExpense |
| 13 | Private investments FY2026 | $17.5B | read_source_pages sec169 page37 |
| 14 | Blackwell+Rubin revenue visibility 2025–2027 | $1T (management statement) | read_source_pages ect81 page1 |
| 15 | Token cost reduction GB300 vs 6mo | -60% (2.7x throughput) | read_source_pages ect81 page1 |
| 16 | H100 rental price YTD | +20% | read_source_pages ect81 page1 |
