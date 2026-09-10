---
artifact_id: "001-NVDA-secular-trends-deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: NVDA
skill: secular-trends
mode: deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure
affix: tech-trends
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "e6b41dbb2426"
as_of: 2026-09-10
entity_claims:
  - entity: NVDA
    metric: robotics_and_simulation_revenue_share_of_total_pct
    value: 7.8
    unit: pct
    period: 2027Q1
    source: "10-Q:page21"
    retrieved_at: 2026-09-10
  - entity: NVDA
    metric: datacenter_revenue_growth_yoy
    value: 92
    unit: pct
    period: 2027Q1
    source: "10-Q:page21"
    retrieved_at: 2026-09-10
  - entity: NVDA
    metric: r_and_d_expense_growth_yoy
    value: 58.5
    unit: pct
    period: 2027Q1
    source: "XBRL:us-gaap:ResearchAndDevelopmentExpense (10-Q)"
    retrieved_at: 2026-09-10
citations:
  - "agentii.ai/v/NVDA/sec169/4"
  - "agentii.ai/v/NVDA/sec169/7"
  - "agentii.ai/v/NVDA/sec169/37"
  - "agentii.ai/v/NVDA/sec169/55"
  - "agentii.ai/v/NVDA/sec169/70"
  - "agentii.ai/v/NVDA/sec169/79"
  - "agentii.ai/v/NVDA/sec173/14"
  - "agentii.ai/v/NVDA/sec173/16"
  - "agentii.ai/v/NVDA/sec173/21"
  - "agentii.ai/v/NVDA/ect81/1"
pillars_addressed: [PIL-1, PIL-3, PIL-4]
claim_state: pinned
key_metrics:
  deferred_revenue_q1fy2027_usd_m: 3117
  remaining_performance_obligations_gt1yr_usd_b: 2.6
  cloud_agreement_commitments_apr2026_usd_b: 30
  expected_dc_leases_usd_b: 32.4
  groq_license_payment_fy2026_usd_b: 13.0
  private_investments_fy2026_usd_b: 17.5
  cuda_developers_m: 7.5
conclusions:
  - "NVDA monetizes data-adjacent value almost entirely through hardware: deferred revenue of $3.1B and >1yr remaining performance obligations of $2.6B are immaterial against $81.6B of quarterly revenue — NVDA is not a data-sale business."
  - "NVDA's strategic position on data value is simulation-generated data (Omniverse world simulation, Cosmos physical-AI world models, DRIVE re-simulation) — consistent with the thesis premise that embodied-AI data acquisition is the binding open problem (PIL-1), though NVDA discloses no embodied-data quantities."
  - "NVDA is itself becoming a large compute/data buyer for its own R&D ($30B cloud commitments, $32.4B expected data-center leases), reinforcing that the compute input — not data — is where capital is being spent."
facts_count: 18
deducted_count: 4
views_count: 4
citation_count: 10
---

# NVDA — Deep Dive: Data Value Trend Assessment (Identified Data Exposure)

**Mode:** deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure
**Thesis:** 001-physical-ai-technology-baseline — PIL-1: embodied AI is data-bound, not compute-bound; NVDA is the compute-boundness counterfactual.
**Source set:** FY2026 10-K (sec169), FY2027 Q1 10-Q (sec173), Q1 FY2027 earnings call (ect81, 2026-05-20), XBRL.

## Executive Summary

NVDA has near-zero direct data-sale exposure and maximal indirect data-value exposure. Its balance sheet proves the first point: deferred revenue of $3.1B and remaining performance obligations (>1 year) of $2.6B are immaterial against $81.6B of quarterly revenue (https://agentii.ai/v/NVDA/sec173/14) (https://agentii.ai/v/NVDA/sec173/21) — NVDA sells compute, not data. Its indirect data-value exposure runs through five vectors: (1) simulation-generated data platforms (Omniverse, Cosmos, DRIVE re-simulation) (https://agentii.ai/v/NVDA/sec169/7) (https://agentii.ai/v/NVDA/sec169/4); (2) an ecosystem gravity of 7.5M CUDA developers (https://agentii.ai/v/NVDA/sec169/7); (3) model-layer investments of $17.5B in FY2026 plus a $13.0B Groq LPU license (https://agentii.ai/v/NVDA/sec169/37) (https://agentii.ai/v/NVDA/sec169/55); (4) sovereign-AI data infrastructure (~40 countries, $50T GDP) (https://agentii.ai/v/NVDA/ect81/1); and (5) its own growing compute purchases — $30B cloud commitments and $32.4B expected data-center leases for R&D (https://agentii.ai/v/NVDA/sec173/16) (https://agentii.ai/v/NVDA/sec173/21). Critically for PIL-1, NVDA's embodied-AI data strategy is simulation-first, and it discloses no embodied-data quantities whatsoever — consistent with, though not dispositive of, the thesis's claim that embodied data is the scarce input.

## 1. Where NVDA's Data Value Sits: Five Vectors

### 1.1 Simulation-generated data (the embodied-AI vector — most PIL-1-relevant)

**[FACT]** Omniverse is "real-time 3D design collaboration and virtual world simulation software" (https://agentii.ai/v/NVDA/sec169/7). [FACT] NVDA "accelerated the release cadence of our open AI model platforms including NVIDIA Nemotron for agentic AI and Cosmos for physical AI" (https://agentii.ai/v/NVDA/sec169/4). [FACT] The DRIVE AV solution includes "GPU-based hardware required to train the neural networks before their in-vehicle deployment, as well as to re-simulate their operation prior to any over-the-air software updates" (https://agentii.ai/v/NVDA/sec169/7). [DEDUCTED] Simulation/re-simulation is NVDA's disclosed mechanism for generating training data for embodied systems — an implicit acknowledgment that field-collected embodied data is scarce or expensive, which is the core premise of PIL-1. [VIEW] Cosmos-as-open-platform is best read as a strategy to make synthetic data cheap at scale — if successful, it would compress the embodied-data gap that PIL-1's wrong_if tests (>3 orders of magnitude vs LLM pretrain tokens). No disclosure quantifies synthetic-data volume, so the gap cannot be measured from NVDA sources.

### 1.2 Ecosystem and developer gravity

**[FACT]** "There are over 7.5 million developers worldwide using CUDA and our other software tools" (https://agentii.ai/v/NVDA/sec169/7). [FACT] NVDA evangelizes AI through "hundreds of universities and tens of thousands of startups through our Inception program" (https://agentii.ai/v/NVDA/sec169/7). [VIEW] This is NVDA's durable data-adjacent moat: the developer base generates the model code, frameworks, and data pipelines that make its hardware the default substrate — but it appears nowhere on the P&L as a data line.

### 1.3 Model-layer and data-ecosystem investments

**[FACT]** In FY2026 NVDA invested $17.5B in private companies and infrastructure funds, "including AI model makers that purchase our products directly or through CSPs" (https://agentii.ai/v/NVDA/sec169/37). [FACT] NVDA paid $13.0B for a non-exclusive Groq license (LPU technology) in FY2026 (https://agentii.ai/v/NVDA/sec169/55), with accrued purchase consideration of $4.0B still on the balance sheet as of Apr 26, 2026 (https://agentii.ai/v/NVDA/sec173/14). [FACT] Q1 FY2027 also carried $13.4B of unrealized gains on publicly-held equity securities (source: 10-Q Note 5; see Verification). [DEDUCTED] NVDA is a material holder of model-layer equity — its data-value exposure includes mark-to-market exposure to the model ecosystem it supplies.

### 1.4 Sovereign and industrial data infrastructure

**[FACT]** Sovereign revenue grew more than 80% YoY, with NVIDIA AI infrastructure "now deployed across nearly 40 countries representing $50 trillion in GDP" (https://agentii.ai/v/NVDA/ect81/1). [FACT] The ACIE (AI Clouds, Industrial & Enterprise) platform generated $37.4B in Q1 FY2027, +74% YoY and +31% QoQ, with AI-cloud revenue "more than tripled year over year" (https://agentii.ai/v/NVDA/sec173/21) (https://agentii.ai/v/NVDA/ect81/1). [VIEW] Sovereign/industrial data-sovereignty demand is a structural growth vector: data that cannot leave a jurisdiction requires in-country compute — a direct data-value → compute revenue translation.

### 1.5 NVDA as a compute/data buyer for its own R&D

**[FACT]** Multi-year cloud service agreement commitments were $27B as of Jan 25, 2026, expected "to be used to support our research and development efforts" (https://agentii.ai/v/NVDA/sec169/70), rising to $30B by Apr 26, 2026 (https://agentii.ai/v/NVDA/sec173/16). [FACT] NVDA expects to commence data-center leases with future obligations of $22.7B (FY2027–2030 per 10-K) (https://agentii.ai/v/NVDA/sec169/79), raised to $32.4B (Q2 FY2027–FY2033 per 10-Q), "primarily for data center leases to support our research and development efforts" (https://agentii.ai/v/NVDA/sec173/21). [DEDUCTED] NVDA's R&D is becoming compute-purchase-intensive (R&D expense +58.5% YoY in Q1 FY2027; XBRL — see Verification) — the company spends capital on compute inputs for its own model/data work, not on data acquisition.

## 2. The Data-Value Structure: Hardware-Led, Software-Thin

**[FACT]** Deferred revenue at Apr 26, 2026 was $3.1B ($1.7B current + $1.4B long-term), including $297M of customer advances (https://agentii.ai/v/NVDA/sec173/14). [FACT] Remaining performance obligations from contracts longer than one year were $2.6B (https://agentii.ai/v/NVDA/sec173/14). [DEDUCTED] RPO >1 year is 0.8% of FY2026 revenue ($215.9B) — NVDA's contracted software/service/data backlog is negligible relative to hardware; subscription-style data monetization is structurally absent. [FACT] Deferred revenue additions in Q1 FY2027 were $2.5B against revenue recognized of $2.0B (https://agentii.ai/v/NVDA/sec173/14).

**[FACT]** Inference is now the volume data-consumption workload: "Tokens are now profitable, so model makers are in a race to produce more. In the AI era, compute capacity is revenue, and profits" (https://agentii.ai/v/NVDA/ect81/5). [FACT] GB300 delivered a 60% reduction in cost per token versus six months prior (https://agentii.ai/v/NVDA/ect81/1). [VIEW] Token economics make compute the toll booth on data's value — NVDA's data-value trend is the unit-economics improvement of turning data (tokens) into revenue for its customers.

## 3. Pillar Implications

- **PIL-1 (data-bound embodied AI):** NVDA's simulation-first embodied-AI data strategy (Omniverse/Cosmos/re-simulation) is consistent with the premise that embodied data is the scarce input, but NVDA discloses no embodied-data quantity metrics, so the >3-orders-of-magnitude gap falsifier is untestable from this ticker. NVDA's regime-level disclosures (energy/capital as constraints) delimit the compute-boundness counterfactual cleanly.
- **PIL-3 (manipulation reliability):** No data. The named robotics customers (industrial, surgical, humanoid) are the disclosure owners; NVDA's role is compute supplier, not reliability measurer.
- **PIL-4 (GPT-3.5 moment timing):** Data-side readiness signals exist only directionally: Cosmos/Nemotron open platforms shipped, physical AI revenue >$9B LTM (https://agentii.ai/v/NVDA/ect81/1), Uber robotaxi deployment targeting 2028 (https://agentii.ai/v/NVDA/ect81/1). No humanoid unit counts → falsifier untestable.

## 4. Coverage Gaps & Citations

Coverage gaps:
1. **No embodied-data quantities:** zero disclosures of dataset hours, synthetic-data volumes, or teleoperation data.
2. **No software/data revenue line:** NVIDIA AI Enterprise, DGX Cloud, and software subscriptions are not separately quantified; deferred revenue ($3.1B) is the only proxy.
3. **No robotics attach-rate data:** cannot size per-robot compute/data economics from filings.
4. **Groq license economics:** payment ($13.0B) and accrual ($4.0B) disclosed, but license amortization/benefit not quantified on a data-value basis.
5. **Public-equity gain detail:** the $13.4B Q1 FY2027 unrealized gain figure comes from the 10-Q note outline (Note 5); page-level confirmation was not re-read due to rate limits — flagged as outline-level [FACT], listed in Verification with its tool call.

### Citations (roll-up index)

- https://agentii.ai/v/NVDA/sec169/4 — Cosmos/Nemotron open platforms; Blackwell Ultra physical AI; $76.7B cumulative R&D
- https://agentii.ai/v/NVDA/sec169/7 — Omniverse; DRIVE re-simulation; 7.5M CUDA developers; AI Enterprise
- https://agentii.ai/v/NVDA/sec169/37 — $17.5B private investments FY2026
- https://agentii.ai/v/NVDA/sec169/55 — Groq $13.0B; capex $6.0B
- https://agentii.ai/v/NVDA/sec169/70 — $27B cloud agreements; $95.2B supply commitments
- https://agentii.ai/v/NVDA/sec169/79 — $22.7B expected DC leases
- https://agentii.ai/v/NVDA/sec173/14 — deferred revenue $3.1B; RPO $2.6B; Groq accrued purchase consideration $4.0B
- https://agentii.ai/v/NVDA/sec173/16 — $30B cloud agreements; $119B supply commitments
- https://agentii.ai/v/NVDA/sec173/21 — ACIE $37.4B +74%; $32.4B expected DC leases; total revenue $81.6B
- https://agentii.ai/v/NVDA/ect81/1 — sovereign +80%; ~40 countries/$50T GDP; physical AI >$9B LTM; Uber 2028; 60% token cost reduction

## 5. Verification

| # | Material number | Value | Tool call that produced it |
|---|---|---|---|
| 1 | Deferred revenue (Apr 26, 2026) | $3,117M ($297M advances) | read_source_pages sec173 page14 |
| 2 | RPO >1 year (Apr 26, 2026) | $2.6B | read_source_pages sec173 page14 |
| 3 | Quarterly revenue (comparator) | $81,615M | read_source_pages sec173 page21 (+ XBRL) |
| 4 | Cloud agreements Jan / Apr 2026 | $27B / $30B | read_source_pages sec169 page70 / sec173 page16 |
| 5 | Expected DC leases | $22.7B / $32.4B | read_source_pages sec169 page79 / sec173 page21 |
| 6 | Groq license payment FY2026 | $13.0B | read_source_pages sec169 page55 |
| 7 | Groq accrued purchase consideration | $3,957M | read_source_pages sec173 page14 |
| 8 | Private investments FY2026 | $17.5B | read_source_pages sec169 page37 |
| 9 | CUDA developers | 7.5M | read_source_pages sec169 page7 |
| 10 | Sovereign revenue growth / country count | +80% / ~40 countries ($50T GDP) | read_source_pages ect81 page1 |
| 11 | ACIE revenue Q1 FY2027 | $37,377M (+74% YoY) | read_source_pages sec173 page21 |
| 12 | Physical AI revenue LTM | >$9B | read_source_pages ect81 page1 |
| 13 | R&D Q1 FY2027 | $6,321M (+58.5% YoY) | search_xbrl_facts ResearchAndDevelopmentExpense |
| 14 | Unrealized gains on public equities Q1 FY2027 | $13.4B | read_source_outline sec173 (page11 description, Note 5) |
| 15 | Token cost reduction GB300 | -60% | read_source_pages ect81 page1 |
| 16 | FY2026 revenue (RPO comparator) | $215,938M | read_source_pages sec169 page37 (+ XBRL) |
