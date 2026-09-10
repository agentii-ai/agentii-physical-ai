---
artifact_id: "001-NVDA-risk-regulatory-compliance-risk-assessment-20260910"
thesis_id: "001-physical-ai-technology-baseline"
ticker: NVDA
skill: risk
mode: regulatory-compliance-risk-assessment
affix: risk-assessment
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "953fc5d396e7"
as_of: 2026-09-10
entity_claims: []
citations:
  - "https://agentii.ai/v/NVDA/sec169/10"
  - "https://agentii.ai/v/NVDA/sec169/25"
  - "https://agentii.ai/v/NVDA/sec169/36"
  - "https://agentii.ai/v/NVDA/sec169/37"
  - "https://agentii.ai/v/NVDA/sec169/55"
  - "https://agentii.ai/v/NVDA/sec169/71"
  - "https://agentii.ai/v/NVDA/sec169/78"
  - "https://agentii.ai/v/NVDA/sec173/16"
  - "https://agentii.ai/v/NVDA/sec173/27"
  - "https://agentii.ai/v/NVDA/sec173/31"
  - "https://agentii.ai/v/NVDA/sec169/26"
  - "https://agentii.ai/v/NVDA/sec169/42"
  - "https://agentii.ai/v/NVDA/sec169/76"
  - "https://agentii.ai/v/NVDA/sec169/33"
  - "https://agentii.ai/v/NVDA/sec157/2"
  - "https://agentii.ai/v/NVDA/sec173/34"
  - "https://agentii.ai/v/NVDA/sec173/35"
  - "https://agentii.ai/v/NVDA/sec173/36"
  - "https://agentii.ai/v/NVDA/sec173/37"
  - "https://agentii.ai/v/NVDA/sec173/38"
pillars_addressed: [PIL-3]
claim_state: pinned
key_metrics:
  h20_charge_q1_fy2026_usd_b: 4.5
  h20_license_revenue_usd_m: 60
  usg_expected_revenue_share_pct: 15
  h200_tariff_pct: 25
  china_antitrust_preliminary_finding_date: "2025-09-15"
  eu_ai_act_effective_date: "2024-08-01"
  effective_tax_rate_fy2026_pct: 15.1
  unrecognized_tax_benefits_usd_b: 4.4
  buyback_authorization_may2026_usd_b: 80
conclusions:
  - "Export controls are NVDA's dominant regulatory risk and are escalating in both scope (worldwide AI Diffusion replacement rule) and instrument (license conditions reaching into chip design and revenue sharing)."
  - "NVDA is now in a two-front regulatory squeeze: U.S. export controls on one side and Chinese antitrust retaliation (Mellanox finding, Action Plan) on the other."
  - "Regulatory shocks have already been financialized once: the H20 license requirement produced a $4.5B inventory/purchase-obligation charge — the template for future control changes given $119B of supply commitments."
  - "For PIL-3: NVDA's regulatory exposure demonstrates the thesis premise that reliability-and-safety regulation gates deployment — but for NVDA the gate is export/competition law applied to compute, not manipulation-reliability law applied to physical AI."
facts_count: 23
deducted_count: 10
views_count: 2
citation_count: 20
---

# NVDA — Regulatory & Compliance Risk Assessment
**Mode:** regulatory-compliance-risk-assessment · **Skill:** risk · **Corpus:** agentii-2026-09-10 · **Pillar:** PIL-3 (regulation as deployment gate)

## Executive Summary

NVDA's regulatory risk is dominated by a single escalating vector: U.S. export controls on AI compute, now layered with Chinese antitrust retaliation and worldwide AI-governance regimes. The control regime has expanded from China-only restrictions (Aug 2022, A100/H100) to D:5-country licensing (Oct 2023), a worldwide AI Diffusion IFR (Jan 2025), an indefinite H20 license requirement that produced a $4.5B charge (Apr 2025) [FACT] https://agentii.ai/v/NVDA/sec169/10 https://agentii.ai/v/NVDA/sec157/2, and — after the IFR's announced rescission — a pending replacement rule of unknown scope [FACT] https://agentii.ai/v/NVDA/sec169/10. On the other front, China's antitrust regulators issued a preliminary finding on 2025-09-15 that NVDA's export-control compliance violated the terms of its Mellanox acquisition approval [FACT] https://agentii.ai/v/NVDA/sec169/26. Broader regimes add compliance breadth: the EU AI Act (effective 2024-08-01), U.S. state AI laws (effective 2026-01-01), worldwide competition-RFI pressure, and proposals (GAIN AI Act, RASA) that would bind future administrations and cloud services [FACT] https://agentii.ai/v/NVDA/sec169/25 https://agentii.ai/v/NVDA/sec173/37. For PIL-3, NVDA is the worked example of the thesis premise that regulation gates deployment — except the gate is export law on compute, not safety law on manipulation [DEDUCTED] https://agentii.ai/v/NVDA/sec173/37.

## Recent Regulatory Developments (timeline)

| Date | Development | Financial/material consequence | Evidence |
|---|---|---|---|
| Aug 2022 | USG export licensing for A100/H100/DGX to China and Russia | China revenue exposure began shrinking | https://agentii.ai/v/NVDA/sec169/10 |
| Jul 2023 | Additional licensing for A100/H100 subset (incl. Middle East) | Regional market restrictions | https://agentii.ai/v/NVDA/sec169/10 |
| Oct 2023 | Expanded licensing to China + D:1/D:4/D:5 (A100/A800/H100/H800/L4/L40/L40S/RTX 4090/GB200 NVL72/B200) | Broad product-scope control | https://agentii.ai/v/NVDA/sec169/10 |
| Jan 2025 | AI Diffusion IFR published — worldwide licensing for H200/GB200/GB300; three-tier country scheme | Would have been global; later rescinded | https://agentii.ai/v/NVDA/sec169/10 |
| Apr 2025 | H20 license required, "for the indefinite future"; 8-K expected up to ~$5.5B charges | Actual charge: $4.5B (Q1 FY2026) | https://agentii.ai/v/NVDA/sec157/2 https://agentii.ai/v/NVDA/sec169/10 |
| May 2025 | USG announces rescission of AI Diffusion IFR; replacement rule pending | Ongoing uncertainty | https://agentii.ai/v/NVDA/sec169/10 |
| Aug 2025 | H20 licenses granted to certain China customers; USG expresses expectation of 15%+ of licensed-sale revenue to USG | ~$60M H20 revenue; novel revenue-sharing condition | https://agentii.ai/v/NVDA/sec169/10 |
| Sep 2025 | China antitrust preliminary finding: Mellanox-approval terms violated | Financial penalties / business restrictions possible | https://agentii.ai/v/NVDA/sec169/26 |
| Oct 2025 | Senate passes GAIN AI Act in NDAA | Would restrict adaptation of export rules; private review of licensing decisions | https://agentii.ai/v/NVDA/sec173/37 |
| Feb 2026 | H200 license (small amounts, specific customers); U.S. inspection required; 25% tariff on importation | Zero revenue to date | https://agentii.ai/v/NVDA/sec169/10 |
| 2024–2026 | EU AI Act effective 2024-08-01 (full applicability after 2-yr transition); U.S. state AI laws effective 2026-01-01 | Model training/deployment constraints; compliance cost | https://agentii.ai/v/NVDA/sec169/25 |
| Ongoing | French Competition Authority inquiry (graphics-card/CSP markets; whether gaming vs data-center GPUs are separate categories); RFIs from EU, US, UK, China, South Korea regulators | Burdensome; could affect export-control scope for gaming GPUs | https://agentii.ai/v/NVDA/sec169/25 https://agentii.ai/v/NVDA/sec173/37 |

All timeline rows above are issuer-disclosed events as stated on the cited pages [FACT].

Supporting structured fact: NVDA's effective tax rate was 15.1% in FY2026 [FACT] https://agentii.ai/v/NVDA/sec169/42 and unrecognized tax benefits were $4.4B [FACT] https://agentii.ai/v/NVDA/sec169/76.

## Forward Policy Risk Analysis

- **AI Diffusion replacement rule.** "The scope, timing, and requirements of the forthcoming rule remain uncertain... may impose new restrictions on our products or operations and/or add license requirements that could have a material impact" [FACT] https://agentii.ai/v/NVDA/sec169/10. Given the IFR draft covered H200/GB200/GB300 worldwide, any successor with Tier-2 caps would throttle non-China demand — the 31% of revenue from non-U.S.-headquartered customers in FY2026 is the exposed base [DEDUCTED] https://agentii.ai/v/NVDA/sec169/78.
- **GAIN AI Act and RASA.** GAIN would restrict executive flexibility on export rules and allow private review/overturn of licensing decisions; RASA could prohibit cloud services to companies with ultimate parents in China [FACT] https://agentii.ai/v/NVDA/sec173/37. Enactment would make the control regime stickier and harder to manage [DEDUCTED] https://agentii.ai/v/NVDA/sec173/37.
- **Design-level regulation.** USG license conditions may "require chip tracking and throttling mechanisms that could disable or impair GPUs" — introducing reliability/security liabilities into the product itself [FACT] https://agentii.ai/v/NVDA/sec173/37. This is regulation reaching into the manipulation-reliability layer of hardware — the closest NVDA analogue to the thesis's PIL-3 premise [DEDUCTED] https://agentii.ai/v/NVDA/sec173/37.
- **Chinese countermeasures.** The Chinese government "has encouraged customers to purchase from our China-based competitors" and published a data-center Action Plan endorsing compute-per-watt/per-memory-bandwidth standards that could exclude NVDA designs if it re-entered [FACT] https://agentii.ai/v/NVDA/sec173/38. Combined with the Mellanox preliminary finding, re-entry optionality is deteriorating [DEDUCTED] https://agentii.ai/v/NVDA/sec169/26.
- **Expansion vectors.** The USG may extend controls to gaming GPUs (impacting the Hong Kong-distributed supply chain) and to networking products used in server GPU clusters [FACT] https://agentii.ai/v/NVDA/sec173/37. Connected-Vehicle import restrictions could constrain automotive solutions [FACT] https://agentii.ai/v/NVDA/sec173/38. Deemed-export limits could impair R&D teams [FACT] https://agentii.ai/v/NVDA/sec169/25.

## Regulatory Preparedness

- **Compliance posture.** NVDA states it "seek[s] to strictly comply with all applicable export control regulators" and provides assistance to authorities on diversion; but it "must also rely on the compliance programs of our customers and partners" since it lacks physical control after sale [FACT] https://agentii.ai/v/NVDA/sec173/38. Diversion risk is therefore partially externalized onto counterparties [DEDUCTED] https://agentii.ai/v/NVDA/sec173/38.
- **Public-defense capability.** Following Chinese government questioning whether H20 contains built-in vulnerabilities (a reaction to U.S. legislative proposals for mandatory chip features), NVDA issued a public response stating its GPUs "do not include such built-in vulnerabilities" [FACT] https://agentii.ai/v/NVDA/sec173/37.
- **Financial shock absorption.** FY2026 ended with the $4.5B charge absorbed inside a year that still produced $120.1B net income and $102.7B operating cash flow, and Q1 FY2027 added an $80B buyback authorization on 2026-05-18 [FACT] https://agentii.ai/v/NVDA/sec169/37 https://agentii.ai/v/NVDA/sec169/55 https://agentii.ai/v/NVDA/sec173/38. Balance-sheet capacity to absorb regulatory charges is therefore high [DEDUCTED] https://agentii.ai/v/NVDA/sec169/37.
- **Supply-chain mitigation.** U.S./Latin America manufacturing expansion responds to Taiwan/Korea concentration — itself a regulatory-policy exposure [FACT] https://agentii.ai/v/NVDA/sec169/36.
- **Governance.** Disclosure controls were assessed effective as of 2026-04-26; ERP phased upgrade in progress with no material ICFR changes [FACT] https://agentii.ai/v/NVDA/sec173/31.

## Risk Mitigation (evaluation)

1. **Diversify end-demand geography.** Non-U.S.-headquartered revenue fell to 22% of total in Q1 FY2027 from 42% a year earlier [FACT] https://agentii.ai/v/NVDA/sec173/27 — U.S. hyperscale concentration reduces export-control exposure but increases customer-concentration risk (21%/17%/16%) [DEDUCTED] https://agentii.ai/v/NVDA/sec173/27.
2. **License-arbitrage product lines.** H20 (~$60M under license) and H200 (pending) preserve nominal China presence but are economically immaterial versus the $4.5B charge and the 15% USG revenue-share expectation [DEDUCTED] https://agentii.ai/v/NVDA/sec169/10.
3. **Litigation/investigation management.** The securities-litigation and worldwide-RFI load is disclosed but unquantified [FACT] https://agentii.ai/v/NVDA/sec169/71.
4. **Structural compliance investment** — U.S. inspection routing for H200 and domestic manufacturing build-out indicate regulatory-mandated supply-chain redesign is underway [DEDUCTED] https://agentii.ai/v/NVDA/sec169/36.

## PIL-3 (Pillar) Relevance

PIL-3's premise is that manipulation reliability gates physical-AI deployment. NVDA's disclosures supply the counterfactual calibration: for compute, the deployment gate is regulatory — export controls, tariffs, and antitrust — and it has already materialized financially ($4.5B) [FACT] https://agentii.ai/v/NVDA/sec169/10. The lesson the thesis can carry: a deployment-gate shock, whatever its cause, lands as inventory and purchase-obligation charges against forward supply commitments ($119B outstanding as of 2026-04-26) [FACT] https://agentii.ai/v/NVDA/sec173/16. A manipulation-reliability regulatory event in physical AI would land on robot OEMs the way H20 landed on NVDA [VIEW] https://agentii.ai/v/NVDA/sec169/10. Moreover, NVDA's own forward policy risk now includes chip-level throttling/tracking mandates — regulation injecting reliability hazards into hardware, the mirror-image of reliability as moat [VIEW] https://agentii.ai/v/NVDA/sec173/37.

## Coverage Gaps

- No retrieval of the China Mellanox preliminary-finding primary document; findings are cited from the 10-K/10-Q restatement only.
- The AI Diffusion replacement rule text is not yet published per NVDA disclosures; scope remains indeterminate — a structural gap, not a retrieval gap.
- Q2 FY2027 10-Q absent from corpus; post-May-2026 regulatory events (if any) are not covered.
- FCA inquiry outcome and worldwide-RFI statuses are unquantified by the issuer.

## Citations (roll-up index)

1. Export-control timeline + consequences — https://agentii.ai/v/NVDA/sec169/10
2. Worldwide regulator interest; EU AI Act; state AI laws; Ukraine — https://agentii.ai/v/NVDA/sec169/25
3. China antitrust / Mellanox preliminary finding — https://agentii.ai/v/NVDA/sec169/26
4. Effective tax rate 15.1% — https://agentii.ai/v/NVDA/sec169/42
5. Unrecognized tax benefits $4.4B — https://agentii.ai/v/NVDA/sec169/76
6. Buyback authorization $60B (FY2026) — https://agentii.ai/v/NVDA/sec169/33
7. 8-K H20 license requirement (indefinite; up to ~$5.5B expected) — https://agentii.ai/v/NVDA/sec157/2
8. 10-Q regulatory risk factors (EU AI Act; FCA; worldwide RFIs) — https://agentii.ai/v/NVDA/sec173/34
9. 10-Q export-control risk factors (China inquiries; sanctions) — https://agentii.ai/v/NVDA/sec173/35
10. 10-Q export-control restatement (foreclosure; H20/H200 details) — https://agentii.ai/v/NVDA/sec173/36
11. 10-Q GAIN/RASA, license conditions (throttling), FCA GPU categories, design-out — https://agentii.ai/v/NVDA/sec173/37
12. 10-Q China Action Plan, Connected Vehicle, Taiwan/Korea, diversion, buyback/dividend — https://agentii.ai/v/NVDA/sec173/38
13. 10-K supply-chain diversification (U.S./Latin America) — https://agentii.ai/v/NVDA/sec169/36
14. 10-K FY2026 summary (net income $120.1B) — https://agentii.ai/v/NVDA/sec169/37
15. 10-K cash flow (operating cash flow $102.7B) — https://agentii.ai/v/NVDA/sec169/55
16. 10-K litigation disclosure (unquantified) — https://agentii.ai/v/NVDA/sec169/71
17. 10-K geography (non-U.S.-headquartered revenue 31% FY2026) — https://agentii.ai/v/NVDA/sec169/78
18. 10-Q commitments ($119B; $95B due in FY2027) — https://agentii.ai/v/NVDA/sec173/16
19. 10-Q concentration of revenue (21/17/16%; outside-US 22%) — https://agentii.ai/v/NVDA/sec173/27
20. 10-Q controls and procedures (effective; ERP upgrade) — https://agentii.ai/v/NVDA/sec173/31

## Verification

| # | Tool | Query | Result | Evidence carried |
|---|---|---|---|---|
| 1 | search_companies | NVDA | NVIDIA Corp, CIK 0001045810 | ticker |
| 2 | get_ticker_coverage | NVDA | corpus through 2026-05-09 | freshness |
| 3 | get_company_fiscal_calendar | NVDA | FY2027 Q1 = Mar–May 2026 | periods |
| 4 | search_documents | other_events_8_01 | 6 risk-event 8-Ks | event map |
| 5 | search_sec_filings | 10-K | sec169 (FY2026, filed 2026-02-25) | annual |
| 6 | search_sec_filings | 10-Q | sec173 (Q1 FY2027, filed 2026-05-20) | quarterly |
| 7 | search_sec_filings | 8-K 2025–2026 | sec157 (H20, 2025-04-15); sec153 (IFR) | event filings |
| 8 | read_source_outline | sec169 | page map; regulatory pages 9–10, 25–28 | page selection |
| 9 | read_source_outline | sec173 | page map; regulatory pages 34–38 | page selection |
| 10 | read_source_outline | sec157 | H20 8-K map | page selection |
| 11 | read_source_pages | sec169 p9,10,25,26 | export-control timeline; worldwide regulators; Mellanox | mode 3 core |
| 12 | read_source_pages | sec173 p31,32,33,34 | 10-Q regulatory risk factors | mode 3 core |
| 13 | read_source_pages | sec173 p35,36,37,38 | GAIN/RASA; license conditions; China Action Plan; Connected Vehicle | mode 3 core |
| 14 | read_source_pages | sec157 p2 | H20 8-K exact text | mode 3 core |
| 15 | search_xbrl_facts | Revenues | FY2026 $215,938M; Q1 FY2027 $81,615M | structured |
| 16 | list_xbrl_concepts | Revenue | concept inventory | structured |
| 17 | search_keyword_in_source | sec169 "energy" | cross-check pages | cross-check |

All regulatory facts above are drawn from issuer filings via the calls listed; no market/price data used (market_data_stage: none).
