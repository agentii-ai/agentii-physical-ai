# Research Plan: Physical AI Technology Baseline

> Ordering rule (Q35/Q36): **fundamentals first, trade ideas last.** This plan starts
> with the physics and business understanding and ends with dateable catalysts and
> sizing. Constitution Check runs twice — at plan start (scalar + scope) and again
> after sizing (aggregate), because `position_pct` does not exist until then.

**Thesis**: `theses/001-physical-ai-technology-baseline/`
**Constitution pin**: `1.2.0`
**Planned**: 2026-09-10 (rev. 3 — see Revision Note)
**Phase**: 0 — Foundation (gates all other theses)
**Tasks**: 25 generated (23 decomposition + 2 synthesis), 13 parallelisable — see `tasks.md`

---

## Revision Note (rev. 3, 2026-09-10)

Rev. 1 was evaluated against its own spec and four defects were found:

1. **PIL-2 was undeliverable.** Its falsifier needs `actuator_share_of_humanoid_bom_pct`,
   but the universe contained no motion-control name and its subscribed work
   (`TSLA × unit-economics`, `AMZN × supply-chain`) could not produce an actuator BOM
   figure. **Fixed** by adding PH (Motion Systems segment, 166 filings, 36 revenue
   facts) and re-pointing PIL-2 at `PH × unit-economics` + `PH × supply-chain`.
2. **Three inconsistent deployment sets.** The spec matrix (11 pairs), pillar
   subscriptions (8), and the rev. 1 phase table (8) disagreed. The `tasks` generator
   reads §3, so the matrix is authoritative; subscriptions and this plan now match it
   exactly (13 pairs, verified as sets).
3. **Depth over-expansion.** `secular-trends × deep` pulled in 8 modes per ticker,
   including `deep-dive-ev-trend-assessment` and
   `deep-dive-analysis-for-quantum-computing-renewable-energy` — 6 tasks with no
   physical-AI bearing. Reduced to `standard`.
4. **Task count was wrong.** Rev. 1 claimed 34; the generator produces 23 at the
   corrected matrix.

Rev. 3 additions (tasks pass, 2026-09-10): `tasks.md` was audited against the
`agentii.tasks` contract and four further defects were found and fixed — two in the
upstream generator.

5. **`src:` was vacuous.** The generator hardcoded `{"pillar": "P1"}`, so every row
   read `(src: P1)` regardless of which pillar the work served, defeating Q26
   traceability. The generator now derives each task's pillar from the spec's
   `Subscribed:` lists (the same Q9 source used for reconciliation). Verified:
   `risk` → `PIL-3`, `unit-economics`/`supply-chain` → `PIL-2`+.
6. **`purpose` was a placeholder.** The matrix's Purpose column was parsed away, so
   all 23 rows read "per spec deployment matrix". Now carried through.
7. **No synthesis task existed.** The plan names cross-stock synthesis and a
   snapshot as Phase 4 deliverables, but no task owned them. Added T024/T025,
   marked never-`[P]` per the template's cross-ticker rule.
8. **The file was not append-only.** Rev. 2's header said "regenerate rather than
   hand-edit", which contradicts the template's Q26 contract ("never rewritten,
   renumbered, reordered or deleted from"). The header now states the append-only
   rule and carries the `agentii.converge` marker.

---

## Constitution Check — first evaluation (scalar + scope)

Run at plan start, before any dispatch.

| Constraint | Status | Evidence |
|---|---|---|
| Research scope — market cap | **PASS** | NVDA, ISRG, TSLA, AMZN, PH all exceed the $100M floor and sit below the $2T ceiling |
| Research scope — regions | **PASS** | All five US-listed: NVDA/ISRG/TSLA/AMZN Nasdaq, PH NYSE (`sec166`, CIK 0000076334) |
| Research scope — excluded sectors | **PASS** | Constitution excludes none categorically; theses span IT, Health Care, Cons Disc, Industrials by design |
| P2 — coverage-bounded universe | **PASS** | All five return filings, documents and XBRL facts. PH: 166 filings, 80 docs, 36 revenue facts (FY26 revenue $21.499B per `ph-20260630.htm`) |
| P2.1 — coverage verification | **PASS** | Each ticker confirmed by direct retrieval across two revenue concepts, not by index lookup |
| POS_SINGLE (≤8%) | **N/A at plan time** | Position sizing does not exist until Phase 5; evaluated in the second Constitution Check |
| STOP_THESIS (≤30%) | **N/A at plan time** | As above |
| P7.1 — no leverage | **PASS** | Research-only thesis; no financing instrument referenced |
| P7.2 — liquidity | **N/A at plan time** | Requires ADV data; resolved in the second check if this thesis proceeds to a trade idea |

**First-check verdict: PASS.** No deviation register entry required at this stage.

---

## Phases

Every `ticker × skill` pair below appears in `spec.md` §3 and in its pillar's
`Subscribed` list. The three sets are verified equal.

| Phase | Content | Skills (ticker × skill × mode) | Depends on |
|:---:|------|------|---|
| 1 — Physics and Literature Baseline | Primitive quantities: torque density, energy density, actuator power budget, thermal envelope | `NVDA × secular-trends × standard`, `ISRG × secular-trends × standard`, `TSLA × secular-trends × standard` | Constitution loaded |
| 2 — Component Economics and Dependency | Actuator/motion cost stack and the physical supply chain — the PIL-2 evidence base | `PH × unit-economics × standard`, `PH × supply-chain × standard`, `TSLA × unit-economics × standard`, `ISRG × unit-economics × standard`, `NVDA × supply-chain × standard`, `AMZN × supply-chain × standard` | Phase 1 |
| 3 — Reliability Evidence | Disclosed MTBF, task success rates, deployment scale from filings and transcripts | `ISRG × operational-kpi × standard`, `AMZN × operational-kpi × standard` | Phase 2 |
| 4 — Risk and Timing Synthesis | Fuse phases 1–3 into a dated capability timeline with explicit falsifiers; produce cross-stock synthesis and snapshot | `NVDA × risk × standard`, `TSLA × risk × standard`, cross-stock synthesis | Phases 1–3 |
| 5 — Trade Ideas | Dateable catalysts + sizing per `constitution.yaml` | Position sizing + catalyst dating | Phase 4 |

**Budget**: 25 tasks (see `tasks.md`) — 23 ticker×skill×mode rows plus 2 synthesis
deliverables. Within the `max_tasks: 80` thesis budget and the `max_tasks_per_day: 60`
workspace budget. 13 tasks carry `[P]` and may run concurrently; 10 serialise behind
their `(ticker, skill)` predecessor; the 2 synthesis tasks are never `[P]` (cross-ticker).
Each task's `src:` names the pillar it serves, derived from the spec's `Subscribed:`
lists via the fixed generator.

---

## Pillar → Evidence Traceability

Every pillar's falsifier must be reachable from its subscribed work. This is the
check that caught the rev. 1 defect.

| Pillar | Priority | Falsifier metric | Subscribed work | Reachable? |
|---|:---:|---|---|:---:|
| PIL-1 — Data, not compute, is binding | P1 | `embodied_dataset_hours_vs_llm_pretrain_token_gap_order_of_magnitude > 3` | `NVDA × secular-trends`, `NVDA × supply-chain`, `AMZN × supply-chain` | yes |
| PIL-2 — Actuators dominate BOM | P2 | `actuator_share_of_humanoid_bom_pct < 35` | `PH × unit-economics`, `PH × supply-chain` | yes — **added rev. 2** |
| PIL-3 — Manipulation reliability gates | P3 | `humanoid_mtbf_hours_in_commercial_deployment > 2000` | `ISRG × operational-kpi`, `ISRG × secular-trends`, `NVDA × risk`, `TSLA × risk` | yes |
| PIL-4 — GPT-3.5 moment 2027–2028 | P4 | `general_purpose_humanoid_commercial_units_deployed > 10000` | `TSLA × secular-trends`, `ISRG × secular-trends`, `TSLA × unit-economics`, `ISRG × unit-economics`, `AMZN × operational-kpi` | yes |

**P1 alone yields a defensible partial conclusion** (Q30): if budget halts after
Phase 1, PIL-1 is testable from `secular-trends` and `supply-chain` output alone.

---

## Side artifacts (Q36)

| artifact | status | content |
|---|---|---|
| `brief.md` | written | Stage-0 context brief — retrieval keys, strategy candidates with `method_selection:` verdicts, `<ref:*>` framed blocks, `corpus_version` pin |
| `entities.md` | written | `entity_claims` schema + entity/metric map. **No bars schema required** — this thesis is `market_data_stage: none` |
| `reproduce.md` | written | Skills + five pins + `as_of`; now also records the missing `plan` subcommand |
| `contracts/` | written | Output frontmatter schemas + `requires:` declarations |
| `tasks.md` | written | 25 generated tasks, grouped by phase; append-only with a converge marker |

### Q42 check — bars schema

This thesis is **not** `market_data_stage: early`. No phase retrieves
`get_price_history`; every pillar is falsifiable from filings, transcripts and
technical disclosure. The `get_price_history` bars schema is **not required** and
`implement` will not refuse for its absence.

> If Phase 5 introduces a price-based catalyst trigger, this thesis must be re-planned
> as `market_data_stage: early` and `entities.md` extended with the bars schema before
> implement.

---

## Constitution Check — second evaluation (aggregate)

Evaluated only if Phase 5 produces a trade idea. At plan time, **Phase 5 is the only
phase that could create positions**; phases 1–4 are research-only.

| Constraint | Status | Evidence |
|---|---|---|
| POS_SINGLE (≤8%) | **DEFERRED** | No position proposed yet; requires Phase 5 output |
| POS_BINARY (≤4%) | **DEFERRED** | No binary-catalyst position identified |
| CONC_SECTOR (≤40%) | **DEFERRED** | Requires the full portfolio from T-015 |
| EXPO_MACRO (≤30%) | **DEFERRED** | Requires the full portfolio from T-015 |
| LEVERAGE (≤100%) | **PASS by construction** | No leverage instrument in scope |
| LIQUIDITY_ADV (≤15%) | **DEFERRED** | Requires 20-day ADV data |

**Second-check verdict: deferred to Phase 5.** Not a violation — the constraints are
inapplicable to a research-only foundation thesis. The aggregate check must be re-run
when Phase 5 produces sizing.

### Pre-flagged for T-015

With PH added, T-001's research universe is 20% Industrials (PH) and 40% Consumer
Discretionary (TSLA, AMZN) if read as a portfolio. **40% sits exactly at the
`CONC_SECTOR` ceiling.** T-001 is research-only and the constraint does not bind here,
but T-015 must not carry this weighting forward without re-checking.

---

## Deviation Register

| Constraint | Why Accepted | Safer Alternative Rejected Because | Approver | Expiry |
|---|---|---|---|---|
| *(none)* | — | — | — | — |

> No-defended-violation = plan not complete. **There are no accepted violations in
> this plan**, so the register is legitimately empty and `agentii.plan` may report
> success.

---

## Risk notes for the implementer

1. **This thesis gates all 14 others.** Its assumptions propagate downstream via the
   `constitution_pin` and `assumption_pin` mechanism. An error here compounds.
2. **PIL-4 is the softest pillar.** `general_purpose_humanoid_commercial_units_deployed > 10000`
   is falsifiable, but its source in 2026 is company disclosure, which is promotional.
   Treat disclosed unit counts as claims to triangulate, not measurements.
3. **AMZN is the weakest entity.** It is included as a fleet-scale deployer, but
   warehouse automation is not humanoids. Its evidence bears on deployment economics
   generally, not on embodied AI specifically. Flag this in the synthesis.
4. **PIL-2 evidence is not audit-grade.** The actuator BOM share comes from teardowns,
   not filed disclosures. PH supplies the segment cost structure, but the *humanoid*
   BOM split remains an industry estimate. The falsifier uses a wide threshold (<35%)
   for this reason.
5. **Do not let Phase 2's data-economics numbers drift into precision they do not
   have.** Cost-per-hour figures for teleoperation are industry estimates with wide
   dispersion; the PIL-1 falsifier uses an order-of-magnitude threshold for this reason.
6. **`deep` depth is unsafe for 62 of 71 skills.** Their `skill-registry.yaml`
   `essentials_modes` is empty, so `depth_to_modes` expands `deep` to mode slugs that
   are SKILL.md *section headings* (`triggers`, `defaults`, `methodology`,
   `retrieval-scope`, `retrieval-strategy`) rather than analysis modes. This plan uses
   `standard` throughout. See the upstream note in `reproduce.md`.

---

*Gate 2 (after plan, informational) shows phases + this Deviation Register.*
