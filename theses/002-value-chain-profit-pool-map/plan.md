# Research Plan: Value Chain Profit Pool Map

> Ordering rule (Q35/Q36): **fundamentals first, trade ideas last.** This plan starts
> with the layer structure and ends with falsifier tests and synthesis. Constitution
> Check runs twice — at plan start (scalar + scope) and again after sizing (aggregate)
> — but T-002 is a research-only structural map with no Phase 5 trade ideas, so the
> second check is deferred exactly as T-001's was.

**Thesis**: `theses/002-value-chain-profit-pool-map/`
**Constitution pin**: `1.3.0`
**Planned**: 2026-09-10 (rev. 5 — fourth optimization round)
**Phase**: 1 — Industry Structure (parallel with T-003…T-007)
**Tasks**: 21 (19 decomposition + 2 synthesis) — exact counts from the
`agentii.tasks` generator at task-materialisation time

---

## Revision Note (rev. 5, 2026-09-10 — fourth optimization round)

Rev. 4 was re-audited with a full-file read plus fresh angles (checklist state,
spec cross-references). Three findings, all annotation-grade:

1. **Another stale reference survived** — the side-artifacts table said
   `reproduce.md … plan_rev 2` while the actual plan_rev is 4. **Fixed** (the
   table no longer pins a number; reproduce.md is the single source of truth).
2. **Spec §5 parenthetical was stale** — "Feeds directly into T-008 (chokepoint
   synthesis)" vs the actual thesis `008-chokepoint-pricing-power`. **Fixed** in
   the spec.
3. **The Q29 soft gate was unaddressed.** The checklist carries 5 unchecked
   upstream-template items, of which CHK003 (empty-result disposition) is
   structurally N/A for a fixed 7-name map. **Fixed** with a new
   "Pre-flagged for implement (Q29)" section under Side artifacts — the owner
   can waive CHK003 with a written rationale instead of re-deriving it at
   implement time. The P6 Chinese-checklist flag is recorded there too.

Rev. 2–4 fixes are carried forward unchanged.

---

## Revision Note (rev. 4, 2026-09-10 — third optimization round)

Rev. 3 was re-audited for internal consistency and measurement risk. Two
findings, both annotation-grade — the plan has converged:

1. **A stale falsifier reference survived the rev-3 edit.** The T-001-inputs
   section still named the superseded level-ratio metric ("motion-vs-model GM
   ratio < 1.0") while the revision note and traceability table carried the
   re-scoped trend metric. **Fixed**: the section now names
   `motion_model_gm_gap_change_pp` (internal contradiction resolved).
2. **Two falsifier-measurement hazards surfaced by continued plan-time
   pre-testing** (now risk note 7): (a) PIL-1a is live-sensitive — the industry
   teardown range (actuators 40–70% + sensing 11–18% = 51–88%) straddles the
   55% threshold, so the synthesis must report a range, never a point estimate;
   (b) the PIL-1b gap-change test spans five fiscal calendars (PH June-30, NVDA
   late-January, ISRG Dec-31, AMBA Jan-31 with a registry month-3 quirk, CGNX
   Dec-31 with 4-4-5 Sunday quarter-ends) — the pairing must be aligned
   like-for-like by period_end date or the test measures calendar drift.

Rev. 2 and rev. 3 fixes are carried forward unchanged.

---

## Revision Note (rev. 3, 2026-09-10 — second optimization round)

Rev. 2 was re-audited, this time testing every falsifier against the T-001
evidence baseline at plan time (a falsifier must survive contact with known
data — the lesson behind T-001's rev.1 defect). Two findings:

1. **PIL-1b's falsifier was pre-falsified by T-001's own audited anchors.**
   The level-ratio metric (`motion_layer_gross_margin_vs_model_layer_gm_ratio
   < 1.0`) was already triggered: PH GM 37.7% (ratio 0.53), PH DI op margin
   23.8% (0.33), ISRG product GM 66.3% (0.93), TSLA automotive GM 17.8% (0.25)
   — every same-line comparison against NVDA's 71.1% GM sits below 1.0. A level
   comparison confounds business-model economics (fabless GPU vendor vs
   diversified industrial vs integrated medical-robot maker) with barriers to
   substitution. **Fixed with the owner's ruling (clarify round 4)**: PIL-1b
   re-scoped to a trend metric — `motion_model_gm_gap_change_pp < -10` (the
   motion-minus-model GM gap falling >10pp over the 3-FY corpus falsifies it).
   Durability is how the gap moves, not its level. Spec prose + YAML + the
   Clarifications record all updated.
2. **YAML had drifted from the rev-2 prose.** P1's YAML subscriptions lacked
   `competitive-positioning × standard` (added to prose in rev. 2). **Fixed**:
   YAML skill sets now mirror the prose for all three pillars.

Rev. 2's fixes (four orphan pairs subscribed → 15 = 15; competitive-positioning
moved to Phase 3 per spec §7; brief.md installed-base correction) are carried
forward unchanged.

---

## T-001 inputs (the upstream dependency, now complete)

This plan is authored against T-001's completed analysis (`cdc5ce3` + converge +
challenge). T-001 established the evidence baseline this thesis builds on:

1. **The BOM-share claims are unfiled.** T-001's PIL-2 (actuator 40–70% of BOM)
   came back `indeterminate` — no humanoid teardown or 10-K BOM split exists in the
   agentii corpus. T-002's PIL-1 (>55% actuation+sensing) and PIL-2 (China ~3×)
   inherit the same structural gap and are governed by the clarify round-3
   evaluation rules (filing proxies carry the tests; teardown figures enter only
   as `[VIEW]`).
2. **The profit-pool reference numbers exist.** From T-001 artifacts: ISRG product
   GM 66.3% / total GM 66.0% (sec166), 84% recurring revenue, I&A ~$1.83K per
   procedure, 12,101 installed systems FY2025; NVDA FY2026 GM 71.1% (sec169), Edge
   Computing $6.4B; PH Motion Systems $3,580M FY2026 at DI segment margin 23.8%
   (sec166); TSLA automotive GM 17.8% FY2025 (sec253). These are the layer-margin
   anchors the durability falsifier (PIL-1 #2: `motion_model_gm_gap_change_pp`
   trend test — re-scoped in rev. 3)
   tests against.
3. **T-001 challenge findings apply.** Finding #1 (falsifier sources outside the
   corpus) is mitigated at the spec level by the round-3 rules; finding #2 (the
   China blind spot) is the subject of the Deviation Register entry below.
4. **Depth hazard resolved.** T-001 reproduce.md deviation #3: `deep` is unsafe for
   skills with empty `essentials_modes`. T-002 runs `standard` on every matrix row
   (§4 note in the spec).

---

## Constitution Check — first evaluation (scalar + scope)

Run at plan start, before any dispatch.

| Constraint | Status | Evidence |
|---|---|---|
| Research scope — market cap | **PASS** | All seven within $100M–$2T: AMBA $2.71B, CGNX $10.47B (`get_company_profile`, freshness 2026-08-26); NVDA/ISRG/TSLA/PH verified in T-001's plan; SPCX $1.62T (largest, in-range) |
| Research scope — regions | **PASS** | All seven US-listed: AMBA Nasdaq (CIK 0001280263), CGNX Nasdaq (CIK 0000851205), NVDA/ISRG/TSLA Nasdaq, PH NYSE, SPCX Nasdaq (T-001 evidence) |
| Research scope — excluded sectors | **PASS** | Constitution excludes none categorically; this map spans IT, Industrials, Health Care, Cons Disc by design |
| P2 — coverage-bounded universe | **PASS** | All seven return filings and XBRL facts. AMBA: 12 10-Ks (sec95–sec106, latest FY2025 filed 2026-03-23), 33 revenue facts (FY2026 $390.7M, authority 3). CGNX: 12 10-Ks (sec82–sec93, latest FY2025 filed 2026-02-12), 35 revenue facts (FY2025 $994.4M, authority 3). Five names carried from T-001's verified run |
| P2.1 — coverage verification | **PASS** | Each ticker confirmed by direct retrieval (filings + revenue facts), not by index lookup. AMBA/CGNX tag only `RevenueFromContractWithCustomerExcludingAssessedTax` (the single-concept pattern T-001 documented for ISRG/TSLA/PH/SPCX) — P2.1 satisfied via same-concept multi-period facts, reconciled at implement against income-statement tables |
| POS_SINGLE (≤8%) | **N/A at plan time** | No sizing phase exists in this thesis; T-002 produces a structural map |
| STOP_THESIS (≤30%) | **N/A at plan time** | As above |
| P7.1 — no leverage | **PASS** | Research-only thesis; no financing instrument referenced |
| P7.2 — liquidity | **N/A at plan time** | Requires ADV data; no position is ever proposed here |

**First-check verdict: PASS** with one defended deviation (see register).

---

## Phases

Every `ticker × skill` pair below appears in `spec.md` §3 and in its pillar's
`Subscribed` list. The three sets are verified equal (15 = 15, rev. 2).

| Phase | Content | Skills (ticker × skill × mode) | Depends on |
|:---:|------|------|---|
| 1 — Layer definition | Enumerate the value-chain layers and assign each ticker; classify the business models that sit on each layer | `PH × business-model × standard` (3 modes), `ISRG × business-model × standard` (3 modes) | Constitution loaded; T-001 artifacts available as reference |
| 2 — Profit quantification | Segment economics per layer: each layer's supply chain, the cost stacks, and the revenue mixes | `NVDA × supply-chain × default`, `PH × supply-chain × default`, `ISRG × supply-chain × default`, `AMBA × supply-chain × default`, `CGNX × supply-chain × default`, `SPCX × supply-chain × default`, `ISRG × unit-economics × default`, `TSLA × unit-economics × default`, `PH × revenue-decomp × default`, `ISRG × revenue-decomp × default` | Phase 1 |
| 3 — Durability assessment and synthesis | Barriers, substitution risk, pricing power per layer; then test all four falsifiers against Phase 1–2 evidence and publish the layer profit-pool map with verdicts | `PH × competitive-positioning × default`, `NVDA × competitive-positioning × default`, `AMBA × competitive-positioning × default`, then cross-stock synthesis + snapshot (never `[P]`) | Phases 1–2 |

**Budget**: 19 decomposition + 2 synthesis = 21 tasks, within `max_tasks: 80` and
the `max_tasks_per_day: 60` workspace budget. Decomposition forms 15 (ticker,
skill) chains: business-model chains carry 3 sequential modes (modes 2–3 not
`[P]`); all other pairs are single default-mode tasks (`[P]`). The 2 synthesis
tasks are never `[P]` (cross-ticker).

---

## Pillar → Evidence Traceability

Every pillar's falsifier must be reachable from its subscribed work — the check
that caught the T-001 rev.1 defect and this plan's rev.1 orphans.

| Pillar | Priority | Falsifier metric | Subscribed work | Reachable? |
|---|:---:|---|---|:---:|
| PIL-1 — Profit concentrates in motion and sensing | P1 | (a) `actuation_plus_sensing_share_of_bom_pct < 55`; (b) `motion_model_gm_gap_change_pp < -10` (trend — re-scoped in rev. 3) | `PH × supply-chain`, `AMBA × supply-chain`, `CGNX × supply-chain`, `ISRG × supply-chain`, `NVDA × supply-chain`, `SPCX × supply-chain`, `ISRG × unit-economics`, `TSLA × unit-economics`, `PH × competitive-positioning` | yes — (a) via SEC-filing proxies per the round-3 rule (the motion/sensing chains vs the compute-chain counterpoint and the demand-side pull); (b) from multi-year segment GM disclosures (PH/NVDA/ISRG, 3 FYs each) — the gap-change test needs no Phase 3 competitive-structure input |
| PIL-2 — China holds a ~3× structural cost advantage | P2 | `nonchina_to_china_humanoid_bom_cost_ratio < 2.0` | `PH × supply-chain`, `AMBA × competitive-positioning`, `NVDA × competitive-positioning` | **partial — defended deviation**: the ratio itself needs teardown data outside the corpus; the test runs on filing-derived proxies (disclosed supplier/cost structure, import-substitution competitive dynamics) with teardown figures as `[VIEW]` only |
| PIL-3 — The model layer captures minimal value near-term | P3 | `model_layer_revenue_per_deployed_unit_usd > 5000` (includes per-unit software/subscription revenue — clarify round 3) | `PH × revenue-decomp`, `ISRG × revenue-decomp`, `PH × business-model`, `ISRG × business-model` | yes — ISRG's per-system subscription/service revenue (T-001: 84% recurring, I&A ~$1.83K/procedure, 12,101 installed) is the direct test input; PH is the null case (hardware vendor with no model-layer rent) |

**P1 alone yields a defensible partial conclusion** (Q30): if budget halts after
Phase 2, both PIL-1 falsifiers are testable from supply-chain + unit-economics
output plus T-001's carried margin anchors — the durability test (b) needs no
Phase 3 competitive-structure input to be evaluated.

---

## Side artifacts (Q36)

| artifact | status | content |
|---|---|---|
| `brief.md` | written | Stage-0 context brief — Q18 retrieval keys, strategy candidates with `method_selection:` verdicts, `<ref:*>` framed blocks, `corpus_version` pin (installed-base figure corrected in rev. 2) |
| `entities.md` | written | `entity_claims` schema + entity/metric map for the 7 names. **No bars schema required** — this thesis is `market_data_stage: none` |
| `reproduce.md` | written | Skills + five pins + `as_of`; records the `plan` subcommand gap (known deviation #1 carried from T-001); `plan_rev` tracks this plan's revision |
| `contracts/` | written | Output frontmatter schemas + `requires:` declarations |
| `tasks.md` | not yet | Materialised by `agentii.tasks` from §3 (regeneration at implement) |

### Q42 check — bars schema

This thesis is **not** `market_data_stage: early`. No phase retrieves
`get_price_history`; every pillar is falsifiable from filings and segment
disclosures. The bars schema is **not required** and `implement` will not refuse
for its absence.

### Pre-flagged for implement (Q29 soft gate)

`checklists/thesis-quality.md` carries 5 unchecked items (CHK001–CHK005) from
the upstream specify template. Three are satisfiable by this spec (CHK001
machine-checkable wrong_if — all four falsifiers carry metric+threshold+source;
CHK002 per-ticker rationale — §2 has all 7; CHK004/CHK005 consistency — the
clarify rounds 2–4 resolved both). CHK003 (empty-result disposition) is
**structurally N/A**: T-002's universe is a fixed 7-name map with no screening
step, so no "screening yields nothing" scenario exists — recommend the owner
waive CHK003 with this note at the Q29 ask. The checklist items are
upstream-generated in Chinese (the T-001 P6 flag applies here too); a
translation pass is owed to the checklist file itself, not to this plan.

---

## Constitution Check — second evaluation (aggregate)

**DEFERRED by construction.** T-002 has no Phase 5 trade-idea phase and no
`position_pct` is ever emitted — the map feeds T-008 and the portfolio layer
T-015, which own the aggregate checks. Same disposition as T-001.

---

## Deviation Register

| Constraint | Why Accepted | Safer Alternative Rejected Because | Approver | Expiry |
|---|---|---|---|---|
| P4 Fact Audit Mandate — PIL-2's claim ($46K Chinese vs $131K non-Chinese BOM, ~3×) cannot trace to agentii-retrievable data | The pillar is framed as a hypothesis under test, not a fact: the round-3 evaluation rule makes SEC-filing-derived proxies the evidence path and restricts teardown figures to `[VIEW]` external references. The claim's origin (macro-plan industry teardowns) is disclosed, not smuggled | Re-scoping the falsifier to corpus-only sources would gut the pillar's content (the China supply-chain dependency is the point of the test); deleting the pillar would drop the import-substitution analysis that Phase 3 durability work needs | Workspace owner (ratify at gate 2) | 2026-10-10 (Phase 2 completion — re-justify against the proxy evidence actually retrieved) |

> No-defended-violation = plan not complete. **There is one accepted violation
> in this plan** — it is defended above with an expiry, so `agentii.plan` may
> report success subject to gate-2 ratification.

---

## Risk notes for the implementer

1. **Falsifier evaluation rules (clarify round 3) are binding.** PIL-1/PIL-2 BOM
   and China-ratio evidence comes from SEC-filing-derived proxies; teardown
   figures enter only as `[VIEW]` external references with the macro-plan origin
   stated. PIL-3's metric includes per-unit software/subscription revenue
   (ISRG My Intuitive+, NVDA platform software).
2. **AMBA and CGNX are smaller issuers, and their robotics exposure is indirect**
   (automotive/industrial vision). Do not over-map them onto humanoids — label the
   layer mapping honestly, the T-001 AMZN lesson (warehouse automation ≠ humanoids)
   applies in spirit.
3. **SPCX is a one-quarter issuer** (T-001 risk note 7). Its supply-chain task
   serves the demand-side pool only: compute-led capex ($28.5B H1-2026, 82.7% AI)
   as the pull on upstream layers. Forward compute targets are promotional claims
   to triangulate, not measurements.
4. **T-001 artifacts are the evidence baseline, not a substitute for retrieval.**
   Agents retrieve fresh; the T-001 numbers (ISRG GM 66.3%, NVDA GM 71.1%, PH
   Motion Systems $3,580M) are the falsifier-threshold anchors the synthesis
   reconciles against. Cross-thesis contradictions between a T-002 artifact and a
   T-001 artifact are findings, not noise — the entity index surfaces them.
5. **No price data** (`market_data_stage: none`); no valuation, no sizing. A
   profit-pool map quantifies economics, not multiples.
6. **Depth hazard** already resolved — every row runs `standard` (spec §4 note).
7. **Falsifier-measurement hygiene (rev. 4).** (a) PIL-1a is live-sensitive: the
   industry teardown range for actuation+sensing (51–88%: actuators 40–70% +
   sensing 11–18%) straddles the 55% threshold — the synthesis must report the
   range honestly, never a point estimate. (b) The PIL-1b gap-change test spans
   five fiscal calendars (PH June-30, NVDA late-January, ISRG Dec-31, AMBA
   Jan-31 with a registry month-3 quirk, CGNX Dec-31 with 4-4-5 Sunday
   quarter-ends): align fiscal years like-for-like by period_end date and state
   the pairing explicitly in the artifact, or the 3-FY gap change measures
   calendar drift instead of margin drift.

---

*Gate 2 (after plan, informational): phases 1–3 + this Deviation Register (one
entry, expiring 2026-10-10). Ratify to proceed to `agentii.tasks`.*
