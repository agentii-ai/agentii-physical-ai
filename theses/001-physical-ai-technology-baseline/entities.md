# Entities — Physical AI Technology Baseline

> Q20/Q36: the `entity_claims` schema and the entity/metric map for this thesis.
>
> **Q42 status: bars schema NOT REQUIRED.** This thesis is `market_data_stage: none`.
> No phase retrieves `get_price_history`; every pillar is falsifiable from filings,
> transcripts and technical disclosure. `implement` will not refuse for its absence.
> If Phase 5 introduces a price-based catalyst trigger, this file must gain the bars
> schema and the thesis must be re-planned as `market_data_stage: early`.

---

## entity_claims schema

```yaml
entity_claims:
  - entity: ISRG
    metric: installed_base_systems
    value: 0                 # to be populated during implement
    unit: count
    period: 2026Q2
    source: "xbrl:<concept>|10-K:pageNN|transcript:YYYY-MM-DD"
    retrieved_at: 2026-09-10T00:00:00-04:00
    observed_at: null        # market-derived claims only (Q71) — null here
```

**Field rules**

- `entity` — ticker, confirmed retrievable via `search_documents` before use (P2.1).
  Never inferred from a fuzzy match; `ALNT` resolves to Alnylam and must be rejected.
- `metric` — snake_case, must appear in the map below.
- `source` — one of `xbrl:<concept>`, `10-K:pageNN`, `10-Q:pageNN`, `transcript:<date>`,
  `teardown:<publisher>`, `trade_press:<outlet>:<date>`.
- `observed_at` — populated **only** for market-derived claims (Q71); null for all
  claims in this thesis.
- `retrieved_at` — ISO-8601 with offset.

---

## Entity / metric map

| entity | metric | unit | source class | pillar |
|---|---|---|---|---|
| NVDA | robotics_and_simulation_revenue_share_of_total_pct | pct | 10-K segment data | PIL-1 |
| NVDA | datacenter_revenue_growth_yoy | pct | 10-K segment data | PIL-1 |
| NVDA | r_and_d_expense_growth_yoy | pct | XBRL | PIL-1 |
| ISRG | installed_base_systems | count | 10-K / transcript | PIL-3 |
| ISRG | procedure_volume_growth_yoy | pct | 10-K / transcript | PIL-3 |
| ISRG | system_utilization_rate | pct | transcript | PIL-3 |
| ISRG | gross_margin | pct | XBRL:us-gaap:GrossProfit / Revenues | PIL-3 |
| TSLA | fleet_size_deployed | count | 10-K / transcript | PIL-1, PIL-4 |
| TSLA | fsd_or_autonomy_miles_cumulative | count | transcript | PIL-1 |
| TSLA | humanoid_revenue_disclosure_present | bool | 10-K segment data | PIL-4 |
| AMZN | robotics_units_deployed | count | 10-K / transcript | PIL-3 |
| AMZN | fulfillment_automation_capex | usd | 10-K segment data | PIL-3 |
| AMZN | cost_per_unit_fulfillment | usd | 10-K | PIL-3 |
| *(industry)* | teleop_cost_per_hour | usd | teardown / trade press | PIL-1 |
| *(industry)* | egocentric_capture_cost_per_hour | usd | teardown / trade press | PIL-1 |
| *(industry)* | embodied_dataset_hours_vs_llm_pretrain_token_gap_order_of_magnitude | orders | technical publication | PIL-1 |
| PH | motion_systems_segment_operating_margin | pct | 10-K segment data | PIL-2 |
| PH | motion_systems_segment_revenue | usd | 10-K segment data | PIL-2 |
| *(industry)* | actuator_share_of_humanoid_bom_pct | pct | teardown | PIL-2 |
| *(industry)* | planetary_roller_screw_share_of_bom_pct | pct | teardown | PIL-2 |
| *(industry)* | humanoid_mtbf_hours_in_commercial_deployment | hours | company / fleet operator | PIL-3 |
| *(industry)* | general_purpose_humanoid_commercial_units_deployed | count | company disclosure | PIL-4 |

**Industry-row rule.** Metrics marked *(industry)* have no single entity issuer. They
are recorded against `entity: INDUSTRY` with `source` naming the publisher and date.
They may satisfy a pillar falsifier but may **not** be used in a valuation model, since
they are estimates rather than audit-grade disclosures. This distinction matters
because three of T-001's four pillar thresholds are industry metrics.

---

## Ticker verification log (P2.1 — mandatory)

Every entity must be confirmed retrievable before its claims are used.

| ticker | search_sec_filings | search_documents | search_xbrl_facts (2 concepts) | verdict |
|---|---|---|---|---|
| NVDA | 169 | present | 169 (+99 revenue facts) | **retrievable** |
| ISRG | 173 | present | 63 revenue facts | **retrievable** |
| TSLA | 259 | 92 | 63,523 facts | **retrievable** |
| AMZN | 86 | present | present | **retrievable** |
| PH | 166 | 80 | 36 revenue facts (FY26 rev $21.499B) | **retrievable — added to T-001 universe in plan rev. 2 to carry PIL-2** |
| EMR | 67 | present | present | retrievable (used in PIL-2 context) |

**No entity in this thesis was declared out-of-universe from an index lookup.** Each
row above was confirmed by direct retrieval, per the rule added after the 2026-09-10
false-negative incident.
