---
artifact_id: "002-SPCX-supply-chain-20260911"
thesis_id: "002-value-chain-profit-pool-map"
ticker: SPCX
skill: supply-chain
mode: default
affix: supply-chain-map
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "8cb3ac1de486"
as_of: 2026-09-11
entity_claims:
  - entity: SPCX
    metric: capital_expenditure_usd
    value: 28476000000
    unit: USD
    period: H1-2026
    source: "10-Q:page9"
    retrieved_at: 2026-09-11
    tag: "[FACT]"
  - entity: SPCX
    metric: ai_segment_capex_share_pct
    value: 82.7
    unit: pct
    period: H1-2026
    source: "10-Q:page31"
    retrieved_at: 2026-09-11
    tag: "[DEDUCTED]"
citations:
  - "https://agentii.ai/v/SPCX/sec8/9"
  - "https://agentii.ai/v/SPCX/sec8/13"
  - "https://agentii.ai/v/SPCX/sec8/14"
  - "https://agentii.ai/v/SPCX/sec8/30"
  - "https://agentii.ai/v/SPCX/sec8/31"
  - "https://agentii.ai/v/SPCX/sec8/36"
  - "https://agentii.ai/v/SPCX/sec8/40"
  - "https://agentii.ai/v/SPCX/sec8/45"
  - "https://agentii.ai/v/SPCX/sec8/49"
  - "https://agentii.ai/v/SPCX/sec7/6"
  - "https://agentii.ai/v/SPCX/sec7/9"
  - "https://agentii.ai/v/SPCX/sec9/2"
  - "XBRL:spcx-20260630.htm — RevenueFromContractWithCustomerExcludingAssessedTax facts (4)"
  - "XBRL:spcx-20260630.htm — us-gaap:Revenues facts (0)"
  - "XBRL:spcx-20260630.htm — PaymentsToAcquirePropertyPlantAndEquipment facts (2)"
pillars_addressed: [PIL-1, PIL-2]
claim_state: pinned
key_metrics:
  ai_segment_capex_usd: 23551000000
  space_segment_capex_usd: 2226000000
  connectivity_segment_capex_usd: 2699000000
  total_capex_yoy_multiple: 4.1
  ai_capex_q2_yoy_multiple: 21.1
  ai_capex_share_q2_2025_pct: 26.5
  nameplate_compute_draw_gw: 1.4
  tesla_megapack_purchases_usd: 329000000
  valor_lease_debt_usd: 13329000000
  echostar_spectrum_consideration_usd: 19600000000
  customer_a_revenue_share_pct: 17.9
  customer_b_revenue_share_pct: 12.2
  backlog_usd: 47461000000
  rfcc_excluding_assessed_tax_usd: 12508000000
  us_gaap_revenues_fact_count: 0
  cloud_service_agreements_contracted_sales_usd: 14100000000
conclusions:
  - "PIL-1 demand-side pull confirmed: H1-2026 capex $28.5B with AI segment 82.7% — end-market demand flows to the compute layer, dwarfing motion/sensing-layer economics."
  - "AI capex inflected from 26.5% of total (Q2-2025) to 86.2% (Q2-2026); nameplate compute draw 1.4GW, 3.5x YoY."
  - "SPCX supply chain is US-centric and only partially disclosed: Tesla (Megapacks), Valor (AI hardware leases), EchoStar (spectrum); servers/networking suppliers unnamed."
  - "No long-term binding purchase orders with parts/raw-materials suppliers — a structurally flexible, capital-intense sourcing model."
  - "Customer concentration moderate: two >10% customers (17.9% and 12.2% of H1 revenue); one AI-only."
  - "P2.1 anomaly verified: revenue tagged under RFCCExcludingAssessedTax ($12.508B H1-2026); us-gaap:Revenues has zero facts — tagging anomaly, not absent revenue."
facts_count: 36
deducted_count: 11
views_count: 5
citation_count: 15
---

# SPCX Supply-Chain Map — Value Chain Profit Pool Map (002)

## 1. Executive Summary

SPCX (Space Exploration Technologies Corp.; NASDAQ; IPO June 2026) has a one-quarter public corpus: the Q2-2026 10-Q plus eight 8-Ks. The filings settle PIL-1's demand-side question decisively: H1-2026 capital expenditures were $28,476M — 4.1x YoY — of which the AI segment consumed $23,551M, an 82.7% share [DEDUCTED], confirming the T-001 estimate and showing end-market demand flowing overwhelmingly to the compute layer while Space took just $2,226M [FACT]. Q2 AI capex of $15,828M was 21.1x its Q2-2025 level [DEDUCTED]; nameplate compute draw reached 1.4GW, 3.5x YoY [DEDUCTED]. The disclosed supply chain is US-centric: Tesla Megapacks ($329M H1-2026 purchases), Valor AI-hardware leases (failed sale-leaseback, $13,329M debt [DEDUCTED]), EchoStar spectrum ($19.6B). Customer A is 17.9% of H1 revenue across all three segments; AI-only Customer B is 12.2% [FACT]. P2.1 verified: XBRL tags revenue under RevenueFromContractWithCustomerExcludingAssessedTax ($12,508M H1-2026) with zero us-gaap:Revenues facts — a tagging anomaly, not absent revenue [FACT]. Backlog $47,461M; no long-term supplier purchase orders [FACT].

## 2. Data Sources

| Source | Citation | Pages read |
|---|---|---|
| 10-Q (Q2-2026, filed 2026-08-04, accession 0001628280-26-052535) | sec8 | 9, 13, 14, 30, 31, 36, 40, 45, 49 (outline: all 55) |
| 8-K earnings release (2026-08-04, accession 0001628280-26-052515) | sec7 | 6, 9 (outline: all 13) |
| 8-K Cursor/Anysphere merger completion (2026-08-14, accession 0001628280-26-056945) | sec9 | 2 (outline: all 96) |
| XBRL facts (gold.xbrl_facts), source_file spcx-20260630.htm | — | RFCCExcludingAssessedTax, Revenues, PaymentsToAcquirePropertyPlantAndEquipment |

Preflight: search_companies (SPCX = SpaceX, CIK 0001181412), get_ticker_coverage (8 SEC filings, 1,517 XBRL facts, 1 transcript, 7 populated sources), get_company_fiscal_calendar (FYE Dec-31, source=default — see §5 data-quality note). Layer 1: search_sec_filings returned 9 filings (sec1–sec9). Layer 2/3: read_source_outline + read_source_pages on sec8, sec7, sec9 as above. The one earnings-call-transcript record in coverage carries no citation_id in the index and is not retrievable through the Layer-1 tool response — logged as a coverage gap (§5).

## 3. Analysis

### 3.1 Capex structure — the demand-side pull (PIL-1)

SPCX is the thesis's demand-side counterpoint: where the end-market demand for physical-AI capability actually spends. The Q2-2026 10-Q segment disclosure makes the flow explicit.

**Total capex.** Cash-flow purchases of property, plant, and equipment were $28,476M for H1-2026 versus $6,965M for H1-2025 [FACT] (https://agentii.ai/v/SPCX/sec8/9). The same figure is tagged in XBRL: us-gaap:PaymentsToAcquirePropertyPlantAndEquipment = 28,476,000,000 (H1-2026, is_primary=true, source_authority=2) [FACT] (XBRL:spcx-20260630.htm). YoY growth of 4.1x [DEDUCTED].

**Segment split (H1-2026).** Space $2,226M, Connectivity $2,699M, AI $23,551M, total $28,476M [FACT] (https://agentii.ai/v/SPCX/sec8/31). AI share = 23,551 / 28,476 = **82.7%** [DEDUCTED] — exactly the T-001 anchor, now filing-verified.

**Q2-2026.** Space $1,174M, Connectivity $1,367M, AI $15,828M, total $18,369M [FACT] (https://agentii.ai/v/SPCX/sec8/30). AI share = 86.2% [DEDUCTED], up from 26.5% in Q2-2025 (AI $749M of $2,825M) [FACT] (https://agentii.ai/v/SPCX/sec8/31) [DEDUCTED share]. AI capex grew 21.1x YoY in Q2 [DEDUCTED]; H1-2025 AI capex was $3,316M, a 47.6% share [FACT] (https://agentii.ai/v/SPCX/sec7/6) [DEDUCTED share]. The inflection from ~27% (Q2-2025) to ~86% (Q2-2026) of capex is the quantitative shape of the demand shift this thesis argues [DEDUCTED framing].

**Capacity metric.** Nameplate compute draw — GPUs installed x all-in power draw — was 1.4GW at 2026-06-30 versus 0.4GW a year earlier [FACT] (https://agentii.ai/v/SPCX/sec8/36); Q1-2026 was 1.0GW [FACT] (https://agentii.ai/v/SPCX/sec7/9). 3.5x YoY [DEDUCTED].

**Balance-sheet evidence.** Servers and networking equipment (the compute hardware stock) was $34,771M at 2026-06-30 versus $22,694M at 2025-12-31; data center infrastructure $3,991M; construction-in-progress $12,554M versus $4,604M; total PP&E net $65,736M [FACT] (https://agentii.ai/v/SPCX/sec8/14). H1-2026 depreciation $5,064M versus $2,547M H1-2025 [FACT] (https://agentii.ai/v/SPCX/sec8/14). Q2-2026 AI-segment D&A alone was $1,885M [FACT] (https://agentii.ai/v/SPCX/sec8/30).

**PIL-1 read.** The AI segment's single-quarter capex ($15.8B) is ~4.4x the entire FY2026 motion-systems revenue anchor for PH ($3.58B, entities.md map) [DEDUCTED]. End-market dollars are accumulating at the compute layer at a scale the actuation/sensing pools cannot match in this corpus. The counterpoint holds: demand-side pull is compute-led (82.7% share), not motion-led.

### 3.2 Supplier relationships (PIL-2 inputs)

SPCX discloses three named supplier/related-party relationships and a general sourcing policy:

- **Tesla, Inc. (Megapacks — energy storage for AI data centers).** Purchases of $295M in Q2-2026 and $329M in H1-2026, recorded in PP&E [FACT] (https://agentii.ai/v/SPCX/sec8/30); the cash-flow statement confirms $329M related-party PP&E purchases in H1-2026 [FACT] (https://agentii.ai/v/SPCX/sec8/9). For full-year 2025 (as of 2025-12-31): $506M of Megapacks and $131M of Cybertrucks at MSRP [FACT] (https://agentii.ai/v/SPCX/sec8/30). Megapacks are the energy-storage backbone of the AI data-center build-out — a US-sourced hardware input.
- **Valor Equity Partners (AI infrastructure hardware leases).** April 2026 equipment-lease agreement for AI infrastructure hardware; deemed a failed sale-leaseback [FACT] (https://agentii.ai/v/SPCX/sec8/30). Recorded debt of $2,039M current + $11,290M non-current at 2026-06-30 — $13,329M combined [DEDUCTED] — versus $455M + $4,052M ($4,507M [DEDUCTED]) at 2025-12-31 [FACT] (https://agentii.ai/v/SPCX/sec8/30). Related interest expense: $327M Q2-2026 / $513M H1-2026 [FACT] (https://agentii.ai/v/SPCX/sec8/30). Valor's founder/CEO Antonio Gracias is a SpaceX director [FACT] (https://agentii.ai/v/SPCX/sec8/30).
- **EchoStar (spectrum — Connectivity input).** License Purchase Agreement: ~$19.6B total consideration — $11.1B equity (261.8M Class A shares) plus up to $8.5B payoff of designated EchoStar debt [FACT] (https://agentii.ai/v/SPCX/sec8/49). FCC approval 2026-05-12; Spectrum Transfer Closing 2026-05-22; $856M paid of the $1,241M expected in 2026 under the Spectrum Credit Agreement [FACT] (https://agentii.ai/v/SPCX/sec8/49).
- **General sourcing policy.** "Because we do not have long-term purchase orders for these parts and raw materials, future purchases may result in material cash commitments" [FACT] (https://agentii.ai/v/SPCX/sec8/49). No supplier geographic concentration is disclosed — see §5.
- **Vertical integration note.** Cursor (Anysphere) merger completed 2026-08-14 for ~$60B implied equity value, 389.3M Class A shares issued [FACT] (https://agentii.ai/v/SPCX/sec9/2) — supply-chain-relevant as it pulls an AI application layer (coding tool) inside the compute owner, and the merger agreement references a "Compute Agreement" between the parties [FACT] (https://agentii.ai/v/SPCX/sec9/2, outline page81).

**PIL-2 read.** SPCX's disclosed procurement is US-centric (Tesla, Valor, EchoStar). The 10-Q does not disclose any China-sourced BOM split, so the PIL-2 falsifier (non-China/China humanoid BOM cost ratio) cannot be tested from this corpus — the SPCX contribution is a US cost-stack anchor at scale, not a ratio input (see §5 gap and Verification table).

### 3.3 Customer concentration and revenue structure

- Concentration table: Customer A = 18.3% of Q2-2026 and 17.9% of H1-2026 revenue, spanning **all three segments**; Customer B = 19.5% (Q2) / 12.2% (H1), AI segment only [FACT] (https://agentii.ai/v/SPCX/sec8/14). No other customer exceeded 10% [FACT] (https://agentii.ai/v/SPCX/sec8/14). Names are not disclosed; an all-segments customer is most plausibly the US government (launch + Starshield + AI) but the filing does not say so [VIEW].
- Segment revenue H1-2026: Space $1,581M, Connectivity $7,548M, AI $3,379M, total $12,508M [FACT] (https://agentii.ai/v/SPCX/sec8/31). Q2-2026 consolidated revenue $7,814M (+91.9% YoY); H1 +53.7% [FACT] (https://agentii.ai/v/SPCX/sec8/40).
- AI Solutions & Infrastructure revenue (the compute-as-a-service line): $2,194M Q2-2026 versus $311M Q2-2025 [FACT] (https://agentii.ai/v/SPCX/sec8/13). The earnings release attributes growth to "new Cloud Services Agreements" totaling $14.1B in contracted sales, producing $1.6B of incremental Q2 AI infrastructure revenue [FACT — company-disclosed in earnings release] (https://agentii.ai/v/SPCX/sec7/9).
- Demand backlog $47,461M; deferred revenue $14,286M at 2026-06-30 [FACT] (https://agentii.ai/v/SPCX/sec8/14).
- Inventory $2,718M (raw materials $1,122M, WIP $875M, finished goods $721M) [FACT] (https://agentii.ai/v/SPCX/sec8/14) — modest relative to capex, consistent with a services/launch-plus-connectivity-kit model rather than a component-inventory-heavy manufacturer.

### 3.4 P2.1 self-verification — the XBRL tagging anomaly

T-001's P2.1 note claimed "RFCCExcludingAssessedTax $12.508B H1-2026 vs Revenues=0." Verified by direct retrieval [FACT]:

- us-gaap:RevenueFromContractWithCustomerExcludingAssessedTax for SPCX returns 4 duration facts: H1-2026 = $12,508,000,000; Q2-2026 = $7,814,000,000; H1-2025 = $8,138,000,000; Q2-2025 = $4,071,000,000 — all is_primary=true, source_authority=2, source_file spcx-20260630.htm [FACT] (XBRL:spcx-20260630.htm).
- us-gaap:Revenues for SPCX returns **zero facts** even with include_all_sources=true [FACT] (XBRL:spcx-20260630.htm).

The income statement itself is intact — Revenue of $7,814M (Q2) and $12,508M (H1) appear on the face [FACT] (https://agentii.ai/v/SPCX/sec8/40). So the anomaly is a tagging choice, not absent revenue: the filer tagged the top line only under the 606-style concept and never under us-gaap:Revenues. Any downstream consumer reading us-gaap:Revenues sees SPCX with zero revenue; thesis pipelines must key on RevenueFromContractWithCustomerExcludingAssessedTax for SPCX. This is a retrieval-correctness finding, not a falsification input.

### 3.5 Forward claims — promotional, tagged [VIEW]

Per the T-001 risk note, forward compute statements are promotional: the "continued build-out of Colossus II and significant incremental capacity under construction" [VIEW] (https://agentii.ai/v/SPCX/sec7/9); Grok 4.5 / "1.5 trillion-parameter V9 foundation model" [VIEW] (https://agentii.ai/v/SPCX/sec7/9); the Q2-2026 statement that Cursor was "expected to close in Q3 2026" [VIEW] (https://agentii.ai/v/SPCX/sec7/9) — subsequently realized by the 2026-08-14 completion 8-K [FACT] (https://agentii.ai/v/SPCX/sec9/2). Data-quality flag: the same release says compute expanded "from 0.4 GW in Q2 2026," which conflicts with its own 1.4GW Q2-2026 figure — an apparent typo for Q2 2025 [VIEW] (https://agentii.ai/v/SPCX/sec7/9).

## 4. Key Metrics

See frontmatter `key_metrics` (16 structured entries) and `entity_claims` (2 map-mandated entries). Headline values:

| Metric | Value | Period | Tag | Citation |
|---|---|---|---|---|
| Capital expenditures | $28,476M | H1-2026 | [FACT] | https://agentii.ai/v/SPCX/sec8/9 |
| AI segment capex | $23,551M | H1-2026 | [FACT] | https://agentii.ai/v/SPCX/sec8/31 |
| AI capex share | 82.7% | H1-2026 | [DEDUCTED] | https://agentii.ai/v/SPCX/sec8/31 |
| AI capex share | 86.2% | Q2-2026 | [DEDUCTED] | https://agentii.ai/v/SPCX/sec8/30 |
| AI capex share | 26.5% | Q2-2025 | [DEDUCTED] | https://agentii.ai/v/SPCX/sec8/31 |
| Nameplate compute draw | 1.4 GW | 2026-06-30 | [FACT] | https://agentii.ai/v/SPCX/sec8/36 |
| Tesla Megapack purchases | $329M | H1-2026 | [FACT] | https://agentii.ai/v/SPCX/sec8/30 |
| Valor lease debt | $13,329M | 2026-06-30 | [DEDUCTED] | https://agentii.ai/v/SPCX/sec8/30 |
| EchoStar spectrum consideration | $19.6B | closing 2026 | [FACT] | https://agentii.ai/v/SPCX/sec8/49 |
| Customer A / B revenue share | 17.9% / 12.2% | H1-2026 | [FACT] | https://agentii.ai/v/SPCX/sec8/14 |
| Backlog | $47,461M | 2026-06-30 | [FACT] | https://agentii.ai/v/SPCX/sec8/14 |
| RFCCExcludingAssessedTax | $12,508M | H1-2026 | [FACT] | XBRL:spcx-20260630.htm |
| us-gaap:Revenues fact count | 0 | all | [FACT] | XBRL:spcx-20260630.htm |

## 5. Coverage Gaps & Citations

**Gaps:**
1. **Earnings-call transcript (2026-08-04) not retrievable** — the single transcript record in get_ticker_coverage has no citation_id in the Layer-1 index; read_source_outline without citation_id returns 404. Management commentary on supplier names and customer identity is therefore absent from this artifact.
2. **Servers/networking suppliers unnamed** — $34,771M of compute hardware on the balance sheet with no disclosed supplier (GPU/OEM vendors not named in the 10-Q).
3. **No geographic concentration disclosure** — no revenue-by-geography or sourcing-by-country table in the 10-Q; PIL-2's China/non-China BOM split cannot be proxied from this corpus.
4. **Customer A and B identity undisclosed** — flagged [VIEW].
5. **Fiscal calendar is default-sourced** — FYE Dec-31 with the tool's cross-validation hint ("No XBRL data available for this ticker — fiscal calendar may be inaccurate"); the filing dates themselves (2026-06-30 quarter end, 2026-08-04 filing) are consistent with a Dec-31 fiscal year, but the calendar endpoint's hint is logged as a data-quality caveat.
6. **One-quarter history** — no multi-period trend beyond H1-2026 vs H1-2025 comparatives inside the single 10-Q; the skill's 4-quarter default lookback is not satisfiable.
7. **Forward compute targets** — treated as [VIEW] per the T-001 risk note.

**Citation index (roll-up):** sec8 pp. 9, 13, 14, 30, 31, 36, 40, 45, 49 (10-Q); sec7 pp. 6, 9 (earnings release 8-K); sec9 p. 2 (Cursor merger completion 8-K); XBRL facts in spcx-20260630.htm (RFCCExcludingAssessedTax ×4, Revenues ×0, PaymentsToAcquirePropertyPlantAndEquipment ×2). See frontmatter `citations` (15 entries).

## 6. Verification table

| Check | Expected (T-001) | Retrieved | Status |
|---|---|---|---|
| P2.1 RFCCExcludingAssessedTax H1-2026 | $12.508B | $12,508,000,000 (is_primary, 10-Q XBRL) | Verified [FACT] |
| P2.1 us-gaap:Revenues = 0 | 0 facts | 0 facts (include_all_sources=true) | Verified [FACT] — tagging anomaly, not absent revenue (face shows $12,508M H1) |
| AI segment capex share H1-2026 | 82.7% | 23,551 / 28,476 = 82.7% | Verified [DEDUCTED] |
| Total capex H1-2026 | $28.5B | $28,476M (CF p.9 + XBRL) | Verified [FACT] |
| Tesla Megapack supplier relationship | expected present | $329M H1-2026; $506M FY2025 | Verified [FACT] |
| Valor/EchoStar agreements | expected present | $13.3B lease debt; $19.6B spectrum | Verified [FACT]/[DEDUCTED] |
| Customer concentration | sought | A 17.9% (all segments), B 12.2% (AI) | Verified [FACT], identity undisclosed [VIEW] |
| Supplier purchase commitments | sought | No long-term binding POs disclosed | Verified [FACT] |
| Geographic/supplier-country split | sought | Not disclosed | Gap — PIL-2 BOM ratio not testable here |

Counts: 36 [FACT], 11 [DEDUCTED], 5 [VIEW], 15 citations. No price data used (EchoStar consideration reported as shares + $ value per the filing; no market prices).
