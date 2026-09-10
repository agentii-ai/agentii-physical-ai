# Stage-0 Context Brief — Value Chain Profit Pool Map

> Q18: the retrieval-context brief the implement agents load before their first
> tool call. It is the contract between the plan and the retrieval layer — never
> a narrative summary.

**Thesis**: `theses/002-value-chain-profit-pool-map/`
**corpus_version**: `agentii-2026-09-10`
**constitution_pin**: `1.3.0`
**as_of**: `2026-09-10`

---

## 1. Retrieval keys (Q18)

| Stage | Keys |
|---|---|
| Mechanical prefilter | `ticker IN (NVDA, PH, ISRG, TSLA, AMBA, CGNX, SPCX)`; form types 10-K/10-Q/8-K + earnings transcripts; no price endpoints (market_data_stage: none) |
| Pillar FTS (full-text search) | PIL-1: `"gross margin"`, `"segment"`, `"motion"`, `"sensing"`, `"actuator"`, `"content"`; PIL-2: `"supplier"`, `"China"`, `"sourcing"`, `"tariff"`, `"rare earth"`, `"cost advantage"`; PIL-3: `"subscription"`, `"recurring"`, `"software"`, `"royalty"`, `"per unit"`, `"installed base"` |
| Cold-start fallback | T-001 artifacts under `../001-physical-ai-technology-baseline/artifacts/{TICKER}/` — the evidence baseline; then `search_by_analogue` / `search_knowledge_entries` for profit-pool and pricing-power frameworks |

**Retrieval discipline** (constitution P4): every material number must carry the
inline `agentii.ai/v/{ticker}/{citation_id}/{page}` citation from a call the agent
actually made; unframed numbers void the artifact. AMBA/CGNX tag only
`RevenueFromContractWithCustomerExcludingAssessedTax` — verify revenue across
multiple periods, not multiple concepts (the single-concept pattern T-001
documented).

## 2. Strategy candidates (Q7 — top-N with verdicts)

| # | Strategy | method_selection | Rationale |
|---|---|---|---|
| 1 | Layer-margin comparison | **USE** | The durability falsifier (motion GM vs model GM) is a direct margin-table comparison: PH Motion Systems segment margin vs NVDA consolidated GM vs ISRG product GM — all retrievable |
| 2 | Recurring-per-unit decomposition | **USE** | PIL-3's falsifier: ISRG recurring revenue per installed system (84% of $10.06B over 12,101 installed systems FY2025 — ~12.8k by Q2-2026, T-001 audited) vs the $5,000/unit threshold |
| 3 | Supplier/cost-structure proxy for China ratio | **USE (proxy only)** | Filing-derived: disclosed supplier concentration, tariff disclosures (PH's IEEPA refund, NVDA's China restrictions), sourcing statements. The ratio itself is teardown data — `[VIEW]` only |
| 4 | BOM-share direct measurement | **REJECT** | No humanoid teardown or 10-K BOM split exists in the corpus (T-001 PIL-2 `indeterminate`). Attempting it wastes the budget |
| 5 | Knowledge-store profit-pool frameworks | **USE IF PRESENT** | `search_knowledge_entries` for profit-pool/pricing-power frameworks; T-001 recorded the stores returning empty for some queries — record honestly, never substitute invented references |

## 3. Framed references (T-001 evidence baseline, carried)

<ref:001-physical-ai-technology-baseline>
- ISRG: product GM 66.3%, total GM 66.0% FY2025; 84% recurring; I&A ~$1.83K/procedure — the integrated-robotics margin anchor.
- NVDA: FY2026 GM 71.1%; Q1 FY2027 74.9%; Edge Computing $6.4B — the model/compute-layer margin anchor.
- PH: Motion Systems $3,580M FY2026 (+7.2%); DI segment op margin 23.8%; consolidated GM 37.7% — the motion-layer margin anchor.
- TSLA: FY2025 automotive GM 17.8%; capex >$25B guided — the vertically-integrated cost reference.
- SPCX: H1-2026 capex $28.5B, 82.7% AI — the demand-side pool pull.
- AMZN: (not in this universe, but T-001's >1M-robot fleet data is the deployment-economics reference frame.)
</ref:001-physical-ai-technology-baseline>

## 4. Known retrieval hazards (carried from T-001)

- `get_segment_data` product-axis values conflicted with PH's 10-K (gold $3,830M
  vs filed $3,341M FY2025 Motion Systems) — **the 10-K wins; flag the conflict**.
- AMZN-class fiscal-calendar registry mismatches possible for other names — verify
  period_end against the filing header before trusting fiscal-year filters.
- XBRL single-revenue-concept pattern (ISRG/TSLA/PH/SPCX/AMBA/CGNX) — the P2.1
  two-concept rule is satisfied by multi-period + dimension triangulation,
  reconciled to income-statement tables.
- Transcripts may cite source UUIDs instead of `secN` citation_ids — carry the
  UUID link form when that is all the corpus returns, and flag it.
