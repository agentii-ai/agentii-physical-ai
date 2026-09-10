---
artifact_id: "002-cross-profit-pool-map-20260911"
thesis_id: "002-value-chain-profit-pool-map"
type: cross_synthesis
tickers_covered: [NVDA, PH, ISRG, TSLA, AMBA, CGNX, SPCX]
pillars_synthesized: [PIL-1, PIL-2, PIL-3]
pillar_verdicts:
  # PIL-1 is a conjunction. Tested halves reported separately (contracts §2 falsifier_evidence):
  #   PIL-1b (motion_model_gm_gap_change_pp < -10 falsifies): TESTED — no pair breaches -10pp
  #   (PH +3.5pp, ISRG +2.2pp, AMBA +0.4pp, TSLA 0.0pp, CGNX -3.3pp worst). NOT falsified —
  #   durability half supported.
  #   PIL-1a (actuation_plus_sensing_share_of_bom_pct < 55 falsifies): UNTESTABLE — no BOM
  #   disclosure exists anywhere in the corpus; the teardown range 51-88% (actuators 40-70% +
  #   sensing 11-18%) straddles the 55% threshold. Range reported, never a point estimate
  #   (risk note 7). One leg untested => conjunction cannot be marked supported
  #   (contracts §2 no_verdict_inflation).
  PIL-1: indeterminate
  # PIL-2 (nonchina_to_china_humanoid_bom_cost_ratio < 2.0 falsifies): UNMEASURABLE — proxy-only
  # per clarify round-3 rule; Deviation Register entry, expiry 2026-10-10. Directional proxies
  # (PH rare-earth disclosure NEW in FY2026 10-K; NVDA "effectively foreclosed", China share
  # 20.2%->9.1%->5.6%; AMBA BIS Entity List customers + WT 70%; CGNX dual-country footprint)
  # consistent with the premise but quantify nothing. No BOM cost data anywhere in the corpus.
  PIL-2: indeterminate
  # PIL-3 (model_layer_revenue_per_deployed_unit_usd > 5000 falsifies): TESTED on the narrow
  # reading per clarify round-3 named examples (model-layer revenue = STANDALONE digital
  # subscription/software revenue). ISRG My Intuitive+ "not material" => ~$0/unit; PH null
  # case (0 subscription hits). NOT falsified. Standing IC ambiguity recorded in body: service
  # contracts ($95-225K/system/yr, realized $129.9K) would exceed the threshold 19-45x under
  # the inclusive reading — verdict uses the narrow reading per the round-3 record.
  PIL-3: supported
constitution_pin: "1.3.0"
as_of: 2026-09-11
profit_pool_map:
  layer_rankings:
    - rank: 1
      layer: compute/model
      tickers: [NVDA]
      durable_margin_evidence: "GM 75.0% (FY25) -> 71.1% (FY26, Hopper->Blackwell mix + $4.5B H20 charge) -> 74.9% (Q1-FY27) — full recovery; 64.5% FY2026 segment operating margin; demand-constrained pricing stability. The layer to beat."
    - rank: 2
      layer: integrated systems
      tickers: [ISRG]
      durable_margin_evidence: "Product GM 65.7 -> 67.2 -> 66.3 (1.5pp stability band through $63.0M tariff hit and da Vinci 5 ramp); 84-85% recurring revenue; ASP rising $1.50M -> $1.60M -> $1.66M; razor-blade consumables ~$1,826/procedure."
    - rank: 3
      layer: sensing
      tickers: [AMBA, CGNX]
      durable_margin_evidence: "Bifurcated: AMBA 60.4 -> 60.5 -> 59.2 (-1.2pp, stable through +72.5% growth; design-in stickiness); CGNX 71.8 -> 68.4 -> 66.9 (-4.9pp, steepest erosion in corpus: E&O charge, mix, tariffs, ~1.2pp Moritex amortization)."
    - rank: 4
      layer: motion/actuation
      tickers: [PH, TSLA]
      durable_margin_evidence: "PH GM 35.8 -> 36.9 -> 37.7 (+1.9pp; ex-IEEPA 37.3); DI margin +100bps 'primarily driven by favorable pricing'; FY2031 target raised +300bps to 30%; Motion Systems +7.2% YoY but -3.4% below FY2024, platform margin undisclosed. TSLA automotive analogue 19.4 -> 18.4 -> 17.8 (-1.6pp) on ~$34.9K unit cost. Lowest level, most improving durability."
    - rank: 5
      layer: demand
      tickers: [SPCX]
      durable_margin_evidence: "H1-2026 capex $28,476M at 82.7% AI share; 1.4GW nameplate compute draw (3.5x YoY); $47.5B backlog. The pool's demand side — no margin pool of its own in this corpus."
  china_cost_ratio_estimate: null   # unmeasurable from corpus; interval-or-null contract (contracts §2 interval_estimate)
  confidence: medium
---

# Cross-Stock Synthesis — Value Chain Profit Pool Map (T-020)

**Scope**: synthesis of 19 decomposition artifacts (PH ×6, ISRG ×6, NVDA ×2, AMBA ×2, CGNX ×1, SPCX ×1, TSLA ×1), all pinned 2026-09-11, constitution 1.3.0. No retrieval calls made in this step; every number below carries its citation from the artifacts. Citation form: all `agentii.ai/v/{TICKER}/{citation_id}/{page}` links, written `TICKER/secNNN/pN` for compactness in tables.

---

## Executive Summary

Across the 7-ticker corpus the compute/model layer remains the profit-pool benchmark: NVDA's 71.1% FY2026 gross margin recovered fully to 74.9% (Q1-FY27), and no motion/sensing series breaches the PIL-1b gap-change falsifier — the motion-vs-model gap narrowed or held flat in every pair (PH +3.5pp; CGNX −3.3pp, worst). Motion durability is improving (PH GM 35.8→37.7%; DI margin +100bps on pricing; 30% FY2031 target), ISRG holds 66.3% product GM on 84% recurring revenue, and sensing is bifurcated (AMBA stable ~60%; CGNX eroding −4.9pp). PIL-1a is unresolvable: no BOM disclosure exists anywhere, and the teardown range (51–88%) straddles 55%. PIL-2's China-cost ratio is unmeasurable (proxy-only, deviation-registered). PIL-3 survives the narrow reading: standalone digital-subscription revenue is ≈$0/unit (ISRG "not material"; PH null), with the service-contract ambiguity (19–45× threshold) recorded for the IC. Verdicts: PIL-1 indeterminate, PIL-2 indeterminate, PIL-3 supported.

---

## 1. The Four Falsifier Tests

### Falsifier PIL-1a — `actuation_plus_sensing_share_of_bom_pct < 55` falsifies

**Evaluation rule (clarify round 3)**: BOM-share evidence is SEC-filing-derived only; teardown figures enter as `[VIEW]` with origin stated.

Filing proxies:

- **PH Motion Systems $3,580M FY2026 = 16.7% of consolidated sales** (series $3,706M → $3,341M → $3,580M, FY2024→FY2026) [FACT] PH/sec166/44. This is a share-of-sales proxy, not a BOM share: PH manufactures motion-control systems and components in-house across 323 plants (35 US states, 43 countries) [FACT] PH/sec166/19, so its actuation content is vertically internalized; external supplier reliance is confined to specialty inputs (rare earths, specialty electronics, super alloys) [FACT] PH/sec166/11.
- **ISRG product-COGS intensity 33.7% of product revenue FY2025** — the only quantified cost-stack cut in the entire 7-ticker corpus [DEDUCTED] ISRG/sec166/77 + /79. As a ceiling proxy: the entire product cost stack is 33.7% of revenue; actuation-heavy content (instruments & accessories) is 70.9% of product revenue [DEDUCTED] ISRG/sec166/77. Direction-consistent at the revenue level, but a revenue-share proxy cannot measure a BOM share (flagged by the ISRG unit-economics agent).
- **TSLA automotive as the labelled analogue**: ~$34,857 cost/vehicle FY2025 [DEDUCTED] TSLA/sec253/42 + /43; the COGS stack is enumerated qualitatively only (materials, labor, overhead, logistics, tariffs, warranty, FSD/connectivity maintenance) [FACT] TSLA/sec253/43; D&A is the sole numeric anchor at 5.5% of automotive-segment COGS [DEDUCTED] TSLA/sec253/98. No Optimus per-unit cost, BOM split, or price exists in any retrieved filing [FACT] TSLA/sec253 (absence).

**[VIEW] Industry teardown range** (macro-plan / T-001 origin, external reference): actuators 40–70% + sensing 11–18% = **51–88% of humanoid BOM**. The range **straddles the 55% threshold** — per risk note 7 this is reported as a range, never a point estimate.

**Result: UNTESTABLE → indeterminate (PIL-1a leg).** No BOM disclosure exists anywhere in the corpus, and the external range cannot resolve the threshold.

### Falsifier PIL-1b — `motion_model_gm_gap_change_pp < −10` falsifies

Gap = motion GM − NVDA GM (pp), computed at the earliest and latest like-for-like fiscal pairing in each series (pairing done by the decomposition agents; NVDA leg is the shared model-layer reference: 72.7% FY2024 → 71.1% FY2026).

| Pair (motion series vs NVDA) | Gap @ earliest (pp) | Gap @ latest (pp) | Δpp | vs −10pp |
|---|---|---|---|---|
| PH 35.8 → 37.7 vs 72.7 → 71.1 | −36.9 | −33.4 | **+3.5** | PASS (moves toward motion) |
| ISRG product 65.7 → 66.3 vs 72.7 → 71.1 | −7.0 | −4.8 | **+2.2** | PASS |
| AMBA 60.4 → 59.2 vs 72.7 → 71.1 | −12.3 | −11.9 | **+0.4** | PASS (flat) |
| CGNX 71.8 → 66.9 vs 72.7 → 71.1 | −0.9 | −4.2 | **−3.3** | PASS (worst; far from −10) |
| TSLA 19.4 → 17.8 vs 72.7 → 71.1 | −53.3 | −53.3 | **0.0** | PASS (flat) |

Series sources: PH PH/sec166/23 + /35; NVDA NVDA/sec169/51 + /37; ISRG ISRG/sec166/79; AMBA AMBA/sec106/72; CGNX CGNX/sec93/72; TSLA TSLA/sec253/43.

**Result: NOT FALSIFIED.** No pair breaches −10pp; four of five gaps move toward motion or hold flat, and CGNX's −3.3pp is one-third of the falsification threshold. Caveat noted honestly: PH FY2026 GM carries ~40bp of non-recurring IEEPA tariff-refund benefit [FACT] PH/sec166/23; on the ex-IEEPA 37.3% [DEDUCTED] PH/sec166/35 the PH gap change is still +3.1pp — the verdict is insensitive to the adjustment. **The durability half of PIL-1 is supported.**

### Falsifier PIL-2 — `nonchina_to_china_humanoid_bom_cost_ratio < 2.0` falsifies

**Evaluation rule (clarify round 3)**: proxy-only. The ratio itself is unmeasurable from the corpus — **no BOM cost data exists for any ticker** — and this remains registered as a Deviation Register entry (expiry 2026-10-10). The verdict is therefore honest: the falsifier can neither fire nor be cleared.

Proxy evidence carried from the artifacts:

- **PH** — the rare-earth "limited suppliers" risk-factor sentence ("rely on a limited number of suppliers for certain critical components, such as specialty electronics, rare earths, …") is **NEW in the FY2026 10-K** [FACT] PH/sec166/11; the FY2025 10-K carries no such sentence (0 keyword hits) [FACT] PH/sec127/11. The addition coincides with the FGC/CIRCOR acquisitions and is filing-linked to increased supply-concentration risk [FACT] PH/sec166/11. The $84M IEEPA refund recognized in Q4 FY2026 [FACT] PH/sec166/23 shows prior tariff absorption on China-linked imports.
- **NVDA** — "effectively foreclosed" from China's data-center compute market [FACT] NVDA/sec169/10; China revenue share 20.2% (FY2024) → 9.1% (FY2026) → 5.6% (Q1-FY27) [DEDUCTED] NVDA/sec169/78, sec173; **$0 China Hopper DC shipments in Q1-FY27 vs $4.6B year-ago** [FACT] NVDA/sec173/25; $4.5B H20 charge, ~$60M licensed H20 revenue, H200 25% import tariff, USG ≥15% revenue-share expectation [FACT] NVDA/sec169/10. China's compute layer is being served by domestic silicon — any China-side BOM cost advantage rests on non-NVDA compute stacks [VIEW] NVDA artifact.
- **AMBA** — BIS Entity List customers (Hikvision, Dahua, Shenzhen Dajiang Baiwang affiliates) with an explicit substitution runway [FACT] AMBA/sec105/35; WT Microelectronics 70% revenue concentration [FACT] AMBA/sec106/98 behind a Taiwan bill-to curtain (69.6% of revenue [DEDUCTED] AMBA/sec106/97); HiSilicon and Horizon Robotics as disclosed Chinese substitution competitors [FACT] AMBA/sec106/17; no mainland-China manufacturing [FACT] AMBA/sec106/17.
- **CGNX** — dual-country footprint: in-house optics in China and Vietnam, EMS assembly in Indonesia/Malaysia (neither in China) [FACT] CGNX/sec93/8 — existence proof that a non-China sensing supply chain operates at scale, but zero cost data; Greater China revenue 16% and declining under BIS controls [FACT] CGNX/sec93/25, /11.
- **ISRG** (context) — China-sourced rare-earth/magnet exposure plus Shanghai JV; 2025 China rare-earth export controls disclosed [FACT] ISRG/sec166/32.

**Result: UNMEASURABLE → indeterminate** (deviation-registered). The proxies are directionally consistent with a structural China cost/supply advantage but quantify nothing. `china_cost_ratio_estimate: null` per the interval-or-null contract.

### Falsifier PIL-3 — `model_layer_revenue_per_deployed_unit_usd > 5000` falsifies

**Adopted reading (per the clarify round-3 record's named examples): narrow** — model-layer revenue = **standalone digital subscription/software revenue**, not hardware-maintenance contracts with bundled software.

- **ISRG**: My Intuitive+ ("a digital subscription package available with the da Vinci 5 platform") [FACT] ISRG/sec166/11 and the whole digital portfolio (Case Insights, SimNow, 3D Models, Intuitive Learning) are disclosed as **"We do not currently generate material revenue from these offerings"** — stated twice, FY2025 10-K and Q2-2026 10-Q [FACT] ISRG/sec166/77, ISRG/sec172/38. Standalone digital revenue per deployed unit ≈ **$0** on 12,101 units [DEDUCTED] — decisively below the $5,000 threshold.
- **PH**: null case — "subscription" appears **0 times** in the entire FY2026 10-K [FACT] PH/sec166 (keyword search); the XBRL product axis contains hardware members only [FACT] PH revenue-decomp artifact. Model-layer revenue per deployed unit = **$0**.

**Result: NOT FALSIFIED → supported (narrow reading).**

**Standing ambiguity note for the IC (recorded, not resolved)** — the ISRG business-model/revenue-composition agent flagged: under the pillar's *inclusive* definition ("includes per-unit software/subscription revenue"), ISRG's service contracts — $95K–$225K per system-year, realized $129.9K/unit — are hardware-maintenance with bundled software upgrades [FACT] ISRG/sec166/77, /11 and would exceed the $5,000 threshold by **19–45×** (26× on realized). The verdict uses the narrow reading per the round-3 record's named examples; if the IC later adopts the inclusive reading, PIL-3 is **refuted** on ISRG alone.

**Immateriality zone**: the $5,000 threshold on 12,101 units crosses at only ~$60.5M/yr of software revenue; up to ~$100M (≈1% of ISRG revenue) could hide under "not material" [DEDUCTED] ISRG revenue-decomp artifact. The falsifier's detectability is materially weaker than the threshold suggests.

---

## 2. Layer Profit-Pool Map

Layers ranked by durable-margin evidence (evidence details in the `profit_pool_map.layer_rankings` frontmatter block):

1. **Compute/model (NVDA)** — 71.1% FY2026 GM with full recovery to 74.9% (Q1-FY27); the FY2026 dip was mix transition plus a one-off China-driven charge, not competitive erosion [FACT] NVDA/sec169/41; demand-constrained pricing stability [FACT] NVDA/sec173/24. **The layer to beat.**
2. **Integrated systems (ISRG)** — 66.3% product GM inside a 65.7–67.2% stability band; 84% recurring (85% Q2-26) [FACT] ISRG/sec166/78, sec172/40; rising ASPs.
3. **Sensing (AMBA, CGNX)** — AMBA ~60% stable (−1.2pp/3FY); CGNX 71.8→66.9 (**−4.9pp, steepest erosion in the corpus**, with ~1.2pp of it Moritex amortization and a $13M E&O one-off) [FACT]/[DEDUCTED] CGNX/sec93/72, /24, /25.
4. **Motion/actuation (PH + TSLA analogue)** — PH GM 35.8→37.7 rising; DI margin +100bps on pricing [FACT] PH/sec166/25; FY2031 target raised 300bps to 30% [FACT] PH/ect72/1. Lowest margin level, best-improving durability; platform-level margin undisclosed. TSLA automotive analogue 17.8% and shallowly declining.
5. **Demand (SPCX)** — $28.5B H1-2026 capex, 82.7% AI [FACT] SPCX/sec8/31; 1.4GW nameplate compute draw, 3.5× YoY [FACT] SPCX/sec8/36. A demand pool, not a margin pool.

**Honest tension with the thesis claim**: the durable-margin ranking places compute/model first, and SPCX shows end-market demand dollars flowing overwhelmingly to compute (82.7% AI share; one quarter of SPCX AI capex, $15.8B, is ~4.4× PH's entire FY2026 Motion Systems revenue [DEDUCTED] SPCX/sec8/30). The thesis claim — "dominant profit pool in actuation and sensing; compute commoditising" — is directionally supported by the PIL-1b gap dynamics (all gaps moving toward motion) but is **not confirmed at the level**: compute margins have fully recovered and are the corpus's highest. The claim survives only as a convergence trend, not a present fact.

---

## 3. Cross-Ticker [FACT] Table

Citations carried from the decomposition artifacts (form `agentii.ai/v/TICKER/secNNN/pN`).

### Motion / actuation

| Ticker | Metric | Value | Period | Citation |
|---|---|---|---|---|
| PH | Motion Systems revenue | $3,580M / $3,341M / $3,706M | FY26/25/24 | PH/sec166/44 |
| PH | Consolidated gross margin | 37.7% / 36.9% / 35.8%; ex-IEEPA 37.3% | FY26/25/24 | PH/sec166/23, /35 |
| PH | DI segment operating margin | 23.8% (vs 22.8%) — "primarily driven by favorable pricing" | FY26 | PH/sec166/25 |
| PH | Aerospace op margin / adjusted segment margin | 26.0% / 27.3% record; FY2031 target 30% (+300bps) | FY26 | PH/sec166/26, ect72/1 |
| PH | IEEPA tariff refund | $84M reduction to cost of sales | Q4 FY26 | PH/sec166/23 |
| PH | Rare-earth "limited suppliers" disclosure | NEW in FY2026 10-K; absent in FY2025 (0 hits) | FY26 | PH/sec166/11, sec127/11 |
| PH | Backlog | $12.8B; ~70% shippable within 12 months | 6/30/26 | PH/sec166/5 |
| PH | Non-US sales share | ~36% (risk factors) vs 33.1% implied (p44 table) — intra-filing basis gap ~2.9pp | FY26 | PH/sec166/10, /44 |
| TSLA | Automotive gross margin | 19.4% / 18.4% / 17.8% | FY23/24/25 | TSLA/sec253/43 |
| TSLA | Per-vehicle economics | $42,394 rev / $34,857 cost / $7,537 GP [DEDUCTED] | FY25 | TSLA/sec253/42, /43 |
| TSLA | D&A share of automotive-segment COGS | 5.5% | FY25 | TSLA/sec253/98 |
| TSLA | Optimus per-unit economics | none disclosed in any filing | all | TSLA/sec253 (absence) |

### Compute / model

| Ticker | Metric | Value | Period | Citation |
|---|---|---|---|---|
| NVDA | Consolidated gross margin | 72.7% / 75.0% / 71.1%; 74.9% Q1-FY27 | FY24/25/26 | NVDA/sec169/51, /37, sec173/27 |
| NVDA | Segment operating margin | 64.5% [DEDUCTED] | FY26 | NVDA/sec169/78 |
| NVDA | China revenue share | 20.2% → 19.2% → 9.1% → 5.6% [DEDUCTED] | FY24→Q1-FY27 | NVDA/sec169/78, sec173 |
| NVDA | H20 charge / licensed H20 revenue | $4.5B / ~$60M | Q1-FY26 / FY26 | NVDA/sec169/10 |
| NVDA | China Hopper DC shipments | $0 Q1-FY27 vs $4.6B Q1-FY26 | Q1-FY27 | NVDA/sec173/25 |
| NVDA | Supply/capacity commitments | $95.2B (2026-01-25) → $119B (2026-04-26) | FY26-end / Q1-FY27 | NVDA/sec169/70, sec173/16 |
| NVDA | Edge Computing revenue | $6,369M (+29% YoY; robotics/automotive/AI-RAN) | Q1-FY27 | NVDA/sec173/25 |
| NVDA | Top-3 direct customer share | 54% [DEDUCTED] | Q1-FY27 | NVDA/sec173/20 |

### Integrated systems

| Ticker | Metric | Value | Period | Citation |
|---|---|---|---|---|
| ISRG | Product gross margin | 65.7% / 67.2% / 66.3%; 67.9% Q2-26 (incl. $27.5M IEEPA refund) | FY23/24/25 | ISRG/sec166/79, sec172/41 |
| ISRG | Product COGS intensity | 33.7% of product revenue (only quantified cost-stack cut) [DEDUCTED] | FY25 | ISRG/sec166/77, /79 |
| ISRG | Revenue mix | I&A 59.8% / systems 24.6% / service 15.6% | FY25 | ISRG/sec166/77 |
| ISRG | Recurring revenue share | 84% (FY25); 85% (Q2-26) | FY25 / Q2-26 | ISRG/sec166/78, sec172/40 |
| ISRG | Installed base | 12,101 (FY25); 12,806 (Q2-26) | — | ISRG/sec166/69, sec172/32 |
| ISRG | Service contract range / realized | $95K–$225K/yr; $129.9K/unit realized [DEDUCTED] | FY25 | ISRG/sec166/77 |
| ISRG | System ASP | ~$1.50M → ~$1.60M → ~$1.66M | FY24→H1-26 | ISRG/sec166/78, sec172/40 |
| ISRG | I&A revenue per procedure | $1,826 (FY25) / $1,852 (Q2-26), combined da Vinci+Ion basis [DEDUCTED] | — | ISRG/sec166/69, /77, sec172/32, /38 |
| ISRG | Digital solutions revenue | "not material" (stated twice) | FY25 + Q2-26 | ISRG/sec166/77, sec172/38 |
| ISRG | Tariff impact on cost of revenues | $63.0M | FY25 | ISRG/sec166/65 |
| ISRG | Manufacturing headcount share | 44.8% [DEDUCTED] | FY25 | ISRG/sec166/25 |

### Sensing

| Ticker | Metric | Value | Period | Citation |
|---|---|---|---|---|
| AMBA | Gross margin | 60.4% / 60.5% / 59.2% | FY24/25/26 | AMBA/sec106/72 |
| AMBA | Revenue | $390.7M (+37.2% YoY) | FY26 | AMBA/sec106/53 |
| AMBA | WT distributor / Taiwan bill-to | ~70% / 69.6% of revenue | FY26 | AMBA/sec106/98, /97 |
| AMBA | BIS Entity List customers | Hikvision, Dahua, Shenzhen Dajiang Baiwang | FY25 10-K | AMBA/sec105/35 |
| AMBA | Robotics exposure | one warehouse-robotics production win; humanoid engagements "not in a place to talk about just yet" | FY26/27 | AMBA/ect53/3, ect54/4 |
| CGNX | Gross margin | 71.8% / 68.4% / 66.9% (−4.9pp/3FY) | FY23/24/25 | CGNX/sec93/72, /24 |
| CGNX | Revenue | $994.4M | FY25 | CGNX/sec93/59 |
| CGNX | Greater China share | 16% (declining; BIS impact disclosed) | FY25 | CGNX/sec93/25, /11 |
| CGNX | Non-US revenue share | 67% | FY25 | CGNX/sec93/8 |
| CGNX | Services share | <10% (all periods) | — | CGNX/sec93/24 |

### Demand

| Ticker | Metric | Value | Period | Citation |
|---|---|---|---|---|
| SPCX | Total capex | $28,476M (4.1× YoY) | H1-26 | SPCX/sec8/9 |
| SPCX | AI segment capex / share | $23,551M = 82.7%; Q2-26 86.2% vs 26.5% Q2-25 | H1-26 | SPCX/sec8/31, /30 |
| SPCX | Nameplate compute draw | 1.4GW (3.5× YoY) | 6/30/26 | SPCX/sec8/36 |
| SPCX | Tesla Megapack purchases | $329M | H1-26 | SPCX/sec8/30 |
| SPCX | Customers A / B revenue share | 17.9% / 12.2% | H1-26 | SPCX/sec8/14 |
| SPCX | Backlog | $47,461M | 6/30/26 | SPCX/sec8/14 |
| SPCX | XBRL tagging anomaly | RFCC $12,508M H1-26; us-gaap:Revenues = 0 facts | H1-26 | XBRL spcx-20260630.htm |

---

## 4. Coverage Gaps (aggregated across all 19 artifacts)

1. **`get_segment_data` gold regression**: returns `INTERNAL_ERROR: column "k" does not exist` on both attempts (PH supply-chain run). The T-001 gold-vs-filed conflict (gold $3,830M vs filed $3,341M for FY2025 Motion Systems) **could not be re-tested**; the filed side is re-confirmed at $3,341M [FACT] PH/sec166/44 and the 10-K-wins directive holds. Conflict stays flagged.
2. **No BOM disclosures anywhere**: zero cost-stack/BOM splits across all 7 tickers (PH, ISRG, TSLA, AMBA, CGNX, NVDA, SPCX). PIL-1a rests on revenue-level proxies (PH 16.7% share-of-sales; ISRG 33.7% COGS-intensity ceiling); PIL-2 rests on nothing quantitative. Teardown figures are `[VIEW]`-only per the round-3 rule.
3. **PIL-2 untestable** — Deviation Register entry, expiry 2026-10-10. `china_cost_ratio_estimate: null`.
4. **PH intra-filing geographic discrepancy**: risk factors state ~36% non-US sales [FACT] PH/sec166/10; the page-44 revenue table implies 33.1% [DEDUCTED] PH/sec166/44 — a ~2.9pp basis gap within one filing, both as filed.
5. **PH**: Motion Systems platform-level margin not disclosed; no quantitative direct:indirect channel split; no customer-level concentration percentage; no magnet-specific sourcing disclosure ("magnet" = 0 hits).
6. **TSLA**: no Optimus per-unit cost/BOM/price in any filing; automotive COGS enumerated qualitatively only; per-unit economics FY2025-only (prior-year deliveries not retrieved).
7. **ISRG**: no standalone software revenue line ("not material" only); "Intuitive Hub" no longer named in the FY2025 10-K digital portfolio; customer-level concentration not disclosed; registry `fiscal_year_end_month: 1` conflicts with Dec-31 filing year-end (calendar-year used); `sec_filings` source shows 0 records (retrieved via `src_documents`); per-procedure basis note: $1,826 combined-basis vs $1,909 da Vinci-only-basis.
8. **AMBA**: registry `fiscal_year_end_month: 3` vs Jan-31 filing header; no quantitative IoT/automotive split (80/20 rests on transcript statement AMBA/ect53/5); robotics design wins unquantifiable; inventory-days sourced from transcripts only.
9. **CGNX**: 4-4-5 Sunday quarter-ends vs MCP calendar-month quarter-ends (pair by XBRL `period_end`); recurring/software revenue not separately disclosed; contract manufacturers unnamed; no China-vs-non-China cost split.
10. **NVDA**: Q2-FY2027 10-Q not yet in corpus; AI-compute market share undisclosed; China domestic-vendor substitution unquantified; no supplier-concentration percentages.
11. **SPCX**: earnings-call transcript not retrievable (no citation_id in the Layer-1 index); GPU/OEM suppliers unnamed; no geographic revenue/sourcing disclosure; one-quarter corpus; XBRL tagging anomaly (revenue under RFCC only, `us-gaap:Revenues` = 0 facts) — downstream pipelines must key SPCX on RFCC.
12. **ISRG + PH map-append requests pending dispatcher**: `software_subscription_revenue_usd` (PH), `instruments_accessories_revenue_usd` / `systems_revenue_usd` / `service_revenue_usd` (ISRG), plus AMBA/TSLA new metrics — per entities.md §2 discipline, none were added by the decomposition agents.

---

## 5. T-001 Reconciliation

**Every re-tested T-001 baseline verified PASS; zero contradictions.** The only flagged items are (a) the PH gold-vs-filed conflict that the tool error prevented from re-testing (carried, not new) and (b) two precision/basis improvements, noted below.

| Ticker | T-001 baseline | Fresh retrieval | Status |
|---|---|---|---|
| PH | Motion Systems $3,580M FY2026 | $3,580M (XBRL detailed fact + 10-K p44) | PASS |
| PH | DI op margin 23.8% | 23.8% (p25; op income $3,440M bridge) | PASS |
| PH | Consolidated GM 37.7% | 37.7% (recompute 37.68%) | PASS |
| PH | Backlog $12.8B | $12.8B (segment sum $12,830M) | PASS |
| PH | FY2025 Motion Systems conflict side | filed $3,341M re-confirmed; gold side untestable (`column "k" does not exist`) | FLAGGED (carried) |
| ISRG | FY2025 mix I&A $6,018.9M / systems $2,473.7M / service $1,572.1M / total $10,064.7M | exact (XBRL authority-3) | PASS |
| ISRG | Recurring 84% | 84% FY25; 85% Q2-26 — update, not contradiction | PASS |
| ISRG | Installed base 12,101 | 12,101 (11,106 dv + 995 Ion) | PASS |
| ISRG | Product GM 66.3% / total GM 66.0% | exact (p79 / p69; income-statement recompute 66.25%) | PASS |
| ISRG | ASP $1.50M → $1.60M → $1.66M | exact trajectory (p78 / sec172 p40) | PASS |
| ISRG | ~45% manufacturing headcount | 44.8% (7,625/17,021) | PASS |
| ISRG | I&A per procedure ~$1.83K | $1,826 FY25 / $1,852 Q2-26 (combined-basis; da Vinci-only basis yields $1,909 — denominator note, not contradiction) | PASS |
| NVDA | FY2026 revenue $215,938M | exact (10-K + XBRL) | PASS |
| NVDA | FY2026 GM 71.1% | 71.07% recompute | PASS |
| NVDA | Edge $6.4B | $6,369M Q1-FY27 | PASS |
| NVDA | Supply commitments $119B | $119B = Q1-FY27 10-Q (2026-04-26); $95.2B = FY2026 year-end 10-K (2026-01-25). **Precision improvement (period attribution), not a contradiction.** | PASS |
| TSLA | FY2025 automotive GM 17.8%; revenue $69,526M; COGS $57,165M; per-vehicle $42,394/$34,857 | all reproduced exactly (p43 + XBRL authority-3) | PASS |
| SPCX | H1-2026 capex $28.5B; AI share 82.7% | $28,476M; 82.7% computed | PASS |
| SPCX | P2.1 anomaly (RFCC $12.508B vs Revenues=0) | verified verbatim — tagging anomaly, not absent revenue | PASS |

AMBA and CGNX carry no T-001 baseline set; their GM series were retrieved fresh with XBRL authority-3 verification and are consistent with the anchors referenced in T-001.

**Net reconciliation statement: zero contradictions introduced.** The two distinctions that could be misread as contradictions are (1) NVDA $119B vs $95.2B commitments — a fiscal-period attribution (10-Q Apr-2026 vs 10-K Jan-2026), and (2) ISRG $1,826 vs $1,909 per-procedure — a denominator-basis choice (combined da Vinci+Ion vs da Vinci-only). Both are precision improvements, recorded here for the IC.
