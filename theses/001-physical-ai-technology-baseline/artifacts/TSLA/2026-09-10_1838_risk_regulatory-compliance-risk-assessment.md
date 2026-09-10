---
artifact_id: "001-TSLA-risk-regulatory-compliance-risk-assessment-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: TSLA
skill: risk
mode: regulatory-compliance-risk-assessment
affix: risk-assessment
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "953fc5d396e7"
as_of: 2026-09-10
entity_claims:
  - "OBBBA-era governmental/regulatory actions have repealed/restricted consumer, manufacturing, and charging-infrastructure tax credits and certain regulatory credit programs tied to Tesla products [10-K sec253 p28]"
  - "TSLA automotive regulatory credits revenue: $2,763M (2024) → $1,993M (2025, -28%) → $526M H1 2026 (-49%); Q2 2026 $146M (-67%) [10-K sec253 p42; 10-Q sec259 p31]"
  - "Feb 2026 U.S. Supreme Court IEEPA ruling invalidated certain tariffs; TSLA may seek refunds; no receivable recognized until realizable [10-Q sec259 p24]"
  - "NHTSA, NTSB, SEC, DOJ maintain ongoing information requests covering Autopilot/FSD/Robotaxi; no agency has concluded wrongdoing [10-Q sec259 p25]"
  - "CRD discrimination trial (first phase) set for September 21, 2026; EEOC case in discovery [10-Q sec259 p24]"
citations:
  - "https://agentii.ai/v/TSLA/sec253/page14"
  - "https://agentii.ai/v/TSLA/sec253/page28"
  - "https://agentii.ai/v/TSLA/sec259/page24"
  - "https://agentii.ai/v/TSLA/sec259/page25"
pillars_addressed: [PIL-3]
claim_state: pinned
key_metrics:
  regulatory_credits_fy2025_usd_m: 1993
  regulatory_credits_fy2025_yoy_pct: -28
  regulatory_credits_h1_2026_usd_m: 526
  regulatory_credits_q2_2026_yoy_pct: -67
  fx_sensitivity_10pct_usd_b_q2_2026: 1.64
  crd_trial_date: "2026-09-21"
conclusions:
  - "Tesla's regulatory exposure is dominated by three active fronts: federal incentive/credit rollback (OBBBA), autonomy oversight (NHTSA/NTSB/DOJ/SEC plus state/city AV patchwork), and employment discrimination litigation (CRD trial Sept 21, 2026)."
  - "For PIL-3: there is no humanoid-specific regulatory framework referenced in the corpus; autonomy regulation (FMVSS/AV) is the closest analogue, and management signals it is cooperative with NHTSA while opposing prescriptive state rules."
facts_count: 19
deducted_count: 4
views_count: 4
citation_count: 19
---

# Regulatory & Compliance Risk Assessment — TSLA (as of 2026-09-10)

**Skill:** agentii/risk — mode `regulatory-compliance-risk-assessment` · **Pillar served:** PIL-3 (manipulation reliability gates deployment — regulatory/compliance lens on autonomy and humanoid deployment)
**Anchor filings:** FY2025 10-K `sec253` · Q2 FY2026 10-Q `sec259` · Q2 2026 call transcript `ect61`

## Executive Summary

Tesla's regulatory risk profile has shifted from incentive-exposure (a tailwind through 2024) to regulatory-rollback exposure (a headwind since 2025). Government actions have "repealed and/or restricted consumer, manufacturing and charging infrastructure tax credits, and certain regulatory credit programs tied to our products" (https://agentii.ai/v/TSLA/sec253/page28), and the financial effect is visible: automotive regulatory credits fell 28% in FY2025 to $1,993M and 67% YoY in Q2 2026 to $146M (https://agentii.ai/v/TSLA/sec253/page42, https://agentii.ai/v/TSLA/sec259/page31). On the autonomy front, the company operates under a regulatory patchwork — updated FMVSS rules at the federal level plus divergent state/city AV regimes, and materially different frameworks in ECE countries and China (https://agentii.ai/v/TSLA/sec253/page14) — while NHTSA, NTSB, SEC, and DOJ maintain ongoing information requests on Autopilot/FSD/Robotaxi matters, with no agency having concluded wrongdoing (https://agentii.ai/v/TSLA/sec259/page25). The immediate compliance calendar includes the CRD employment-discrimination trial set for September 21, 2026 (https://agentii.ai/v/TSLA/sec259/page24) and the Ninth Circuit FSD class-certification appeal (oral argument August 31, 2026) (https://agentii.ai/v/TSLA/sec259/page24). A February 2026 Supreme Court IEEPA ruling opens a possible tariff-refund recovery, unrecorded until realizable (https://agentii.ai/v/TSLA/sec259/page24). For PIL-3: no humanoid-specific regulatory regime appears anywhere in the corpus; autonomy regulation is the operative template, and management's posture toward it is explicitly cooperative at the federal level and adversarial toward prescriptive state rules.

## Recent Regulatory Developments

- **OBBBA-era rollback of EV incentives and credit programs [FACT]:** the FY2025 10-K states recent governmental/regulatory actions "repealed and/or restricted" tax credits and "certain regulatory credit programs tied to our products" (https://agentii.ai/v/TSLA/sec253/page28); the 10-K revenue narrative attributes the 28% drop in regulatory-credit revenue in 2025 to these actions (https://agentii.ai/v/TSLA/sec253/page42). [DEDUCTED] With Q2 2026 credits at $146M, an annualized run-rate of ~$0.6B vs. $2.76B in 2024, this policy channel has been materially impaired.
- **IEEPA tariff invalidation [FACT]:** the U.S. Supreme Court's February 2026 ruling invalidating certain IEEPA tariffs may entitle Tesla to refunds of tariffs previously paid; the company will recognize no receivable "until such amounts are realized or realizable," and future refunds may reduce revenue where energy-storage customers hold contractual pass-through rights (https://agentii.ai/v/TSLA/sec259/page24).
- **2018 CEO award reinstated [FACT]:** the Delaware Supreme Court on December 19, 2025 reversed the Chancery rescission, reinstating Musk's 2018 package with $1 in nominal damages and a "significantly reduced" fee award from the prior $345M (https://agentii.ai/v/TSLA/sec253/page93). This removes a long-standing governance/litigation overhang while the 2025 CEO Performance Award introduces a new one (423.7M shares, $2.0T–$8.5T market-cap milestones) (https://agentii.ai/v/TSLA/sec253/page86) [DEDUCTED].
- **Delaware→Texas reincorporation backdrop [FACT]:** the company converted from a Delaware to Texas corporation on June 13, 2024; Delaware derivative suits were dismissed April 13, 2026 with a plaintiff appeal pending in the Delaware Supreme Court as of May 2026 (https://agentii.ai/v/TSLA/sec259/page24).
- **Employment discrimination enforcement [FACT]:** CRD first-phase trial set for September 21, 2026 (moved from July 20, 2026 in the 10-K) (https://agentii.ai/v/TSLA/sec259/page24, https://agentii.ai/v/TSLA/sec253/page94); EEOC action in discovery with no trial date (https://agentii.ai/v/TSLA/sec259/page24).
- **Autonomy-related litigation milestones [FACT]:** a limited California consumer class was certified August 18, 2025 in the FSD misrepresentation action; the Ninth Circuit granted Tesla's appeal petition December 18, 2025 and the district court stayed the case January 5, 2026; oral argument set August 31, 2026 (https://agentii.ai/v/TSLA/sec259/page24). The earlier 2019-2023 securities class action was affirmed-dismissed December 2, 2025 (https://agentii.ai/v/TSLA/sec253/page95).
- **Benavides product-liability verdict [FACT]:** post-trial motions denied February 19, 2026; Tesla's Eleventh Circuit opening brief filed July 2, 2026; recorded accrual is immaterial ($129M compensatory at 33% fault; $200M punitive) (https://agentii.ai/v/TSLA/sec259/page25).

## Forward Policy Risk Analysis

- **AV regulation fragmentation [FACT]:** NHTSA has updated certain FMVSS for AV design but other FMVSS "do not currently account for autonomous vehicle design"; states and cities impose or are considering restrictions on AV testing, commercial operation, and ride-hailing — "this regulatory patchwork increases the legal complexity" (https://agentii.ai/v/TSLA/sec253/page14). In ECE countries, rules "can compromise or prevent" ADAS/AV use entirely; China's emerging rules "may differ materially" (https://agentii.ai/v/TSLA/sec253/page14).
- **FMVSS reform for purpose-built AVs [VIEW]:** on the Q2 2026 call, Lars Moravy welcomed "FMVSS rules, moving towards acceptance and adoption of purely built AVs" and NHTSA support, while criticizing New Jersey's state-level sensor-requirement proposals as "regulations that provide a solution before identifying the problem" (https://agentii.ai/v/TSLA/ect61/page4). Analysts noted NHTSA Administrator Jonathan Morrison's public comments on removing steering wheels/pedals; Tesla says no other federal gating factor exists for Cybercab ramp (https://agentii.ai/v/TSLA/ect61/page5) [VIEW].
- **Tariff and trade policy [FACT]:** the 10-K warns the "exact scope" of U.S. tariffs "is not known at this time"; historical U.S. special tariff actions "have increased our costs" and retaliatory tariffs have "impacted the pricing for our products" (https://agentii.ai/v/TSLA/sec253/page21). The 10-Q adds the tariff regime "will have a relatively larger impact on our energy generation and storage business" (https://agentii.ai/v/TSLA/sec259/page28).
- **Critical-minerals traceability [FACT]:** OBBBA compliance "requires rigorous traceability of raw materials"; failure to document origin of critical minerals can strip products of tax-credit eligibility, raising effective customer prices (https://agentii.ai/v/TSLA/sec253/page28).
- **Energy policy headwinds [FACT]:** net-metering benefits have been "reduced, altered or eliminated in several jurisdictions" and contested before FERC; OBBBA provisions "could significantly increase battery cell expenses" (https://agentii.ai/v/TSLA/sec253/page28, https://agentii.ai/v/TSLA/sec259/page30).
- **Humanoid regulatory vacuum [DEDUCTED]:** the corpus contains no humanoid-robot-specific regulatory discussion (safety certification, labor-displacement rules, workplace robot standards). If Optimus deploys at scale, the nearest analogue frameworks are NHTSA/FMVSS (vehicles), OSHA (workplace), and product-liability common law — all currently unequipped for general-purpose humanoids [DEDUCTED]. This is the PIL-3 regulatory exposure: deployment ambition ("1 million bots delivered" milestone, https://agentii.ai/v/TSLA/sec253/page86) running ahead of any disclosed regulatory engagement.

## Regulatory Preparedness

- **Federal-regulator cooperation [FACT/VIEW]:** Tesla states it "routinely cooperates" with NHTSA/NTSB/SEC/DOJ requests and that no agency has concluded wrongdoing (https://agentii.ai/v/TSLA/sec259/page25). Moravy: "we have a partner there [NHTSA], and we're working together" on FMVSS modernization (https://agentii.ai/v/TSLA/ect61/page5) [VIEW].
- **Cybersecurity compliance infrastructure [FACT]:** ISO/IEC 27001:2013 certification of the Information Security Management System as of 2025, third-party assessments, bug bounty, and tabletop exercises (https://agentii.ai/v/TSLA/sec253/page32).
- **Disclosure controls [FACT]:** CEO/CFO evaluated disclosure controls and procedures as effective as of June 30, 2026; no material change in internal control over financial reporting (https://agentii.ai/v/TSLA/sec259/page37).
- **Market-risk disclosure maturity [FACT]:** quantified FX sensitivity of $1.64B at June 30, 2026 for a 10% adverse currency move, assuming no hedging (https://agentii.ai/v/TSLA/sec259/page37).
- **Financial contingency posture [FACT]:** immaterial accrual recorded for Benavides; no receivable for IEEPA refunds until realized; $556M unused letters of credit at Dec 31, 2025 (https://agentii.ai/v/TSLA/sec259/page25, https://agentii.ai/v/TSLA/sec259/page24, https://agentii.ai/v/TSLA/sec253/page96).

## Risk Mitigation

- **Performance-as-advocacy [VIEW]:** management's stated regulatory strategy is to let safety performance drive adoption and rulemaking — "the best regulations… provide companies and innovators with a goal or a task and allow us to figure out the solution"; Tesla will "let our performance speak for itself" (https://agentii.ai/v/TSLA/ect61/page4). This aligns with PIL-3: manipulation reliability is the company's primary regulatory-risk mitigation instrument [VIEW].
- **Supply-chain localization vs. tariffs [FACT]:** the 10-K mitigation posture is "vertical integration, supply chain localization" and domestic cell production against tariff exposure (https://agentii.ai/v/TSLA/sec253/page37, https://agentii.ai/v/TSLA/sec253/page21).
- **Litigation defense posture [FACT]:** Tesla "intends to vigorously defend itself" across the discrimination, securities, and product-liability dockets, with active appeals in the Ninth and Eleventh Circuits (https://agentii.ai/v/TSLA/sec259/page24, https://agentii.ai/v/TSLA/sec259/page25).
- **Traceability and documentation [FACT]:** compliance with OBBBA critical-minerals documentation is treated as a customer-price-risk mitigation (https://agentii.ai/v/TSLA/sec253/page28).

## Coverage Gaps & Citations

**Coverage gaps:** (1) No humanoid-robot regulatory disclosure exists in the corpus — the PIL-3 "autonomy regulatory exposure" question is answerable only by analogy to AV/vehicle frameworks. (2) No DOJ/SEC/NHTSA investigation outcome documents are retrievable; filings state no wrongdoing concluded. (3) The `other_events_8_01` label is thin (5 records, newest April 2024); 8-K-level regulatory events post-2024 were not individually retrievable by label. (4) Un-attributed $71M damages XBRL fact (Q1 2026 10-Q) excluded. (5) No state-level (e.g., New Jersey sensor rule) primary texts in corpus — known only via transcript commentary [VIEW].

**Citations (roll-up index):**

1. https://agentii.ai/v/TSLA/sec253/page14
2. https://agentii.ai/v/TSLA/sec253/page21
3. https://agentii.ai/v/TSLA/sec253/page28
4. https://agentii.ai/v/TSLA/sec253/page32
5. https://agentii.ai/v/TSLA/sec253/page37
6. https://agentii.ai/v/TSLA/sec253/page42
7. https://agentii.ai/v/TSLA/sec253/page86
8. https://agentii.ai/v/TSLA/sec253/page93
9. https://agentii.ai/v/TSLA/sec253/page94
10. https://agentii.ai/v/TSLA/sec253/page95
11. https://agentii.ai/v/TSLA/sec253/page96
12. https://agentii.ai/v/TSLA/sec259/page24
13. https://agentii.ai/v/TSLA/sec259/page25
14. https://agentii.ai/v/TSLA/sec259/page28
15. https://agentii.ai/v/TSLA/sec259/page30
16. https://agentii.ai/v/TSLA/sec259/page31
17. https://agentii.ai/v/TSLA/sec259/page37
18. https://agentii.ai/v/TSLA/ect61/page4
19. https://agentii.ai/v/TSLA/ect61/page5

## Verification (call trace)

| # | Tool | Call | Result used |
|---|---|---|---|
| 1 | search_companies | TSLA | CIK, exchange, filing dates |
| 2 | get_ticker_coverage | TSLA | corpus inventory |
| 3 | get_company_fiscal_calendar | TSLA | period mapping |
| 4 | search_documents | other_events_8_01; transcripts | 8-K label coverage gap; transcript list |
| 5 | search_sec_filings | 10-K / 10-Q / 8-K | sec253, sec259 |
| 6 | read_source_outline | sec253, sec259, transcript | page maps; ect61 |
| 7 | list_xbrl_concepts | revenue, contingency | concept selection |
| 8 | read_source_pages | sec253 p14,21,28,32,37,42,86,93,94,95,96 | regulatory environment, incentives, litigation |
| 9 | read_source_pages | sec259 p24,25,28,30,31,37 | IEEPA, docket, credits, controls |
| 10 | read_source_pages | ect61 p4,5 | NHTSA partnership, state-rule posture |
| 11 | search_xbrl_facts | RevenueFromContractWithCustomerExcludingAssessedTax, Revenues FY2025 | $94,827M |
| 12 | search_xbrl_facts | LossContingencyDamagesAwardedValue | $129M/$1/$176M/$345M |
| 13 | search_keyword_in_source | sec253 "Optimus"; sec256 "damages" | disclosure maps |
| 14 | list_sources | 2026 transcripts | ect61 resolution |

Tool diversity: 11 distinct tools. All cited numbers trace to these calls; nothing fabricated where the corpus was silent.
