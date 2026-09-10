# Contracts — Value Chain Profit Pool Map

> Output frontmatter schemas and `requires:` declarations for artifacts produced
> by this thesis. Downstream consumers (`converge`, `implement`) read these
> declarations; an artifact whose frontmatter fails its schema is rejected rather
> than partially consumed.

---

## 1. Per-ticker artifact schema

Applies to every `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md` file produced under
this thesis.

```yaml
---
artifact_id: "002-PH-supply-chain-20260910-1930"
thesis_id: "002-value-chain-profit-pool-map"
ticker: PH                       # must be P2.1-verified retrievable
skill: supply-chain
mode: default
affix: supply-chain-map

# Pins — an artifact is only valid against the pins it was produced under
constitution_pin: "1.3.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "<content-hash>"       # per-skill, from skill_pins.jsonl
as_of: 2026-09-10

# Evidence discipline (P4) — STRUCTURED claims only (G1: prose claims rejected)
entity_claims:
  - entity: PH
    metric: motion_systems_revenue_usd   # must exist in entities.md §2 map
    value: 3580000000
    unit: USD
    period: 2026Q4
    source: "10-K:page44"
    retrieved_at: 2026-09-10

citations:                        # inline citation targets, agentii.ai/v/... form
  - "agentii.ai/v/PH/sec166/44"

pillars_addressed: [PIL-1, PIL-2]
claim_state: pinned               # pinned|superseded|retired|retired_by_ic|pending_review|stale_price|pending_gate
---
```

**requires:**

- `ticker` confirmed retrievable by direct retrieval (P2.1; single-concept taggers
  verified across multiple periods). Declaration: `requires: p2_1_verified_ticker`
- every `entity_claims[].metric` present in `entities.md` entity/metric map.
  Declaration: `requires: metric_in_entity_map`
- every material quantitative statement followed inline by its citation.
  Declaration: `requires: inline_citation` (P4)
- `constitution_pin` equal to the workspace's current ratified version.
  Declaration: `requires: constitution_pin_current`
- **Round-3 evaluation rules (clarify 2026-09-10)**: PIL-1a/PIL-2 evidence is
  SEC-filing-derived only; teardown figures enter exclusively as `[VIEW]` with
  the macro-plan origin stated. PIL-3 model-layer revenue includes per-unit
  software/subscription revenue. Declaration: `requires: round3_falsifier_rules`

---

## 2. Cross-stock synthesis schema

Applies to `_cross/002-value-chain-profit-pool-map_synthesis.md`.

```yaml
---
artifact_id: "002-cross-profit-pool-map-20260910"
thesis_id: "002-value-chain-profit-pool-map"
type: cross_synthesis
tickers_covered: [NVDA, PH, ISRG, TSLA, AMBA, CGNX, SPCX]
pillars_synthesized: [PIL-1, PIL-2, PIL-3]
pillar_verdicts:
  PIL-1: supported | refuted | indeterminate
  PIL-2: supported | refuted | indeterminate
  PIL-3: supported | refuted | indeterminate
constitution_pin: "1.3.0"
as_of: 2026-09-10
profit_pool_map:
  layer_rankings: []              # layers ordered by durable-margin evidence
  china_cost_ratio_estimate: null # interval or null if unmeasurable
  confidence: low | medium | high
---
```

**requires:**

- every `pillar_verdicts` entry backed by a stated falsifier test result (both
  PIL-1 falsifiers tested separately).
  Declaration: `requires: falsifier_evidence`
- `indeterminate` is a legal verdict — an unsupported pillar must **not** be
  silently upgraded to `supported`. Declaration: `requires: no_verdict_inflation`
- the China-ratio estimate is an interval or null, never a point claim.
  Declaration: `requires: interval_estimate`
- T-001 reconciliation: any number contradicting a T-001 artifact is a finding,
  not noise — stated explicitly. Declaration: `requires: t001_reconciliation`

---

## 3. Snapshot schema

Applies to `snapshots/002-value-chain-profit-pool-map/YYYY-MM-DD_thesis.md`.

```yaml
---
thesis_id: "002-value-chain-profit-pool-map"
snapshot_date: 2026-09-10
claim: "The dominant profit pool sits in actuation, transmission, and force sensing; ..."
conviction: null                  # derived from evidence, never hand-set
falsifiers_status:
  PIL-1a: untested
  PIL-1b: untested
  PIL-2: untested
  PIL-3: untested
known_open: []
constitution_pin: "1.3.0"
assumption_pin: 1
---
```

**requires:**

- `conviction` derived by the reduction step, never authored. Declaration:
  `requires: derived_conviction` (Q5/Q8)
- the snapshot is written only by `scripts/reduce_journals.py`, one atomic write
  per cycle. Declaration: `requires: single_writer` (Q5/Q15)

---

## 4. What this thesis does NOT contract

- **No price evidence.** `market_data_stage: none`. No `close`-basis quotes, no
  `evidence/quotes/` snapshots, no bars schema (Q42 not triggered).
- **No valuation outputs.** No DCF, comps, or SOTP artifacts. T-002 produces a
  profit-pool map; valuation belongs to the Phase 3 company theses (T-009…T-014).
- **No position sizing.** No `position_pct` field is emitted. Sizing appears only
  in T-015, after the second Constitution Check.

> If any of the above is later required, this thesis must be amended — not extended
> in place — because the change alters its `market_data_stage` contract.
