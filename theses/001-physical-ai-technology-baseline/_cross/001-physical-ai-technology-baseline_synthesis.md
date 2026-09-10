---
artifact_id: "001-cross-technology-baseline-20260910"
thesis_id: "001-physical-ai-technology-baseline"
type: cross_synthesis
tickers_covered: [NVDA, ISRG, TSLA, AMZN, PH, SPCX]
pillars_synthesized: [PIL-1, PIL-2, PIL-3, PIL-4]
pillar_verdicts:
  PIL-1: indeterminate   # falsifier test: embodied-data gap >3 orders of magnitude — UNTESTABLE (no embodied-data volumes disclosed anywhere in the corpus)
  PIL-2: indeterminate   # falsifier test: actuator share <35% — NOT TRIGGERED but NO EVIDENCE EXISTS (no humanoid teardown or 10-K BOM disclosure anywhere; 40-70% remains industry estimate)
  PIL-3: supported       # falsifier test: humanoid MTBF >2000h disclosed — NOT TRIGGERED (no MTBF disclosed anywhere, incl. ISRG); gating premise corroborated by TSLA management statements
  PIL-4: supported       # falsifier test: >10,000 commercial humanoid units before 2027-Q4 — NOT TRIGGERED (TSLA 10-K: "We have yet to commercialize Bots"; zero disclosed units)
constitution_pin: "1.3.0"
as_of: 2026-09-10
capability_timeline:
  gpt_3_5_moment_estimate: "2027-Q4 to 2028-Q2"   # interval estimate, never a point (plan risk note 2)
  confidence: medium
---

# Cross-Stock Synthesis — Physical AI Technology Baseline (001)

**Synthesis task:** T025 (never-[P]) · **Inputs:** 24 per-ticker artifacts (NVDA ×6, ISRG ×5, TSLA ×7, AMZN ×2, PH ×2, SPCX ×1) · **Contract:** contracts/output-schemas.md §2 · **Constitution pin:** 1.3.0 · **As of:** 2026-09-10 · **No retrieval calls made** — all evidence and citations carried from the artifacts.

---

## Executive Summary

Across six names and 24 artifacts, the Q3-2026 disclosure record is consistent with — but does not prove — the thesis's central claim that embodied AI is data- and reliability-bound rather than compute-bound, with a step-change window of 2027-Q4 to 2028-Q2.

- **PIL-1 (data-bound): indeterminate.** No company discloses embodied-data volumes; the >3-orders-of-magnitude gap test is unmeasurable. Mechanism evidence (NVDA simulation-first, TSLA fleet-data strategy) is directionally consistent; TSLA's chip-supply commentary is a recorded counterpoint.
- **PIL-2 (actuator BOM 40–70%): indeterminate.** No teardown or 10-K discloses a humanoid BOM anywhere; PH's premium-margin Motion Systems franchise is the closest structural proxy and supports direction, not magnitude.
- **PIL-3 (reliability gates): supported.** No MTBF is disclosed anywhere — including ISRG after 25 years and 13M+ procedures; TSLA management twice states reliability (not capability) is the deployment gate. Falsifier (>2,000h MTBF disclosed) untriggered.
- **PIL-4 (2027-Q4–2028 inflection): supported.** TSLA's own 10-K: "we have yet to commercialize Bots"; no commercial humanoid units disclosed by anyone; TSLA's ramp, ISRG's S-curves, AMZN's sequencing, and SPCX's compute-led capex all point to late-2027/2028. Unit-count aspirations treated as promotional.

Headline output: GPT-3.5-moment interval **2027-Q4 to 2028-Q2**, confidence **medium**.

---

## 1. Pillar-by-pillar falsifier evaluation

### PIL-1 — Data, not compute, is the binding constraint — VERDICT: indeterminate

**wrong_if:** `metric=embodied_dataset_hours_vs_llm_pretrain_token_gap_order_of_magnitude threshold=>3 source=industry_technical_disclosures op=>`

**Falsifier test result: UNTESTABLE** — not triggered, not passed. No industry technical disclosure quantifying embodied-data volumes versus LLM pretrain tokens exists in the retrieval scope, and no company in the six-name corpus discloses any embodied-data volume (dataset hours, teleoperation hours, episodes, or tokens). The metric cannot be computed; the pillar can be neither falsified nor confirmed in magnitude.

**Best evidence found:**
- **NVDA (compute-boundness counterfactual):** management names energy, data-center capacity, and capital as the binding constraints on the LLM regime (https://agentii.ai/v/NVDA/sec169/36) — bounding PIL-1's scope to embodied AI, exactly as the thesis frames it. NVDA's embodied-AI strategy is simulation-first (Omniverse, Cosmos, DRIVE re-simulation — https://agentii.ai/v/NVDA/sec169/7), consistent with field embodied data being scarce, but discloses zero embodied-data quantities.
- **TSLA (mechanism, no magnitude):** discloses the embodied-data collection stack in full — factory-human observation fleet, dedicated demo team, internet video, Optimus Academy RL loop — and earmarks the first Optimus builds for data collection rather than sale (https://agentii.ai/v/TSLA/sec258/9, https://agentii.ai/v/TSLA/ect61/3), but zero volumes. Its disclosures are compute-rich (~250 MW → ~400 MW planned; AI-infrastructure PP&E $10.8B — https://agentii.ai/v/TSLA/sec258/10) and data-poor in units. Recorded counterpoint, not suppressed: management itself treats chip supply as a prospective binding constraint ("we simply won't have enough AI chips" to scale Optimus — https://agentii.ai/v/TSLA/ect61/1).
- **AMZN:** >1M warehouse robots are the largest disclosed generator of industrial embodied-robot operational data (https://agentii.ai/v/AMZN/ect81/5); no data volumes disclosed.
- **ISRG:** the data flywheel is monetized (84% recurring revenue — https://agentii.ai/v/ISRG/sec166/page78) and the dv5 10,000x compute step was spent on data-capture infrastructure (https://agentii.ai/v/ISRG/sec166/page8) — compute enabling data capture, not replacing it; no dataset-size disclosure.

**Verdict: indeterminate** — plausible and directionally corroborated, but the falsifier is unmeasurable from this corpus. Not upgraded (no_verdict_inflation).

### PIL-2 — Actuators dominate BOM; compute is marginal — VERDICT: indeterminate

**wrong_if:** `metric=actuator_share_of_humanoid_bom_pct threshold=<35 source=public_teardown_or_10K_disclosure op=<`

**Falsifier test result: NOT TRIGGERED, but no evidence of either sign exists.** No humanoid teardown is in the corpus and no 10-K discloses any humanoid BOM split whatsoever. The 40–70% actuator / 10–15% compute claim remains an industry estimate (plan risk note 4): an honest reading cannot falsify it from filings, and equally cannot confirm it.

**Best evidence found:**
- **PH (closest structural proxy):** Motion Systems — the platform containing the exact PIL-2 categories (electromechanical/hydraulic actuators, pumps/motors, drives/controllers) — $3,580M FY2026 (https://agentii.ai/v/PH/sec166/44). Premium economics: DI segment operating margin 23.8%, Aerospace 26.0% (https://agentii.ai/v/PH/sec166/25, https://agentii.ai/v/PH/sec166/26), consolidated GM 37.7% (https://agentii.ai/v/PH/sec166/23) — actuators are high-value engineered content, directionally consistent with a large BOM share. But PH has zero humanoid/robotics disclosure ("robot" = 0 hits in the FY2026 10-K), no content-per-platform dollars, no platform-level profitability, and no quantitative rare-earth data (https://agentii.ai/v/PH/sec166/11).
- **ISRG (disclosed analogue, direction only):** effectively ~100% of its revenue stack is actuation-adjacent — instruments & accessories 59.8% of FY2025 revenue, actuated capital at $0.6–3.1M, precision-maintenance service $95–225K/yr (https://agentii.ai/v/ISRG/sec166/page77) — and da Vinci ASPs rose $1.50M → $1.66M on actuation/feature content while compute costs elsewhere deflate (https://agentii.ai/v/ISRG/sec166/page78). The finest disclosed cost cut is product vs service gross margin (66.3%/64.6% — https://agentii.ai/v/ISRG/sec166/page79); no BOM-level split exists to calibrate the 40–70% magnitude.
- **TSLA:** zero Optimus BOM or per-unit cost disclosure (https://agentii.ai/v/TSLA/sec253/36). The only cost-structure commentary is compute-side — "a lot of really specialized power electronics and circuit boards", Samsung/TSMC/Micron AI-compute investment (https://agentii.ai/v/TSLA/ect61/5, https://agentii.ai/v/TSLA/ect61/3) — consistent with compute being the scarce minority (~10–15%) of BOM, silent on the actuator figure.
- **NVDA (supplier-side mix, not a BOM):** today's value-weighted physical-AI stack is compute, not actuators (Data Center $75.2B vs Edge $6.4B Q1 FY2027 — https://agentii.ai/v/NVDA/sec173/21) — a statement about the build-out phase, not a humanoid's bill of materials.

**Verdict: indeterminate** — the <35% falsifying evidence has not appeared and nothing contradicts the claim, but the claim itself is an unverified industry estimate; PH's Motion Systems segment is the structural proxy to monitor.

### PIL-3 — Manipulation reliability, not intelligence, gates deployment — VERDICT: supported

**wrong_if:** `metric=humanoid_mtbf_hours_in_commercial_deployment threshold=>2000 source=company_disclosure_or_fleet_operator op=>`

**Falsifier test result: NOT TRIGGERED** — no company or fleet operator discloses a humanoid MTBF at all, let alone one above 2,000 hours. The disclosure that would falsify the pillar does not exist anywhere in the six-name corpus, including ISRG.

**Best evidence found:**
- **ISRG (the reliability benchmark's own non-disclosure):** after 25+ years, >13M cumulative Xi procedures (https://agentii.ai/v/ISRG/ect75/page1), and ~13k installed systems, ISRG publishes no MTBF, uptime, or failure-rate metric anywhere in its 10-K/10-Q/transcripts; reliability appears only as a design goal (https://agentii.ai/v/ISRG/ect75/page1). The only quantitative reliability-adjacent metric is utilization (procedures/system/year): +3% FY2025, +3% Q2 2026 (https://agentii.ai/v/ISRG/sec166/page69, https://agentii.ai/v/ISRG/sec172/page32). Even the leader runs a human service layer around reliability — 24/7 support, proactive health monitoring, OnSite (https://agentii.ai/v/ISRG/sec166/page11): reliability is a serviced, fleet-level property, not a published spec.
- **TSLA (the only disclosed humanoid programme — management corroboration):** two independent statements name reliability, not model capability, as the gate: robotaxi scaling constrained by "the March of 9s of reliability... Ideally, you want 99.999% reliable" — "the only thing really constraining our growth in robotaxi" (https://agentii.ai/v/TSLA/ect61/4); and "if we injure even one person... regulators will immediately clamp down on our activities" (https://agentii.ai/v/TSLA/ect61/1). Optimus "needs to be out in the field and not break down" (https://agentii.ai/v/TSLA/ect61/1). Capability exists (FSD v14 in production, v15 tracks merged) while deployment is throttled — capability ≠ deployment. No quantitative MTBF disclosed for either program.
- **AMZN (production-scale counterexample in structured environments):** 1M+ warehouse robots with the manipulation sub-fleet (Cardinal, Sparrow arms) doubling in 2026, and measurable payback — fulfillment intensity 15.4% → 15.2% of net sales (https://agentii.ai/v/AMZN/ect83/2, https://agentii.ai/v/AMZN/sec131/25). Manipulation reliability has cleared the gate in semi-structured settings, reinforcing that the residual gate is unstructured-environment reliability. No per-task reliability metrics disclosed; warehouse automation is not humanoids (plan risk note 3).
- **NVDA (compute-side calibration):** the deployment-gate shock that has materialized in AI is regulatory, not reliability — the $4.5B H20 charge against $119B supply commitments (https://agentii.ai/v/NVDA/sec169/10) — a different gate, but the same structural lesson: gates land on the balance sheet of whoever holds forward supply.

**Verdict: supported** — falsifier untriggered; the gating premise is corroborated by the actors themselves (TSLA) and by the reliability leader's non-disclosure pattern (ISRG). Caveat: no quantitative humanoid MTBF exists to measure against the 2,000h threshold — the verdict rests on gating-premise evidence, not on an MTBF observation.

### PIL-4 — The 'GPT-3.5 moment' arrives late 2027 through 2028 — VERDICT: supported

**wrong_if:** `metric=general_purpose_humanoid_commercial_units_deployed threshold=>10000 source=company_and_fleet_disclosures` (a commercially deployed, general-purpose humanoid fleet at scale before 2027-Q4 falsifies it)

**Falsifier test result: NOT TRIGGERED** — zero commercial general-purpose humanoid units are disclosed by any company in the corpus. TSLA's own filings state "We have yet to commercialize Bots" (https://agentii.ai/v/TSLA/sec253/21) and describe a "nascent industry that has yet to develop commercially" (https://agentii.ai/v/TSLA/sec253/20); no other name discloses a humanoid deployment at all.

**Best evidence found:**
- **TSLA (the only filed humanoid timeline):** starter production late Jul-Aug 2026 (https://agentii.ai/v/TSLA/ect60/3); initial S-curve "quite flat and long" across "10,000 unique items" (https://agentii.ai/v/TSLA/ect61/1, https://agentii.ai/v/TSLA/ect60/3); "useful outside of Tesla sometime next year" (2027) (https://agentii.ai/v/TSLA/ect60/1); second factory (Giga Texas) ~summer 2027 (https://agentii.ai/v/TSLA/ect60/1); first builds go to Optimus Academy data collection, not customers (https://agentii.ai/v/TSLA/sec258/9). The "1 million bots delivered" CEO-award milestone (https://agentii.ai/v/TSLA/sec253/86) and the "10 million units a year" Optimus 4 aspiration (https://agentii.ai/v/TSLA/ect61/5) are promotional and excluded from the verdict (plan risk note 2).
- **ISRG (deployment-curve floor rate):** ~25 years to reach ~12–13k systems at ~1.7–2.0k placements/year (https://agentii.ai/v/ISRG/sec166/page69); the dv5 generational-compute transition reached ~1.7k units in ~2 years. A >10,000-unit humanoid fleet by 2027-Q4 would require a deployment curve roughly 6x faster than the most successful surgical-robot platform transition on record, in a less-proven application. Hardware cycles are multi-year S-curves (7-year Xi precedent — https://agentii.ai/v/ISRG/ect75/page5), and deployment-cost deflation arrives via tiering and cost-per-use (extended-use instruments from H1 2027), not list-price collapse (https://agentii.ai/v/ISRG/ect75/page2).
- **AMZN (robotics sequencing):** greenfield-only (Shreveport, 2024) → fleetwide retrofit mandate (2026) is a ~2-year bridge (https://agentii.ai/v/AMZN/ect77/4, https://agentii.ai/v/AMZN/ect82/2) — warehouse automation, not humanoids (plan risk note 3) — but the pattern implies capex intensity concentrates in years 2–4 of a deployment wave.
- **SPCX (upstream leading indicator):** compute-led capex — H1 2026 capex $28.5B (+309% YoY), AI segment 82.7% (https://agentii.ai/v/SPCX/sec8/9, https://agentii.ai/v/SPCX/sec8/30); nameplate compute 0.4 → 1.4 GW (https://agentii.ai/v/SPCX/sec8/36); $6.7B of cloud contracts signed in early Q3 2026 on 6-month terms (https://agentii.ai/v/SPCX/ect1/3). The infrastructure for the 2027–2028 window is being capitalized now, while the deployment-rate analogue (launches, mass to orbit) is flat-to-down — growth is compute-led, not launch-led (https://agentii.ai/v/SPCX/sec8/35). One-quarter issuer; treat forward compute targets as promotional (plan risk note 7).
- **NVDA (compute-platform readiness):** VeraRubin production shipments begin Q3 2026 — the compute side is ready ahead of the window (https://agentii.ai/v/NVDA/ect81/1); Uber robotaxi fleet targeted across ~30 cities and 4 continents by 2028 (https://agentii.ai/v/NVDA/ect81/1).

**Verdict: supported** — falsifier untriggered (zero commercial units exist, so a >10,000-unit fleet before 2027-Q4 cannot exist), and five independent disclosure sets each place first meaningful scale in late-2027/2028. Disclosed unit-count and aspiration claims are promotional and excluded (plan risk note 2).

---

## 2. Capability timeline (the thesis's headline output)

**GPT-3.5 moment estimate: 2027-Q4 to 2028-Q2** — an interval with a confidence band, never a point estimate. **Confidence: medium.**

| Phase | Evidence anchors (citations carried from artifacts) |
|---|---|
| **2026 H2 — compute and data infrastructure completes** | VeraRubin ships Q3 2026 (https://agentii.ai/v/NVDA/ect81/1); Optimus starter production late Jul-Aug 2026, first builds → data collection (https://agentii.ai/v/TSLA/ect60/3, https://agentii.ai/v/TSLA/sec258/9); AMZN robotic-arm fleet doubles in 2026 (https://agentii.ai/v/AMZN/ect83/2); SPCX compute draw 1.4 GW with ~$18B/quarter capex run-rate (https://agentii.ai/v/SPCX/sec8/36, https://agentii.ai/v/SPCX/ect1/4); TSLA 2026 capex >$20B → >$25B including the Optimus factory (https://agentii.ai/v/TSLA/ect59/2, https://agentii.ai/v/TSLA/sec259/30) |
| **2027 H1 — capacity and cost-curve preparation** | Giga Texas Optimus plant ~summer 2027; "useful outside Tesla" sometime 2027 (https://agentii.ai/v/TSLA/ect60/1); ISRG extended-use instruments H1 2027 — the cost-per-use deflation template (https://agentii.ai/v/ISRG/ect75/page2); Rubin ramping (https://agentii.ai/v/NVDA/sec173/33) |
| **2027-Q4 to 2028-Q2 — the band (headline output)** | First meaningful Optimus scale per the flat-and-long S-curve and "no significant production volume until end of 2026" (https://agentii.ai/v/TSLA/ect61/1, https://agentii.ai/v/TSLA/ect59/3); deployment-cost inflection via tiering + cost-per-use per the ISRG template (https://agentii.ai/v/ISRG/ect75/page2); SPCX 6-month cloud contracts (from Oct 2026) absorbing compute capacity (https://agentii.ai/v/SPCX/ect1/3) |
| **2028+ — fleet formation** | Uber robotaxi fleet ~30 cities / 4 continents by 2028 (https://agentii.ai/v/NVDA/ect81/1); NVDA "physical AI third wave" 5-year framing, directional and undated (https://agentii.ai/v/NVDA/ect81/5) |

**Band rationale.** The lower bound (2027-Q4) is set by TSLA's own filed statements — no significant production volume before end-2026, external usefulness in 2027, second factory summer 2027 — and by the falsifier design itself (a >10,000-unit fleet before 2027-Q4 falsifies PIL-4; nothing in the corpus suggests that is possible). The upper bound (2028-Q2) reflects the deployment-cost deflation mechanism (ISRG tiering/cost-per-use) and the capex absorption cycle (SPCX contract-backed compute). **Confidence is medium, not high**, because: (1) every timing input is company disclosure with promotional bias (plan risk note 2); (2) no unit-cost data exists anywhere, so an inflection cannot be measured as it arrives; (3) ISRG and AMZN are analogue curves, not humanoid data; (4) the falsifier is untriggered only because no units exist at all — the negative evidence is absence, not measurement.

---

## 3. Cross-ticker evidence table

Headline [FACT] numbers per ticker, with agentii.ai/v/ citations carried from the artifacts. No new citations; where an artifact has no number, none is added.

| Ticker | Headline [FACT] | Value | Citation |
|---|---|---|---|
| NVDA | FY2026 revenue | $215.9B (+65%) | https://agentii.ai/v/NVDA/sec169/37 |
| NVDA | Q1 FY2027 revenue | $81.6B (+85% YoY) | https://agentii.ai/v/NVDA/sec173/21 |
| NVDA | Data Center Q1 FY2027 / FY2026 | $75.2B (+92%) / $193.7B (90% of revenue) | https://agentii.ai/v/NVDA/sec173/21 ; https://agentii.ai/v/NVDA/sec169/79 |
| NVDA | Edge Computing (contains robotics) Q1 FY2027 | $6.4B (+29%) | https://agentii.ai/v/NVDA/sec173/21 |
| NVDA | Physical AI revenue (LTM) | >$9B | https://agentii.ai/v/NVDA/ect81/1 |
| NVDA | Manufacturing/supply/capacity commitments | $119B (Apr 26, 2026) | https://agentii.ai/v/NVDA/sec173/16 |
| NVDA | VeraRubin production shipments | Q3 2026 (POs in hand) | https://agentii.ai/v/NVDA/ect81/1 |
| NVDA | China Hopper shipments Q1 FY2027 | $0 (vs $4.6B a year earlier) | https://agentii.ai/v/NVDA/sec173/25 |
| ISRG | FY2025 revenue / procedures / installed base | $10,064.7M (+21%) / 3,153k (+18%) / 11,106 da Vinci (+12%) | https://agentii.ai/v/ISRG/sec166/page69 |
| ISRG | Utilization (only quantitative reliability proxy) | +3% FY2025; +3% Q2 2026 | https://agentii.ai/v/ISRG/sec166/page69 ; https://agentii.ai/v/ISRG/sec172/page32 |
| ISRG | Recurring revenue share | 84% FY2025 ($8,465.3M); 85% Q2 2026 | https://agentii.ai/v/ISRG/sec166/page78 |
| ISRG | I&A revenue / per procedure | $6,018.9M FY2025; $900–3,700 per procedure (range); ~$1.83K Q2 2026 | https://agentii.ai/v/ISRG/sec166/page77 ; https://agentii.ai/v/ISRG/ect75/page2 |
| ISRG | da Vinci ASP trajectory | ~$1.50M (2024) → $1.60M (2025) → $1.66M (H1 2026) | https://agentii.ai/v/ISRG/sec166/page78 ; https://agentii.ai/v/ISRG/sec172/page40 |
| ISRG | dv5 compute vs Xi / dv5 placements | >10,000x / 870 FY2025, 246 Q2 2026 | https://agentii.ai/v/ISRG/sec166/page8 ; https://agentii.ai/v/ISRG/sec166/page69 |
| ISRG | MTBF disclosure | None anywhere (negative finding) | https://agentii.ai/v/ISRG/ect75/page1 |
| TSLA | FY2025 revenue / R&D | $94,827M (−3%) / $6,411M (+41%) | https://agentii.ai/v/TSLA/sec253/page36 ; https://agentii.ai/v/TSLA/sec253/page44 |
| TSLA | Commercial Bots status | "We have yet to commercialize Bots" (10-K) | https://agentii.ai/v/TSLA/sec253/21 |
| TSLA | Optimus production timeline | Late Jul-Aug 2026 (Fremont); Giga Texas plant ~summer 2027 | https://agentii.ai/v/TSLA/ect60/3 ; https://agentii.ai/v/TSLA/ect60/1 |
| TSLA | Optimus unit economics | None disclosed (BOM/cost/price absent) | https://agentii.ai/v/TSLA/sec253/36 |
| TSLA | FSD data asset / subscriptions / deferred revenue | ~17.2B cumulative miles / 1.48M active / $4.05B | https://agentii.ai/v/TSLA/sec258/11 ; https://agentii.ai/v/TSLA/sec258/8 ; https://agentii.ai/v/TSLA/sec259/10 |
| TSLA | Unsupervised robotaxi miles | 380,000+, zero notable incidents | https://agentii.ai/v/TSLA/ect61/3 |
| TSLA | Training compute | Cortex 1+2 >205 MW; ~400 MW planned Dec-2026 | https://agentii.ai/v/TSLA/sec258/10 |
| TSLA | 2026 capex | FY2025 actual $8.53B → >$20B guided (Q4 call) → >$25B (10-Q) | https://agentii.ai/v/TSLA/sec253/36 ; https://agentii.ai/v/TSLA/ect59/2 ; https://agentii.ai/v/TSLA/sec259/30 |
| TSLA | Reliability gate (management) | "March of 9s... 99.999%" — "the only thing really constraining" | https://agentii.ai/v/TSLA/ect61/4 |
| AMZN | Robots in fulfillment network | >1,000,000 (Feb 2026) | https://agentii.ai/v/AMZN/ect81/5 |
| AMZN | Robotic arms (Cardinal, Sparrow) 2026 | More than double the fleet | https://agentii.ai/v/AMZN/ect83/2 |
| AMZN | FY2025 net sales / cash capex | $716.9B (+12%) / $128.3B (vs $77.7B) | https://agentii.ai/v/AMZN/sec131/69 ; https://agentii.ai/v/AMZN/sec131/23 |
| AMZN | H1 2026 cash capex | $96.3B (Q2 alone $53.1B) | https://agentii.ai/v/AMZN/sec177/27 |
| AMZN | Segment P&E net additions FY2025 | NA (fulfillment) $35.9B vs AWS $96.5B | https://agentii.ai/v/AMZN/sec131/70 |
| AMZN | Fulfillment intensity | $109.1B = 15.2% of net sales (vs 15.4%) | https://agentii.ai/v/AMZN/sec131/25 |
| AMZN | "robot" in FY2025 10-K | Zero hits (negative finding) | — (keyword scan, sec131) |
| PH | Motion Systems revenue | $3,580M FY2026 / $3,341M FY2025 / $3,706M FY2024 | https://agentii.ai/v/PH/sec166/44 |
| PH | Total net sales FY2026 | $21,499M | https://agentii.ai/v/PH/sec166/23 |
| PH | Segment operating margins | DI 23.8% / Aerospace 26.0%; consolidated GM 37.7% | https://agentii.ai/v/PH/sec166/25 ; https://agentii.ai/v/PH/sec166/26 ; https://agentii.ai/v/PH/sec166/23 |
| PH | Backlog (record) | $12.8B (Jun 30, 2026) | https://agentii.ai/v/PH/sec166/5 |
| PH | Rare-earth sourcing | "limited number of suppliers" (qualitative only) | https://agentii.ai/v/PH/sec166/11 |
| PH | Robotics disclosure | Zero "robot" hits in 10-K and both transcripts (negative finding) | — (keyword scans, sec166/ect72/ect71) |
| SPCX | H1 2026 revenue | $12,508M | https://agentii.ai/v/SPCX/sec8/13 |
| SPCX | H1 2026 capex | $28,476M vs $6,965M (+309%) | https://agentii.ai/v/SPCX/sec8/9 |
| SPCX | AI segment share of capex | 82.7% H1 / 86.2% Q2 2026 | https://agentii.ai/v/SPCX/sec8/30 ; https://agentii.ai/v/SPCX/sec8/31 |
| SPCX | Nameplate compute draw | 0.4 GW → 1.4 GW YoY | https://agentii.ai/v/SPCX/sec8/36 |
| SPCX | Servers & networking equipment | $22,694M → $34,771M in six months | https://agentii.ai/v/SPCX/sec8/14 |
| SPCX | Contracted cloud demand | +$1.6B Q2 2026; +$6.7B contracted early Q3 2026 | https://agentii.ai/v/SPCX/sec8/44 ; https://agentii.ai/v/SPCX/ect1/3 |
| SPCX | Deployment-rate analogue | Falcon launches 77 H1 2026 (vs 81); mass to orbit 485t (vs 652t) | https://agentii.ai/v/SPCX/sec8/35 |

---

## 4. Coverage gaps (aggregated from the artifacts)

**Universe-level gaps:**
1. **No embodied-data volumes disclosed anywhere** in the six-name corpus — no dataset hours, teleoperation hours, episodes, or synthetic-data volumes (NVDA, TSLA, ISRG, AMZN, PH all silent). PIL-1's magnitude test requires industry-technical sources beyond SEC filings; the retrieval scope cannot reach them.
2. **No MTBF disclosed anywhere**, including ISRG (the only US-listed company with a decade of surgical-robot reliability disclosure). ISRG's utilization (+3%) and I&A-per-procedure are the only quantitative reliability proxies in the corpus.
3. **No humanoid BOM split or teardown anywhere.** PIL-2's 40–70% actuator / 10–15% compute split is an industry estimate; TSLA discloses no Optimus BOM/cost/price; ISRG discloses no BOM-level cost cut; PH discloses no content-per-platform dollars; AMZN's robotics is vertically integrated with no component-supplier disclosure.
4. **No commercial humanoid units disclosed by anyone.** TSLA discloses no Optimus unit counts or revenue; NVDA's robotics sits undifferentiated inside Edge Computing ($6.4B).

**Ticker-level gaps (as declared by the artifacts):**
5. **AMZN is warehouse automation, not humanoids** (plan risk note 3): its evidence bears on deployment economics only; the word "robot" appears zero times in the FY2025 10-K — fleet metrics (>1M robots, arm doubling) live only in earnings-call transcripts.
6. **PH has zero robotics disclosure**: zero "robot" hits in the FY2026 10-K and the Q3/Q4 FY2026 transcripts; no quantitative rare-earth/magnet sourcing data; no platform-level COGS or margin for Motion Systems; no supplier names. The largest listed actuator franchise does not yet claim a humanoid revenue stream — the single most important PIL-4 negative evidence.
7. **SPCX is a one-quarter issuer**: a single 10-Q (2026-08-04) plus 8-Ks; no multi-year history; no named GPU/ASIC/memory/power suppliers in filings (NVIDIA is transcript-only); supplier contracts carry no long-term binding purchase orders. Forward compute targets (>2 GW end-2026, 10 GW end-2027) are promotional (plan risk note 7).
8. **NVDA**: no robotics standalone revenue; no embodied-data quantities; no China outlook beyond "no China data-center compute revenue"; Q2 FY2027 10-Q not yet filed (corpus one quarter stale for near-term risk reads).
9. **TSLA**: no per-unit economics for Optimus or FSD (no churn/MRR); no quantitative reliability metrics (miles-per-incident, MTBF); robotaxi fleet size disclosed only qualitatively; H2 2026 filings absent.
10. **ISRG**: no I&A standalone gross margin; no CAC/payback per hospital; Q2 2026 10-Q citation_ids not surfaced by search_documents (quarterly data cited via transcript + XBRL).

---

## 5. Data-quality flags surfaced by the agents

1. **PH `get_segment_data` conflict**: gold reports Motion Systems FY2025 $3,830M vs 10-K $3,341M (and Aerospace FY2025 operating income $854M vs 10-K $1,441M) — gold's product-axis rows appear stale or mis-mapped; **10-K values used throughout**.
2. **AMZN fiscal-calendar registry mismatch**: gold registry returns FY-end month 2 for AMZN, but the 10-K is for the fiscal year ended Dec 31, 2025; fiscal-year-filtered XBRL queries returned empty, so calendar-dated facts and filing text were used.
3. **NVDA `RevenueFromContractWithCustomerExcludingAssessedTax` untagged**: empty result set; revenue verified via consolidated plus dimensioned `Revenues` facts (OperatingSegments/ProductOrService axes).
4. **ISRG / TSLA / PH / SPCX single revenue concept**: `us-gaap:Revenues` (and `...IncludingAssessedTax`) return zero facts for each; P2.1 two-concept verification was handled by triangulation — same concept across two fiscal years and dimensions, reconciled to 10-K income-statement and MD&A tables (PH additionally triangulated via `CostOfGoodsAndServicesSold` reproducing the 37.7% gross margin).
5. **AMZN XBRL revenue/capex concepts empty**: `us-gaap:Revenues` and `PaymentsToAcquirePropertyPlantAndEquipment` return no AMZN facts (AMZN custom taxonomy not loaded in the store); values taken from 10-K/10-Q text pages and earnings calls.
6. Additional flags: NVDA capex concept `PaymentsToAcquirePropertyPlantAndEquipment` is stale (last used 2020; current series is `PaymentsToAcquireProductiveAssets`); TSLA XBRL `DeferredRevenue` empty (FSD deferred revenue $4.05B taken from 10-Q Note 1 text); TSLA `search_sec_filings` shows 0 records (discovery via `search_documents`/`list_sources`); ISRG fiscal-calendar returns FY-end month 1 inconsistent with calendar-year reporting; TSLA FSD cumulative-miles chart values post-Jun-2024 extraction-flagged as visually estimated (~17.2B approximate); an un-attributed $71M `LossContingencyDamagesAwardedValue` XBRL fact (TSLA, Q1 2026 10-Q) was excluded by the agent.

---

## 6. Contract compliance (output-schemas.md §2 requires)

- **falsifier_evidence**: every `pillar_verdicts` entry above is backed by a stated falsifier test result in §1 (PIL-1: untestable — metric uncomputable; PIL-2: not triggered — no evidence exists; PIL-3: not triggered — no MTBF disclosed; PIL-4: not triggered — zero disclosed commercial units).
- **no_verdict_inflation**: PIL-1 and PIL-2 are held at `indeterminate` despite directional support — no unsupported pillar was upgraded. PIL-3 and PIL-4 are `supported` strictly on the evidence stated.
- **interval_estimate**: the capability timeline carries an explicit interval (2027-Q4 to 2028-Q2) with a stated confidence band (medium), never a point estimate (plan risk note 2).
