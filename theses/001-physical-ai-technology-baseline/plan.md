# Research Plan: Physical AI Technology Baseline

> Ordering rule (Q35/Q36): **fundamentals first, trade ideas last.** This plan starts
> with the physics and business understanding and ends with dateable catalysts and
> sizing. Constitution Check runs twice — at plan start (scalar + scope) and again
> after sizing (aggregate), because `position_pct` does not exist until then.

**Thesis**: `theses/001-physical-ai-technology-baseline/`
**Constitution pin**: `1.2.0`
**Planned**: 2026-09-10
**Phase**: 0 — Foundation (gates all other theses)

---

## Constitution Check — first evaluation (scalar + scope)

Run at plan start, before any dispatch.

| Constraint | Status | Evidence |
|---|---|---|
| Research scope — market cap | **PASS** | NVDA, ISRG, TSLA, AMZN all exceed the $100M floor and sit below the $2T ceiling; all four are large-cap |
| Research scope — regions | **PASS** | All four are US-listed (NVDA/ISRG Nasdaq, TSLA Nasdaq, AMZN Nasdaq); no ADR dependency |
| Research scope — excluded sectors | **PASS** | Constitution excludes none categorically; theses span IT, Health Care, Cons Disc by design |
| P2 — coverage-bounded universe | **PASS** | All four return filings, documents and XBRL facts (NVDA: 169 filings/169 xbrl; ISRG: 173/63 revenue facts; TSLA: 259 filings/63,523 xbrl facts; AMZN: 86 docs) |
| P2.1 — coverage verification | **PASS** | Each ticker confirmed by direct retrieval across two revenue concepts, not by index lookup |
| POS_SINGLE (≤8%) | **N/A at plan time** | Position sizing does not exist until Phase 4; evaluated in the second Constitution Check |
| STOP_THESIS (≤30%) | **N/A at plan time** | As above |
| P7.1 — no leverage | **PASS** | Research-only thesis; no financing instrument referenced |
| P7.2 — liquidity | **N/A at plan time** | Requires ADV data; resolved in the second check if this thesis proceeds to a trade idea |

**First-check verdict: PASS.** No deviation register entry is required at this stage.

---

## Phases

| Phase | Content | Skills (ticker × skill × mode) | Depends on |
|:---:|------|------|---|
| 1 — Physics and Literature Baseline | Establish the primitive quantities: torque density, energy density, actuator power budget, thermal envelope | `NVDA × secular-trends × default`, `ISRG × operational-kpi × default` | Constitution loaded |
| 2 — Data Economics | Quantify the cost per hour of teleoperation vs egocentric video vs synthetic simulation; size the embodied-data gap | `TSLA × business-model × default`, `AMZN × operational-kpi × default`, `NVDA × business-model × default` | Phase 1 |
| 3 — Reliability Evidence | Extract disclosed MTBF, task success rates, and deployment scale from filings and transcripts | `ISRG × recent-quarter × default`, `ISRG × operational-kpi × default`, `AMZN × recent-quarter × default` | Phase 2 |
| 4 — Capability Timing Synthesis | Fuse phases 1–3 into a dated capability timeline with explicit falsifiers; produce the cross-stock synthesis and snapshot | `NVDA × secular-trends × deep`, `TSLA × risk × default`, cross-stock synthesis | Phases 1–3 |
| 5 — Trade Ideas | Dateable catalysts + sizing per `constitution.yaml` | Position sizing + catalyst dating | Phase 4 |

**Budget**: 34 tasks (see `tasks.md`), within the `max_tasks: 80` thesis budget and
the `max_tasks_per_day: 60` workspace budget.

---

## Side artifacts (Q36)

| artifact | status | content |
|---|---|---|
| `brief.md` | written | Stage-0 context brief — retrieval keys, strategy candidates with `method_selection:` verdicts, `<ref:*>` framed blocks, `corpus_version` pin |
| `entities.md` | written | `entity_claims` schema + entity/metric map. **No bars schema required** — this thesis is `market_data_stage: none` |
| `reproduce.md` | written | Skills + five pins + `as_of` |
| `contracts/` | written | Output frontmatter schemas + `requires:` declarations |

### Q42 check — bars schema

This thesis is **not** `market_data_stage: early` (no price-history retrieval in any
phase; all pillars are falsifiable from filings, transcripts and technical
disclosures). The `get_price_history` bars schema is therefore **not required** and
`implement` will not refuse for its absence.

> If Phase 5 introduces a price-based catalyst trigger, this thesis must be re-planned
> as `market_data_stage: early` and `entities.md` extended with the bars schema before
> implement.

---

## Constitution Check — second evaluation (aggregate)

Evaluated only if Phase 5 produces a trade idea. At plan time, **Phase 5 is the only
phase that could create positions**, and this thesis's phases 1–4 are research-only.

| Constraint | Status | Evidence |
|---|---|---|
| POS_SINGLE (≤8%) | **DEFERRED** | No position proposed yet; requires Phase 5 output |
| POS_BINARY (≤4%) | **DEFERRED** | No binary-catalyst position identified |
| CONC_SECTOR (≤40%) | **DEFERRED** | Requires the full portfolio from T-015 |
| EXPO_MACRO (≤30%) | **DEFERRED** | Requires the full portfolio from T-015 |
| LEVERAGE (≤100%) | **PASS by construction** | No leverage instrument in scope |
| LIQUIDITY_ADV (≤15%) | **DEFERRED** | Requires 20-day ADV data |

**Second-check verdict: deferred to Phase 5.** This is not a violation — the
constraints are inapplicable to a research-only foundation thesis. The aggregate
check must be re-run when Phase 5 produces sizing.

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
2. **The §4 capability-timing pillar is the softest.** `general_purpose_humanoid_commercial_units_deployed > 10000`
   is falsifiable but the source in 2026 is company disclosure, which is promotional
   in character. Treat any disclosed unit count as a claim to be triangulated, not a
   measurement.
3. **AMZN is the weakest link.** It is included as a fleet-scale deployer, but
   warehouse automation is not humanoids. Its evidence bears on deployment economics
   generally, not on embodied AI specifically. Flag this in the synthesis.
4. **Do not let Phase 2's data-economics numbers drift into precision they do not
   have.** Cost-per-hour figures for teleoperation are industry estimates with wide
   dispersion; the pillar falsifier uses an order-of-magnitude threshold for this
   reason.

---

*Gate 2 (after plan, informational) shows phases + this Deviation Register.*
