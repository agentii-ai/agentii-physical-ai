---
artifact_id: "002-ISRG-business-model-distribution-channel-analysis-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: ISRG
skill: business-model
mode: distribution-channel-analysis
affix: ""
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "9479220eef91"
as_of: 2026-09-11
entity_claims:
  - entity: ISRG
    metric: recurring_revenue_share_pct
    value: 85
    unit: pct
    period: Q2-2026
    source: "10-Q:page40"
    retrieved_at: 2026-09-11
  - entity: ISRG
    metric: installed_base_units
    value: 12806
    unit: units
    period: Q2-2026
    source: "10-Q:page32 + 10-Q:page35"
    retrieved_at: 2026-09-11
citations:
  - "sec166 (FY2025 10-K, filed 2026-02-03)"
  - "sec172 (Q2-2026 10-Q, filed 2026-07-21)"
  - "8-K 2026-03-02 (ab medica acquisition, via search_documents)"
pillars_addressed: [PIL-3]
claim_state: pinned
key_metrics:
  da_vinci_placements_op_lease_share_pct_fy2025: 51
  op_lease_installed_base_share_pct_q2_2026: 29.8
  ab_medica_acquisition_cash_usd: 533100000
  us_revenue_share_pct_fy2025: 68
conclusions:
  - "Go-to-market is a hybrid: direct sales organizations in major markets (U.S., most of Europe, China-JV, Japan, S.Korea, India, Taiwan, Canada) plus distributors elsewhere; no numeric direct:indirect revenue split is disclosed."
  - "Channel evolution is measurable along two axes: (1) leasing (op-lease share of da Vinci placements 48% → 51% → 51%, 2023-2025; 54% Q2-2026) and (2) distributor-to-direct conversion in Europe via the $533.1M ab medica acquisition (March 2026)."
facts_count: 14
deducted_count: 4
views_count: 2
citation_count: 22
---

# ISRG — Distribution Channels & Go-to-Market (mode 1_2)

## Executive Summary

ISRG's distribution model is **hybrid**: direct sales organizations in the U.S., Europe (excluding Greece and Eastern European countries — after March 2026), China (via majority-owned Fosun JVs), Japan, South Korea, India, Taiwan, and Canada; distributors cover the remainder of OUS and selected U.S. government, China, and Japan accounts [FACT] [https://agentii.ai/v/ISRG/sec172/page35]. The direct sales force is split into a capital-sales team and a clinical-sales team [FACT] [https://agentii.ai/v/ISRG/sec166/page14]. No direct:indirect revenue mix is disclosed — the largest disclosed channel-share metric is instead **acquisition mode**: 51% of FY2025 da Vinci placements went under operating leases, and 29.8% of the Q2-2026 installed base sits on ISRG's own balance sheet via operating leases [FACT + DEDUCTED] [https://agentii.ai/v/ISRG/sec166/page75], [https://agentii.ai/v/ISRG/sec172/page37]. The March 2026 $533.1M ab medica acquisition converted Italy, Spain, Portugal, Malta, and San Marino from distributor to direct distribution [FACT] [https://agentii.ai/v/ISRG/sec172/page14] — a deliberate shift toward direct control in high-value European markets.

## Mode 1_2 — Distribution Channel Analysis

**Distribution Model: Hybrid (direct-led, distributor-complemented)**

Direct sales organizations operate in: U.S.; Europe (10-K FY2025 wording: excluding Italy, Spain, Portugal, Greece, and Eastern European countries; Q2-2026 10-Q wording: excluding Greece and Eastern European countries); China through the Intuitive Surgical-Fosun Medical Technology (Shanghai) Co., Ltd. and Intuitive Surgical-Fosun (HongKong) Co., Ltd. JVs with Fosun Pharma; Japan; South Korea; India; Taiwan; Canada [FACT] [https://agentii.ai/v/ISRG/sec166/page14], [https://agentii.ai/v/ISRG/sec172/page35]. Distributors are used (a) for some U.S. government customers, (b) in China and Japan alongside direct organizations, and (c) in "the remainder of our OUS markets" [FACT] [https://agentii.ai/v/ISRG/sec166/page14].

Sales organization structure: a capital sales team (systems) and a clinical sales team (procedure support), selling into individual hospitals and IDN groups; initial system sale is a major capital purchase with a lengthy sales cycle [FACT] [https://agentii.ai/v/ISRG/sec166/page14]. Service infrastructure: field service engineers across U.S., Canada, Europe, Asia plus distributor relationships globally [FACT] [https://agentii.ai/v/ISRG/sec166/page11].

**Distribution Partners (disclosed)**: Fosun Pharma (China JV); formerly ab medica, Abex, Excelencia Robótica (European distributors, acquired March 1, 2026); unspecified distributors in remaining OUS markets [FACT] [https://agentii.ai/v/ISRG/sec166/page14], [https://agentii.ai/v/ISRG/sec172/page14].

**Current Channel Mix**: Direct : Indirect revenue split — **not disclosed** [Coverage Gap]. Disclosed proxies [DEDUCTED]:
- Geography: direct-channel countries generated ≥ the U.S.-plus-direct-OUS revenue; U.S. alone = 68% of FY2025 revenue [FACT] [https://agentii.ai/v/ISRG/sec166/page14]. Distributor-served "remainder OUS" is a subset of the 32% OUS share.
- Acquisition mode (system level): FY2025 da Vinci placements — 872 of 1,721 under operating leases (51%) plus 40 sales-type leases = 53% lease-financed [DEDUCTED from table] [https://agentii.ai/v/ISRG/sec166/page75].

**Historical Channel Trend (trailing 3 years)**:
- Operating-lease share of da Vinci placements: 2023: 48% → 2024: 51% → 2025: 51%; Q2-2026: 54% [FACT] [https://agentii.ai/v/ISRG/sec166/page75], [https://agentii.ai/v/ISRG/sec172/page36].
- Usage-based lease share of op-lease installed base (da Vinci): 1,023/2,227 (45.9%) 2023 → 1,492/2,799 (53.3%) 2024 → 1,810/3,210 (56.4%) 2025 [DEDUCTED] [https://agentii.ai/v/ISRG/sec166/page76] — a shift toward per-procedure (consumption) pricing.
- Direct-control expansion: March 1, 2026 — acquired da Vinci and Ion distribution businesses of ab medica, Abex, Excelencia Robótica for ~$533.1M cash (net of $32.6M receivable settlement); direct distribution assumed for Italy, Spain, Portugal, Malta, San Marino, and associated territories [FACT] [https://agentii.ai/v/ISRG/sec172/page14]. Cash used for business acquisition in H1-2026: $528M [FACT] [https://agentii.ai/v/ISRG/sec172/page45].
- Installed-base geography (Q2-2026): U.S. 6,615 / Europe 2,325 / Asia 2,111 / RoW 659 of 11,710 da Vinci systems; OUS = 43.5% of da Vinci installed base [FACT + DEDUCTED] [https://agentii.ai/v/ISRG/sec172/page35].

**Strategic Implication**: [VIEW] The direct organization plus balance-sheet leasing gives ISRG pricing control and customer intimacy (service contracts attach at placement: $95K–$225K/system/year) [https://agentii.ai/v/ISRG/sec166/page77], while usage-based leases convert capital equipment into consumption-based recurring revenue — tightening the razor-razorblade flywheel and raising SG&A burden (SG&A +10% YoY Q2-2026 to $617.9M) [FACT] [https://agentii.ai/v/ISRG/sec172/page42]. [VIEW] The ab medica buyout extends the direct model into Southern Europe, removing distributor margin leakage; distributor dependency risks (regulatory authorization, retention) remain for the long-tail OUS markets [https://agentii.ai/v/ISRG/sec166/page41].

## Coverage Gaps & Citations

- **Direct vs indirect revenue mix**: never disclosed numerically; the mode-1_2 template ratio (Direct : Indirect = 1 : XX) is not computable from filings — approximated structurally via geography and lease share only.
- **Distributor names**: not disclosed for "remainder OUS" markets.
- **Channel economics**: no distributor-margin or channel-discount disclosure.

**Citations (roll-up)**: sec166 pages 11, 14, 41, 75, 76, 77; sec172 pages 14, 35, 36, 37, 42, 45; 8-K 2026-03-02 via search_documents.

## Verification Table (number → tool call)

| Number | Value | Tool call |
|---|---|---|
| Direct sales markets | U.S., Europe excl. Greece/E.Europe, China-JV, Japan, S.Korea, India, Taiwan, Canada | sec172 page35 |
| Sales org split | capital + clinical teams | sec166 page14 |
| Op-lease share of dv placements | 51% FY2025 (48% 2023, 51% 2024); 54% Q2-2026 | sec166 page75; sec172 page36 |
| Lease-financed share FY2025 | 912/1,721 = 53% | sec166 page75 |
| Op-lease installed base | 3,210 dv + 360 Ion (12/31/25); 3,425 + 397 (6/30/26) | sec166 page76; sec172 page37 |
| ab medica acquisition | $533.1M cash, 2026-03-01; Italy/Spain/Portugal/Malta/San Marino direct | sec172 page14 |
| Q2-2026 installed base by region | U.S. 6,615; Europe 2,325; Asia 2,111; RoW 659 | sec172 page35 |
| Service contract fee (attach rate) | $95K–$225K/system/year | sec166 page77 |
| SG&A Q2-2026 | $617.9M (+10%) | sec172 page42 |
