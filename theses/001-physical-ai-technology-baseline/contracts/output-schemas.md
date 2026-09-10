# Contracts — Physical AI Technology Baseline

> Output frontmatter schemas and `requires:` declarations for artifacts produced by
> this thesis. Downstream consumers (`converge`, `implement`) read these declarations;
> an artifact whose frontmatter fails its schema is rejected rather than partially
> consumed.

---

## 1. Per-ticker artifact schema

Applies to every `{ticker}/YYYY-MM-DD_HHMM_{skill}_{affix}.md` file produced under
this thesis.

```yaml
---
artifact_id: "001-NVDA-secular-trends-20260910-1530"
thesis_id: "001-physical-ai-technology-baseline"
ticker: NVDA                    # must be P2.1-verified retrievable
skill: secular-trends
mode: default
affix: ""

# Pins — an artifact is only valid against the pins it was produced under
constitution_pin: "1.2.0"
assumption_pin: 1
corpus_version: "agentii-2026-09-10"
skill_pin: "75ce82d"
as_of: 2026-09-10

# Evidence discipline (P4)
entity_claims:                  # every material number appears here
  - entity: NVDA
    metric: robotics_and_simulation_revenue_share_of_total_pct
    value: null                 # populated at implement
    unit: pct
    period: 2026Q2
    source: "10-K:pageNN"
    retrieved_at: 2026-09-10T00:00:00-04:00
    observed_at: null

citations:                      # inline citation targets, agentii.ai/v/... form
  - "agentii.ai/v/NVDA/secNNN/NN"

pillars_addressed: [PIL-1, PIL-4]
claim_state: pinned             # pinned|superseded|retired|retired_by_ic|pending_review|stale_price|pending_gate
---
```

**requires:**

- `ticker` confirmed retrievable by direct retrieval across **two** revenue concepts
  (P2.1). Declaration: `requires: p2_1_verified_ticker`
- every `entity_claims[].metric` present in `entities.md` entity/metric map.
  Declaration: `requires: metric_in_entity_map`
- every material quantitative statement followed inline by its citation.
  Declaration: `requires: inline_citation` (P4)
- `constitution_pin` equal to the workspace's current ratified version.
  Declaration: `requires: constitution_pin_current`

---

## 2. Cross-stock synthesis schema

Applies to `_cross/{slug}_synthesis.md`.

```yaml
---
artifact_id: "001-cross-technology-baseline-20260910"
thesis_id: "001-physical-ai-technology-baseline"
type: cross_synthesis
tickers_covered: [NVDA, ISRG, TSLA, AMZN]
pillars_synthesized: [PIL-1, PIL-2, PIL-3, PIL-4]
pillar_verdicts:
  PIL-1: supported | refuted | indeterminate
  PIL-2: supported | refuted | indeterminate
  PIL-3: supported | refuted | indeterminate
  PIL-4: supported | refuted | indeterminate
constitution_pin: "1.2.0"
as_of: 2026-09-10
capability_timeline:
  gpt_3_5_moment_estimate: "2027-Q4 to 2028-Q2"   # the thesis's dated output
  confidence: low | medium | high
---
```

**requires:**

- every `pillar_verdicts` entry backed by a stated falsifier test result.
  Declaration: `requires: falsifier_evidence`
- `indeterminate` is a legal verdict — an unsupported pillar must **not** be silently
  upgraded to `supported`. Declaration: `requires: no_verdict_inflation`
- the capability timeline must carry an explicit confidence band, never a point
  estimate. Declaration: `requires: interval_estimate` (see plan risk note 2)

---

## 3. Snapshot schema

Applies to `snapshots/{slug}/YYYY-MM-DD_thesis.md`.

```yaml
---
thesis_id: "001-physical-ai-technology-baseline"
snapshot_date: 2026-09-10
claim: "Embodied AI is data-bound, not compute-bound; ..."
conviction: null                # derived from evidence, never hand-set
falsifiers_status:
  PIL-1: untested
  PIL-2: untested
  PIL-3: untested
  PIL-4: untested
known_open: []
constitution_pin: "1.2.0"
assumption_pin: 1
---
```

**requires:**

- `conviction` derived by the reduction step, never authored. Declaration:
  `requires: derived_conviction` (Q5/Q8)
- the snapshot is written only by `scripts/reduce_journals.py`, one atomic write per
  cycle. Declaration: `requires: single_writer` (Q5/Q15)

---

## 4. What this thesis does NOT contract

- **No price evidence.** `market_data_stage: none`. No `close`-basis quotes, no
  `evidence/quotes/` snapshots, no bars schema (Q42 not triggered).
- **No valuation outputs.** No DCF, comps, or SOTP artifacts. T-001 produces a
  technology baseline; valuation belongs to the Phase 3 company theses.
- **No position sizing.** No `position_pct` field is emitted. Sizing appears only in
  T-015 (`portfolio-construction-hedge`), after the second Constitution Check.

> If any of the above is later required, this thesis must be amended — not extended
> in place — because the change alters its `market_data_stage` contract.
