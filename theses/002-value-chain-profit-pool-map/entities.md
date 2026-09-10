# Entities — Value Chain Profit Pool Map

> `entity_claims` schema + the entity/metric map. Every material number an
> artifact emits must be a structured `{entity, metric, value, unit, period,
> source, retrieved_at}` claim; prose-form claims are rejected (G1 — the T-001
> entity-index vacuity finding). **No bars schema** — this thesis is
> `market_data_stage: none` (Q42 not triggered).

---

## 1. entity_claims schema (binding at implement)

```yaml
entity_claims:
  - entity: PH
    metric: motion_systems_revenue_usd
    value: 3580000000
    unit: USD
    period: 2026Q4          # fiscal period of the source filing
    source: "10-K:page44"
    retrieved_at: 2026-09-10
```

## 2. Entity / metric map

| entity | metric | unit | period | notes |
|---|---|---|---|---|
| NVDA | consolidated_gross_margin_pct | pct | FY2026 / Q1-FY2027 | model/compute-layer margin anchor |
| NVDA | edge_computing_revenue_usd | USD | Q1-FY2027 | robotics-adjacent platform revenue |
| PH | motion_systems_revenue_usd | USD | FY2026 | actuation-layer pool size |
| PH | diversified_industrial_segment_operating_margin_pct | pct | FY2026 | motion-layer profitability |
| PH | consolidated_gross_margin_pct | pct | FY2026 | cross-check anchor |
| ISRG | product_gross_margin_pct | pct | FY2025 | integrated-system margin anchor |
| ISRG | recurring_revenue_share_pct | pct | FY2025 / Q2-2026 | per-unit subscription base for PIL-3 |
| ISRG | installed_base_units | units | FY2025 / Q2-2026 | denominator for per-unit revenue |
| ISRG | revenue_per_procedure_usd | USD | Q2-2026 | I&A per procedure (~$1.83K anchor) |
| TSLA | automotive_gross_margin_pct | pct | FY2025 | vertically-integrated cost reference |
| TSLA | automotive_cost_of_revenue_usd | USD | FY2025 | COGS structure for cost-stack proxies |
| AMBA | revenue_usd | USD | FY2026 | sensing-silicon layer size ($390.7M FY26) |
| AMBA | gross_margin_pct | pct | FY2026 | sensing-layer margin |
| CGNX | revenue_usd | USD | FY2025 | industrial vision layer size ($994.4M FY25) |
| CGNX | gross_margin_pct | pct | FY2025 | sensing-layer margin |
| SPCX | capital_expenditure_usd | USD | H1-2026 | demand-side pool pull ($28.5B) |
| SPCX | ai_segment_capex_share_pct | pct | H1-2026 | compute-led demand evidence (82.7%) |

**Metric discipline**: only metrics appearing above (or derived arithmetic on
them, stated as `[DEDUCTED]`) may enter `entity_claims`. New metrics discovered
during retrieval are appended to this map by the implement dispatcher, never
invented inline.

## 3. Falsifier-threshold anchors (carried from T-001, for the synthesis)

| falsifier | threshold | test inputs |
|---|---|---|
| PIL-1a `actuation_plus_sensing_share_of_bom_pct` | < 55 falsifies | filing proxies only; teardown figures `[VIEW]` |
| PIL-1b `motion_model_gm_gap_change_pp` | < -10 falsifies (gap falls >10pp over 3 FYs) | PH/NVDA/ISRG multi-year GM series; motion GM minus model GM, pp |
| PIL-2 `nonchina_to_china_humanoid_bom_cost_ratio` | < 2.0 falsifies | proxies only — Deviation Register entry, expiry 2026-10-10 |
| PIL-3 `model_layer_revenue_per_deployed_unit_usd` | > 5000 falsifies | ISRG recurring revenue ÷ installed base; NVDA platform software |
