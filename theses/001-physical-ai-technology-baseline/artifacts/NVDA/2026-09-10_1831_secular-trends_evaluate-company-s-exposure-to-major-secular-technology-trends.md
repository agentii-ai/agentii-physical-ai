---
artifact_id: "001-NVDA-secular-trends-evaluate-company-s-exposure-to-major-secular-technology-trends-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: NVDA
skill: secular-trends
mode: evaluate-company-s-exposure-to-major-secular-technology-trends
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
    metric: datacenter_revenue_growth_yoy
    value: 68
    unit: pct
    period: FY2026
    source: "10-K:page37"
    retrieved_at: 2026-09-10
  - entity: NVDA
    metric: r_and_d_expense_growth_yoy
    value: 43.2
    unit: pct
    period: FY2026
    source: "XBRL:us-gaap:ResearchAndDevelopmentExpense (10-K)"
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
  - "agentii.ai/v/NVDA/sec169/36"
  - "agentii.ai/v/NVDA/sec169/37"
  - "agentii.ai/v/NVDA/sec169/55"
  - "agentii.ai/v/NVDA/sec169/70"
  - "agentii.ai/v/NVDA/sec169/77"
  - "agentii.ai/v/NVDA/sec169/79"
  - "agentii.ai/v/NVDA/sec173/19"
  - "agentii.ai/v/NVDA/sec173/20"
  - "agentii.ai/v/NVDA/sec173/21"
  - "agentii.ai/v/NVDA/sec173/23"
  - "agentii.ai/v/NVDA/sec173/25"
  - "agentii.ai/v/NVDA/ect81/1"
  - "agentii.ai/v/NVDA/ect81/5"
pillars_addressed: [PIL-1, PIL-3, PIL-4]
claim_state: pinned
key_metrics:
  revenue_fy2026_usd_m: 215938
  revenue_q1fy2027_usd_m: 81615
  datacenter_fy2026_usd_m: 193737
  edge_computing_q1fy2027_usd_m: 6369
  physical_ai_revenue_ltm_usd_b: 9
  capex_fy2026_usd_m: 6042
conclusions:
  - "NVDA's dominant secular exposure is AI/data-center compute (Data Center = 90% of FY2026 revenue); robotics/physical-AI exposure is real but small (~7.8% of quarterly revenue via Edge Computing) and disclosed only in qualitative terms."
  - "Management frames the binding constraint on AI scaling as data centers, energy, and capital — i.e., compute+energy-bound language, consistent with NVDA's role as the compute-boundness counterfactual for PIL-1."
  - "Robotics/physical-AI disclosures contain no embodied-data quantity metrics and no manipulation-reliability (MTBF) data; PIL-1 and PIL-3 falsifiers cannot be tested from NVDA filings alone."
facts_count: 24
deducted_count: 2
views_count: 3
citation_count: 16
---

# NVDA — Evaluate Company's Exposure to Major Secular Technology Trends

**Mode:** evaluate-company-s-exposure-to-major-secular-technology-trends
**Thesis:** 001-physical-ai-technology-baseline — NVDA is the compute-boundness counterfactual (PIL-1/PIL-3/PIL-4).
**Source set:** FY2026 10-K (sec169, filed 2026-02-25), FY2027 Q1 10-Q (sec173, filed 2026-05-20), Q1 FY2027 earnings call (ect81, 2026-05-20), XBRL facts.

## Executive Summary

NVDA's exposure to the AI secular trend is total: Data Center revenue was $193.7B in FY2026 (+68% YoY), 90% of total revenue (https://agentii.ai/v/NVDA/sec169/79), and $75.2B in Q1 FY2027 (+92% YoY), with Blackwell as the majority architecture (https://agentii.ai/v/NVDA/sec173/21). Total revenue reached $215.9B in FY2026 (+65%) and $81.6B in Q1 FY2027 (+85% YoY) (https://agentii.ai/v/NVDA/sec169/37) (https://agentii.ai/v/NVDA/sec173/21). Robotics/physical-AI exposure is disclosed qualitatively: "physical AI" revenue exceeded $9B over the last twelve months, and robotics customers span industrial, surgical, and humanoid applications (https://agentii.ai/v/NVDA/ect81/1). Structurally, robotics sits inside Edge Computing, which generated $6.4B in Q1 FY2027 (+29% YoY), 7.8% of revenue (https://agentii.ai/v/NVDA/sec173/25). Simulation/digital-twin (Omniverse) and AV (DRIVE) are strategic but financially immaterial. NVDA's filings frame the constraint on AI scaling as data-center capacity, energy, and capital — compute-bound language (https://agentii.ai/v/NVDA/sec169/36) — supporting its role as the thesis's compute-boundness counterfactual.

## 1. Trend Exposure Matrix (relevance_assessment)

| Trend | Exposure | Key evidence |
|---|---|---|
| AI / data-center accelerated computing | **Very high** | Data Center $193.7B FY2026, 90% of revenue (https://agentii.ai/v/NVDA/sec169/79) |
| Agentic AI | **High** | Blackwell Ultra "optimized for agentic, reasoning, and physical AI" (https://agentii.ai/v/NVDA/sec169/4); Vera CPU opens $200B TAM (https://agentii.ai/v/NVDA/ect81/1) |
| Robotics / embodied (physical) AI | **Medium-low, rising** | Physical AI revenue >$9B LTM (https://agentii.ai/v/NVDA/ect81/1); embedded in Edge Computing $6.4B +29% (https://agentii.ai/v/NVDA/sec173/25) |
| Simulation / digital twins | **Medium** | Omniverse "real-time 3D design collaboration and virtual world simulation" (https://agentii.ai/v/NVDA/sec169/7) |
| Autonomous vehicles | **Low-medium** | Automotive $2.3B FY2026, +39% YoY (https://agentii.ai/v/NVDA/sec169/79) |
| Sovereign AI | **Medium-high growth** | Sovereign revenue +80% YoY, ~40 countries (https://agentii.ai/v/NVDA/ect81/1) |
| Open-source AI | **Risk + counter-position** | Competitor-platform risk disclosed (https://agentii.ai/v/NVDA/sec169/36); NVDA ships open models (Nemotron, Cosmos) (https://agentii.ai/v/NVDA/sec169/4) |

## 2. Trend-by-Trend Exposure Detail (summary_findings)

**[FACT]** Revenue scaled from $60.9B (FY2024) to $130.5B (FY2025) to $215.9B (FY2026) (https://agentii.ai/v/NVDA/sec169/79). [FACT] Q1 FY2027 revenue of $81.6B was +85% YoY and +20% QoQ, the 14th consecutive quarter of sequential growth (https://agentii.ai/v/NVDA/ect81/1).

**[FACT]** Data Center FY2026 revenue was $193.7B, split Compute $162.4B and Networking $31.4B (https://agentii.ai/v/NVDA/sec169/79). [FACT] In Q1 FY2027, under the new market-platform presentation, Data Center was $75.2B (+92% YoY): Hyperscale $37.9B (+115%) and AI Clouds, Industrial & Enterprise (ACIE) $37.4B (+74%) (https://agentii.ai/v/NVDA/sec173/21). [DEDUCTED] Data Center is ~92% of Q1 FY2027 revenue; hyperscale is ~50% of Data Center, so hyperscale is ~46% of total revenue — exposure concentration in a small number of buyers. [FACT] Three direct customers were 21%, 17%, and 16% of Q1 FY2027 total revenue (https://agentii.ai/v/NVDA/sec173/20).

**[FACT]** Robotics and physical AI are explicitly bundled into Edge Computing: "Edge Computing highlights devices for agentic and physical AI including PCs, game consoles, workstations, AI-RAN base stations, robotics and automotive" (https://agentii.ai/v/NVDA/sec173/25). [FACT] Edge Computing revenue was $6.4B in Q1 FY2027, +29% YoY (https://agentii.ai/v/NVDA/sec173/21). [FACT] CFO disclosed physical AI revenue "exceeding $9 billion in revenue over the last 12 months" and an Uber robotaxi partnership across ~30 cities and 4 continents by 2028 (https://agentii.ai/v/NVDA/ect81/1). [FACT] "Leading companies across a range of industrial, surgical, and humanoid applications are building on NVIDIA's technology" (https://agentii.ai/v/NVDA/ect81/1). [VIEW] Robotics is real, growing, but economically undifferentiated inside a $6.4B bucket — NVDA cannot yet claim a disclosed robotics P&L line.

**[FACT]** Simulation assets: Omniverse is described as virtual-world simulation software (https://agentii.ai/v/NVDA/sec169/7), and NVDA accelerated release of "Cosmos for physical AI" open model platforms (https://agentii.ai/v/NVDA/sec169/4). [FACT] The DRIVE AV platform includes GPU-based re-simulation of AV operation before OTA updates (https://agentii.ai/v/NVDA/sec169/7). [VIEW] Simulation is NVDA's chosen instrument for embodied-AI data generation — strategically aligned with the thesis's data-boundness pillar (PIL-1), though no simulation-revenue quantification is disclosed.

**[FACT]** Gaming FY2026 revenue was $16.0B, +41% YoY (https://agentii.ai/v/NVDA/sec169/37); Automotive $2.3B, +39% (https://agentii.ai/v/NVDA/sec169/79). [FACT] Graphics segment (GeForce + RTX workstation) revenue was $7.1B in Q1 FY2027, +58% YoY, with segment operating income of $2.9B (https://agentii.ai/v/NVDA/sec173/19).

## 3. Financial Validation (quantitative_support)

**[FACT]** R&D expense grew from $12.9B (FY2025) to $18.5B (FY2026), +43.2% YoY, and Q1 FY2027 R&D was $6.3B, +58.5% YoY (XBRL us-gaap:ResearchAndDevelopmentExpense; see Verification). [FACT] Cumulative R&D since inception exceeded $76.7B, and more than half of NVDA's engineers work on software (https://agentii.ai/v/NVDA/sec169/4). [FACT] FY2026 capex (purchases of property, equipment, and intangibles) was $6.0B (https://agentii.ai/v/NVDA/sec169/55). [DEDUCTED] Capex is only 2.8% of FY2026 revenue — NVDA is asset-light; the physical compute build-out is capitalized on customer balance sheets, consistent with NVDA monetizing the compute trend rather than owning its infrastructure.

**[FACT]** FY2026 operating cash flow was $102.7B (https://agentii.ai/v/NVDA/sec169/55). [FACT] Total operating expenses grew 41% in FY2026 to $23.1B (https://agentii.ai/v/NVDA/sec169/37). [FACT] Segment operating income in Q1 FY2027 was $56.3B before unallocated items (https://agentii.ai/v/NVDA/sec173/20).

**[FACT]** Supply commitment evidence of secular demand: manufacturing/supply/capacity commitments of $95.2B as of Jan 25, 2026 (https://agentii.ai/v/NVDA/sec169/70), rising to $119B by Apr 26, 2026 (https://agentii.ai/v/NVDA/sec173/16). [FACT] Multi-year cloud service agreements (compute purchased by NVDA itself for R&D) were $27B, rising to $30B (https://agentii.ai/v/NVDA/sec169/70) (https://agentii.ai/v/NVDA/sec173/16).

**[FACT]** Constraint framing: "The availability of data centers, energy, and capital to support the buildout of NVIDIA AI infrastructure by our customers and partners is crucial" (https://agentii.ai/v/NVDA/sec169/36) (https://agentii.ai/v/NVDA/sec173/23). [VIEW] Management's own language is compute- and energy-bound, not data-bound — direct counterfactual evidence for PIL-1's claim that embodied AI (not this LLM/data-center regime) is the data-bound domain. This does not falsify PIL-1; it bounds its scope.

**[FACT]** Export controls are the main AI-trend disrupter: a $4.5B H20 charge in Q1 FY2026, ~$60M H20 revenue under licenses, and zero China data-center compute revenue included in the outlook (https://agentii.ai/v/NVDA/sec169/36) (https://agentii.ai/v/NVDA/sec173/25). [FACT] Revenue from customers headquartered outside the US fell to 22% of total in Q1 FY2027 from 42% a year earlier (https://agentii.ai/v/NVDA/sec173/20).

## 4. Pillar Linkage

- **PIL-1 (embodied AI is data-bound):** NVDA's robotics strategy leans on simulation-generated data (Omniverse/Cosmos), which is consistent with embodied-data scarcity being the open problem; but NVDA discloses no embodied-data quantity metrics. Exposure verdict: platform exposure high, falsifier data absent.
- **PIL-3 (manipulation reliability gates deployment):** No MTBF or manipulation-reliability disclosures exist in NVDA filings; reliability sits with robotics customers (industrial/surgical/humanoid). Coverage gap.
- **PIL-4 (GPT-3.5 moment 2027-Q4–2028):** Compute-side readiness is concrete — VeraRubin production shipments start Q3 calendar 2026 (https://agentii.ai/v/NVDA/ect81/1) and Jensen expects "physical AI and robotics segment" to "grow incredibly fast" within 5 years (https://agentii.ai/v/NVDA/ect81/5). NVDA discloses no humanoid unit counts, so the >10,000-units falsifier is untestable from this source set.

## 5. Coverage Gaps & Citations

Coverage gaps:
1. **Robotics/simulation standalone revenue:** not disclosed; embedded in Edge Computing ($6.4B Q1 FY2027) and ACIE. Only the LTM physical-AI figure (>$9B) is disclosed verbally (https://agentii.ai/v/NVDA/ect81/1).
2. **Embodied-data metrics:** none (no dataset hours, teleoperation, or synthetic-data volumes).
3. **Humanoid unit deployments / MTBF:** none.
4. **Second revenue concept:** us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax is not tagged by NVDA (empty result set); revenue verified instead via consolidated + dimensioned Revenues facts (OperatingSegments / ProductOrService axes).
5. **Capex concept:** us-gaap:PaymentsToAcquirePropertyPlantAndEquipment is stale for NVDA (last used 2020); current series is PaymentsToAcquireProductiveAssets ($6.0B FY2026).

### Citations (roll-up index)

- https://agentii.ai/v/NVDA/sec169/4 — business overview, $76.7B cumulative R&D, Cosmos/Nemotron, Blackwell Ultra
- https://agentii.ai/v/NVDA/sec169/7 — Omniverse, DRIVE, CUDA 7.5M developers, AI Enterprise
- https://agentii.ai/v/NVDA/sec169/36 — MD&A: Blackwell majority, GB300, H20 $4.5B charge, energy constraint, open-source risk
- https://agentii.ai/v/NVDA/sec169/37 — FY2026 summary table: revenue $215.9B, GM 71.1%, segment growth, $17.5B private investments
- https://agentii.ai/v/NVDA/sec169/55 — cash flow: OCF $102.7B, Groq $13.0B, capex $6.0B
- https://agentii.ai/v/NVDA/sec169/70 — commitments: $95.2B supply, $27B cloud, debt $8.5B
- https://agentii.ai/v/NVDA/sec169/77 — segment table FY2024–FY2026
- https://agentii.ai/v/NVDA/sec169/79 — end-market revenue: DC $193.7B, Compute $162.4B, Networking $31.4B, Gaming $16.0B, Auto $2.3B; $22.7B future DC leases
- https://agentii.ai/v/NVDA/sec173/16 — commitments $119B, cloud $30B
- https://agentii.ai/v/NVDA/sec173/19 — Q1 FY2027 segments: C&N $74.55B, Graphics $7.07B
- https://agentii.ai/v/NVDA/sec173/20 — customer concentration 21/17/16%; outside-US revenue 22%
- https://agentii.ai/v/NVDA/sec173/21 — platform revenue: DC $75.2B (+92%), Hyperscale $37.9B, ACIE $37.4B, Edge $6.4B; $32.4B future DC leases
- https://agentii.ai/v/NVDA/sec173/23 — MD&A Q1: Blackwell majority of shipments
- https://agentii.ai/v/NVDA/sec173/25 — Edge Computing definition incl. robotics; no China Hopper shipments
- https://agentii.ai/v/NVDA/ect81/1 — prepared remarks: physical AI >$9B LTM, Uber, Vera $200B TAM, $1T Blackwell/Rubin visibility, H100 rental +20%, Q2 guide $91B
- https://agentii.ai/v/NVDA/ect81/5 — closing: physical AI as third segment, billions of robotic systems

## 6. Verification

| # | Material number | Value | Tool call that produced it |
|---|---|---|---|
| 1 | FY2026 revenue | $215,938M | read_source_pages sec169 page37 (+ XBRL Revenues, authority 3) |
| 2 | Q1 FY2027 revenue | $81,615M | read_source_pages sec173 page21 (+ XBRL Revenues Q1 FY2027) |
| 3 | Data Center FY2026 | $193,737M | read_source_pages sec169 page79 (+ XBRL Revenues DataCenterMember) |
| 4 | DC Compute/Networking FY2026 | $162,361M / $31,376M | read_source_pages sec169 page79 (+ XBRL detailed) |
| 5 | Q1 FY2027 DC / Hyperscale / ACIE / Edge | $75,246M / $37,869M / $37,377M / $6,369M | read_source_pages sec173 page21 (+ XBRL detailed) |
| 6 | Physical AI revenue LTM | >$9B | read_source_pages ect81 page1 |
| 7 | R&D FY2025 / FY2026 / Q1 FY2027 | $12,914M / $18,497M / $6,321M | search_xbrl_facts ResearchAndDevelopmentExpense |
| 8 | Capex FY2026 | $6,042M | search_xbrl_facts PaymentsToAcquireProductiveAssets + read_source_pages sec169 page55 |
| 9 | OCF FY2026 | $102,718M | read_source_pages sec169 page55 |
| 10 | Supply commitments (Jan / Apr 2026) | $95.2B / $119B | read_source_pages sec169 page70 / sec173 page16 |
| 11 | Cloud agreements (Jan / Apr 2026) | $27B / $30B | read_source_pages sec169 page70 / sec173 page16 |
| 12 | Customer concentration Q1 FY2027 | 21% / 17% / 16% | read_source_pages sec173 page20 |
| 13 | H20 charge | $4.5B | read_source_pages sec169 page36 |
| 14 | Outside-US revenue share Q1 FY2027 | 22% | read_source_pages sec173 page20 |
| 15 | Segment revenue Q1 FY2027 C&N / Graphics | $74,550M / $7,065M | read_source_pages sec173 page19 (+ XBRL detailed) |
| 16 | Gaming / Automotive FY2026 | $16,042M / $2,349M | read_source_pages sec169 page79 |
