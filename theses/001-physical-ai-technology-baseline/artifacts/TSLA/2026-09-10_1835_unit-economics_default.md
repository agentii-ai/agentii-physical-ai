---
artifact_id: "001-TSLA-unit-economics-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: TSLA
skill: unit-economics
mode: default
affix: unit-economics
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "e87ee63269a2"
as_of: 2026-09-10
entity_claims:
  - "Optimus is 'a general purpose, autonomous humanoid robot' developed using Tesla's real-world AI data strengths (FY2025 10-K MD&A)"
  - "Fremont Model S/X line being converted to an Optimus factory with long-term goal of 1M units/year (Q4 2025 call)"
  - "Optimus production start targeted late July-August 2026; second Optimus factory at Giga Texas to start production ~summer 2027 (Q1 2026 call)"
  - "Optimus 4 (Austin) 'aspirationally 10 million units a year versus 1 million units a year of Optimus 3', much more vertically integrated (Q2 2026 call)"
  - "'1 million bots delivered' is operational milestone #3 of the 2025 CEO Performance Award (FY2025 10-K)"
  - "No Optimus per-unit cost, BOM breakdown, or price target disclosed in any retrieved SEC filing or transcript"
citations:
  - "sec253 (FY2025 10-K, filed 2026-01-29): p36, p37, p42, p43, p44, p55, p86"
  - "sec259 (Q2 2026 10-Q, filed 2026-07-23): p28, p29, p32"
  - "ect59 (Q4 FY2025 earnings call, 2026-01-28): p1, p2, p3"
  - "ect60 (Q1 FY2026 earnings call, 2026-04-22): p1, p3"
  - "ect61 (Q2 FY2026 earnings call, 2026-07-22): p1, p3, p5"
pillars_addressed: [PIL-2, PIL-4]
claim_state: pinned
key_metrics:
  FY2025_total_revenues_usd_bn: 94.827
  FY2025_total_gross_margin_pct: 18.0
  FY2025_automotive_gross_margin_pct: 17.8
  FY2025_automotive_revenue_usd_bn: 69.526
  FY2025_automotive_cogs_usd_bn: 57.165
  FY2025_deliveries_m: 1.64
  FY2025_revenue_per_vehicle_usd: 42394
  FY2025_cost_per_vehicle_usd: 34857
  FY2025_capex_usd_bn: 8.53
  FY2026_capex_guidance_usd_bn_gt: 20
  Q2_2026_total_gross_margin_pct: 16.8
  Q2_2026_automotive_gross_margin_pct: 16.9
  Q2_2026_total_revenues_usd_bn: 28.24
conclusions:
  - "TSLA discloses zero Optimus per-unit economics (no BOM, no cost/unit, no price target); Optimus is pre-revenue and pre-volume through Q2 2026, so PIL-2's BOM split cannot be validated against TSLA filings."
  - "The only Optimus cost-structure signal management discloses is compute: AI chips and memory are stated as the binding supply constraint (Terafab, Samsung/TSMC/Micron commentary), directionally consistent with compute being the scarce minority of BOM."
  - "Management's own timeline (starter production late Jul-Aug 2026, Giga Texas plant summer 2027, flat-and-long S-curve, 'useful outside Tesla' ~2027) aligns with PIL-4's 2027-Q4-2028 inflection window."
  - "Automotive per-unit economics (FY2025: ~$42.4K revenue, ~$34.9K cost, ~$7.5K gross profit per vehicle; 17.8% automotive GM) are the only filed unit-economics anchor but are a weak BOM analogue for humanoids."
  - "FY2026 capex guidance of >$20B (vs $8.53B actual FY2025), explicitly including 'the Optimus factory', marks the disclosed capacity-build phase for the PIL-4 window."
facts_count: 24
deducted_count: 5
views_count: 6
citation_count: 18
---

# TSLA — Unit Economics (default) | Thesis 001 Pillars PIL-2 & PIL-4

## 1. Executive Summary

Tesla discloses no per-unit economics for Optimus: no BOM, no cost per robot, no price target exists anywhere in the retrieved FY2025 10-K, 2025-2026 10-Qs, or the last three earnings calls https://agentii.ai/v/TSLA/sec253/36. What management does disclose is the cost *structure of the constraint set*: a supply chain that must be built "in its entirety" https://agentii.ai/v/TSLA/ect61/1, production scaling described as the hardest ramp in company history with "10,000 unique items" https://agentii.ai/v/TSLA/ect60/3, and AI compute explicitly named as the binding input — Terafab exists because Tesla "simply won't have enough AI chips" to scale Optimus https://agentii.ai/v/TSLA/ect61/1. Filed automotive unit economics provide the only hard per-unit anchor: FY2025 revenue of ~$42.4K and cost of ~$34.9K per vehicle on a 17.8% automotive gross margin https://agentii.ai/v/TSLA/sec253/42 https://agentii.ai/v/TSLA/sec253/43. The disclosed ramp timeline (production late Jul-Aug 2026, second plant summer 2027, flat-and-long S-curve) https://agentii.ai/v/TSLA/ect60/3 supports PIL-4's 2027-Q4-2028 inflection window, while PIL-2's 40-70% actuator-content claim remains untestable against filings — a coverage gap, not a contradiction.

## 2. Data Sources

- FY2025 Form 10-K (citation_id sec253, filed 2026-01-29): MD&A pages 36-37, revenue table p42, cost/gross-margin table p43, R&D p44, income statement p55, CEO award p86.
- Q2 2026 Form 10-Q (citation_id sec259, filed 2026-07-23): MD&A pages 28-29, cost/gross-margin table p32.
- Earnings call transcripts: ect59 (2026-01-28), ect60 (2026-04-22), ect61 (2026-07-22).
- XBRL facts: us-gaap:Revenues, us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax (second revenue concept per P2.1), us-gaap:CostOfRevenue, FY2025-FY2026.

## 3. Analysis

### 3.1 Optimus: disclosed cost-structure commentary (PIL-2)

[FACT] The FY2025 10-K frames Optimus as a development-stage "general purpose, autonomous humanoid robot" built on Tesla's real-world AI data strengths, with no segment revenue, unit counts, or cost disclosures for it anywhere in the filing https://agentii.ai/v/TSLA/sec253/37. [FACT] The Q2 2026 10-Q adds that Tesla is "making preparations and investments in large-scale production" for Optimus and explicitly lists Optimus among the manufacturing operations the company is expanding https://agentii.ai/v/TSLA/sec259/28 https://agentii.ai/v/TSLA/sec259/29.

[FACT] On the Q2 2026 call, Musk stated that for Optimus "there is no supply chain. So we've had to build up the supply chain in its entirety or in-house the production," and that "the production scaling challenge is very substantial... the initial portion of the S-curve will be quite flat and long" https://agentii.ai/v/TSLA/ect61/1. [FACT] He quantified the novelty: "everything on the robot is new," with ramp speed set by "10,000 unique items" — production "will move as fast as the least luckiest, lowest, dumbest part in the entire 10,000" https://agentii.ai/v/TSLA/ect60/3.

[FACT] On BOM composition, the only disclosed cost-stack commentary concerns electronics and compute: "Optimus has a lot of really specialized power electronics and circuit boards. It's all Tesla design... but it is fabricated by suppliers," while Optimus 4 (Austin) will be "much more vertically integrated... probably doing a lot of the sort of PCV [PCB] work in-house" https://agentii.ai/v/TSLA/ect61/5. [FACT] Supply-chain partners named for Optimus-specific categories include Samsung and TSMC — "putting in tens of billions of dollars... to build AI compute for Optimus and robotaxi" — and Micron, which gave Tesla "a very significant allocation on reasonable terms given the pretty insane pricing of memory these days" https://agentii.ai/v/TSLA/ect61/3. [FACT] Karn Budhiraj added that supplier investment is flowing into "metal injection molded parts, flexible printed circuits and all sorts of nonlinear technologies that are more based for the robot as opposed to the traditional vehicle supply chain" https://agentii.ai/v/TSLA/ect61/3.

[DEDUCTED] Tesla's disclosed Optimus cost narrative is compute-centric: AI chips and memory are the inputs management says will gate scale (Terafab, fab investments, memory allocation), consistent with the PIL-2 framing that the AI compute stack is the scarce minority (~10-15%) of humanoid BOM rather than the dominant cost https://agentii.ai/v/TSLA/ect61/1 https://agentii.ai/v/TSLA/ect61/3. [VIEW] The complementary PIL-2 claim — that actuator+drive is 40-70% of BOM — has no TSLA disclosure to validate it; Tesla discusses actuators only qualitatively (dexterity, electromechanical design), so the pillar's wrong_if test (<35% actuator content) cannot be run against this ticker's filings https://agentii.ai/v/TSLA/ect61/1.

[FACT] No Optimus unit cost or price target appears in any retrieved document. [DEDUCTED] Because Optimus is pre-revenue and reported within no segment, its unit economics are $0 disclosed revenue and 100% capitalized/R&D-phase costs through Q2 2026 https://agentii.ai/v/TSLA/sec259/28. [VIEW] Any external "$20-30K per robot" figures are promotional statements outside the SEC record and must not be treated as filed economics; this artifact records their absence rather than their value.

### 3.2 Automotive per-unit economics as the manufacturing-cost analogue

[FACT] FY2025: automotive sales revenue of $65,821M; total automotive revenues $69,526M (-10% YoY) https://agentii.ai/v/TSLA/sec253/42. [FACT] Total automotive cost of revenues $57,165M, automotive gross margin 17.8% (vs 18.4% in 2024, 19.4% in 2023); total gross margin 18.0%; energy segment gross margin 29.8% https://agentii.ai/v/TSLA/sec253/43. [FACT] The 10-K enumerates the automotive cost stack: "direct and indirect materials, labor costs, manufacturing overhead, including depreciation... shipping and logistic costs, tariffs, reserves for estimated warranty expenses, FSD... maintenance costs, vehicle connectivity costs, and allocations of electricity and infrastructure costs" related to free Supercharging https://agentii.ai/v/TSLA/sec253/43.

[FACT] XBRL cross-check (both revenue concepts): us-gaap:Revenues = $94,827M and us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax = $94,827M for FY2025, with us-gaap:CostOfRevenue = $77,733M — matching the 10-K tables exactly https://agentii.ai/v/TSLA/sec253/55.

[DEDUCTED] Per-vehicle FY2025 (1.64M deliveries https://agentii.ai/v/TSLA/sec253/36, total automotive revenue and cost above): revenue ≈ $69,526M / 1.64M ≈ **$42,394/vehicle**; cost ≈ $57,165M / 1.64M ≈ **$34,857/vehicle**; gross profit ≈ **$7,537/vehicle** (17.8% margin) https://agentii.ai/v/TSLA/sec253/42 https://agentii.ai/v/TSLA/sec253/43.

[FACT] Q2 2026: total revenues $28.24B (+$5.74B YoY), H1 $50.62B; total cost of revenues $23,485M; total gross margin 16.8% (Q2) and 18.7% (H1); automotive gross margin 16.9% (Q2), 18.7% (H1); energy gross margin fell to 20.4% from 30.3% YoY https://agentii.ai/v/TSLA/sec259/28 https://agentii.ai/v/TSLA/sec259/32. [FACT] The 10-Q's per-unit language: "Average cost per unit was relatively consistent due to unfavorable sales mix and a negative impact from the weakening of the United States dollar... offset by favorable impacts related to warranty adjustments and tariffs" https://agentii.ai/v/TSLA/sec259/32.

[DEDUCTED] H1 2026 (838K deliveries https://agentii.ai/v/TSLA/sec259/28; automotive cost $29,865M at 18.7% automotive GM https://agentii.ai/v/TSLA/sec259/32): implied automotive revenue ≈ $36,733M → ≈ $43.8K revenue/vehicle and ≈ $35.6K cost/vehicle — per-unit cost ~2% above FY2025, directionally consistent with the 10-Q's "relatively consistent" statement. [VIEW] Automotive per-unit cost stability shows the cost-down machine is currently offset by mix/tariffs/FX; as an analogue for humanoid manufacturing it is weak, because Tesla itself stresses Optimus shares "nothing from the existing supply chains" https://agentii.ai/v/TSLA/ect59/1.

### 3.3 Cost-down statements and the capex step-change (PIL-4)

[FACT] 10-K: "Our cost reduction efforts, cost innovation strategies, and additional localized procurement and manufacturing are key to our vehicles' affordability" https://agentii.ai/v/TSLA/sec253/37. [FACT] FY2025 R&D was $6,411M, +41% YoY, 7% of revenues, driven partly by AI-related engineering https://agentii.ai/v/TSLA/sec253/44. [FACT] Q4 2025 call: automotive margins ex-credits improved sequentially 15.4% → 17.9%; total gross margin >20.1%; 2026 capex guided "in excess of $20 billion" paying for six factories including "the Optimus factory," with continued elevated spend on "AI-related initiatives and new products like CyberCab, Semi, Optimus, and MegaPack" https://agentii.ai/v/TSLA/ect59/2. [FACT] FY2025 actual capex was $8.53B (vs $11.34B in 2024); H1 2026 capex already $8.28B (+$4.40B YoY) https://agentii.ai/v/TSLA/sec253/36 https://agentii.ai/v/TSLA/sec259/28.

[FACT] Optimus ramp disclosures: Fremont S/X line being converted to an Optimus factory with "a long-term goal of having a million units a year" https://agentii.ai/v/TSLA/ect59/1; production start "somewhere around the late July, August time frame" of 2026, with "production rate... impossible to predict" https://agentii.ai/v/TSLA/ect60/3; a second Optimus factory at Giga Texas "will probably start production around summer next year" (2027) https://agentii.ai/v/TSLA/ect60/1; Optimus to be "useful outside of Tesla sometime next year" (2027) https://agentii.ai/v/TSLA/ect60/1; Optimus 4 aspirationally "10 million units a year versus 1 million units a year of Optimus 3" https://agentii.ai/v/TSLA/ect61/5. [FACT] In the 10-K, "1 million bots delivered" is codified as operational milestone #3 of 12 in the 2025 CEO Performance Award, alongside $2.0-8.5T market-cap milestones https://agentii.ai/v/TSLA/sec253/86. [FACT] On the Q4 2025 call Musk cautioned Optimus "is still in the R&D phase... We wouldn't expect to have any kind of significant Optimus production volume until probably the end of this year [2026]" https://agentii.ai/v/TSLA/ect59/3.

[DEDUCTED] Assembling the disclosed timeline — starter production late Jul-Aug 2026, "quite flat and long" initial S-curve, Giga Texas plant from summer 2027, external usefulness "sometime next year" — first meaningful Optimus scale lands in the late-2027 through 2028 window https://agentii.ai/v/TSLA/ect60/3 https://agentii.ai/v/TSLA/ect61/1. [VIEW] This independently supports PIL-4's 2027-Q4-2028 "GPT-3.5 moment" window for physical AI, with the caveat that a moment defined by cost-per-unit inflection cannot be verified because Tesla discloses no Optimus unit cost. [VIEW] The 1M-bots CEO-award milestone is a long-dated incentive target, not guidance — promotional claims must be tagged accordingly https://agentii.ai/v/TSLA/sec253/86. [VIEW] The >$20B FY2026 capex program, explicitly naming the Optimus factory, marks the disclosed capacity build for that window https://agentii.ai/v/TSLA/ect59/2.

## 4. Key Metrics

| Metric | Value | Period | Citation |
|---|---|---|---|
| Total revenues | $94,827M | FY2025 | https://agentii.ai/v/TSLA/sec253/42 |
| Total gross margin | 18.0% | FY2025 | https://agentii.ai/v/TSLA/sec253/43 |
| Automotive gross margin | 17.8% | FY2025 | https://agentii.ai/v/TSLA/sec253/43 |
| Revenue per vehicle (deducted) | ~$42.4K | FY2025 | https://agentii.ai/v/TSLA/sec253/42 |
| Cost per vehicle (deducted) | ~$34.9K | FY2025 | https://agentii.ai/v/TSLA/sec253/43 |
| Gross profit per vehicle (deducted) | ~$7.5K | FY2025 | https://agentii.ai/v/TSLA/sec253/43 |
| Capex | $8.53B actual / >$20B guided | FY2025 / FY2026 | https://agentii.ai/v/TSLA/sec253/36 |
| Total gross margin | 16.8% | Q2 2026 | https://agentii.ai/v/TSLA/sec259/32 |
| Automotive gross margin | 16.9% | Q2 2026 | https://agentii.ai/v/TSLA/sec259/32 |
| Optimus unit economics | none disclosed | all periods | https://agentii.ai/v/TSLA/sec253/36 |
| Optimus production start | late Jul-Aug 2026 (guided) | — | https://agentii.ai/v/TSLA/ect60/3 |
| Optimus plant #2 (Giga Texas) | ~summer 2027 (guided) | — | https://agentii.ai/v/TSLA/ect60/1 |

## 5. Coverage Gaps & Citations

**Coverage gaps:**
1. **Optimus BOM / per-unit cost / price target**: not disclosed in any retrieved SEC filing or transcript. PIL-2's 40-70% actuator-content claim and its wrong_if test cannot be validated against TSLA's record.
2. **Optimus segment economics**: no Optimus revenue, COGS, or R&D split; robots sit inside unsegmented R&D and capex. R&D composition is described only qualitatively.
3. **Unit delivery counts for Optimus**: Q4 2025 call states Optimus is not in material factory use; no unit figures are filed.
4. **PIL-2 teardown corroboration**: teardown-derived industry BOM splits are not available via SEC retrieval; treat as external, wide-dispersion inputs.
5. **Promotional cost targets**: any Optimus cost/price figures from non-filing sources (e.g., social media) are out of retrieval scope; this artifact deliberately does not repeat them.

**Citation index (roll-up, non-duplicative):**

| citation_id | Filing | Pages used |
|---|---|---|
| sec253 | FY2025 10-K | 36, 37, 42, 43, 44, 55, 86 |
| sec259 | Q2 2026 10-Q | 28, 29, 32 |
| ect59 | Q4 FY2025 call | 1, 2, 3 |
| ect60 | Q1 FY2026 call | 1, 3 |
| ect61 | Q2 FY2026 call | 1, 3, 5 |

## 6. Verification

| # | Tool call | Purpose | Result |
|---|---|---|---|
| 1 | search_companies(TSLA) | Ticker resolution | Confirmed: Tesla, Inc., CIK 0001318605, NASDAQ |
| 2 | get_ticker_coverage(TSLA) | Coverage preflight | 7 sources; xbrl_facts 63,523 records; 19 transcripts |
| 3 | get_company_fiscal_calendar(TSLA) | Fiscal alignment | FY end Jan; latest 10-K report_date 2025-12-31 |
| 4 | search_documents ×5 (keyword/forms) | Layer 1 discovery | 92 docs; 5 10-Ks; 14 10-Qs; 19 transcripts |
| 5 | search_sec_filings (10-K, 10-Q) | citation_ids | sec253 (FY2025 10-K), sec259 (Q2 2026 10-Q), sec256, sec249, sec244 |
| 6 | read_source_outline(sec253) | Layer 2 map | 107-page map; margin table at p43, bots milestone at p86 |
| 7 | search_keyword_in_source(sec253/259, "Optimus") | Layer 2 filter | 7 hits (10-K), 2 hits (10-Q) |
| 8 | read_source_pages(sec253, p36/37/42/43) | Layer 3 | Revenue + cost/margin tables extracted |
| 9 | read_source_pages(sec259, p28/29/32) | Layer 3 | Q2 2026 MD&A + margin table + per-unit cost statement |
| 10 | list_sources(transcripts) | Transcript discovery | 19 source_ids (retried once after rate limit) |
| 11 | read_source_outline ×3 (transcripts) | ect citation_ids | ect59 (Q4 2025), ect60 (Q1 2026), ect61 (Q2 2026) |
| 12 | read_source_pages(ect61, p1/3/5) | Layer 3 | Supply-chain/compute cost commentary |
| 13 | read_source_pages(ect59, p1/2/3) | Layer 3 | Fremont 1M/yr line; margins 15.4%→17.9%; capex >$20B |
| 14 | read_source_pages(ect60, p1/3) | Layer 3 | Production start Jul-Aug 2026; Giga Texas plant 2027 |
| 15 | list_xbrl_concepts("Revenue") | Concept discovery (P2.1) | Revenues; RevenueFromContractWithCustomerExcludingAssessedTax |
| 16 | search_xbrl_facts ×5 | Structured numbers | FY2025 rev $94,827M (both concepts), COGS $77,733M; Q2 2026 rev $28,236M, COGS $23,485M |
| 17 | batch_search (XBRL, 6 sub-queries) | Consolidation attempt | Values stripped in batch mode; fell back to direct calls |
| 18 | search_unified("Optimus cost") | Cross-source sweep | Tool error (invalid JSON input); superseded by keyword searches |

All material numbers above trace to calls in this table; nothing was imported from memory or external sources. No price data used (market_data_stage: none).
