# Reproduce — Physical AI Technology Baseline

> Q8 contract 5 / Q36: the thesis-level reproduction recipe. This is the **one file**
> an external reviewer — compliance, an LP, a new analyst — needs to reconstruct the
> work. Every artifact's own frontmatter carries its pins; this file aggregates them.

**Thesis**: `theses/001-physical-ai-technology-baseline/`
**Generated**: 2026-09-10
**Workspace**: `/Users/frank/B/agentii-physical_ai`
**Git**: branch `main`, baseline commit `c776860`

---

## Skills used

| skill | mode | version_hash (skill_pin) |
|---|---|---|
| `secular-trends` | standard | `e6b41dbb2426` |
| `unit-economics` | standard | `e87ee63269a2` |
| `supply-chain` | standard | `8cb3ac1de486` |
| `operational-kpi` | standard | `0730fd170124` |
| `risk` | standard | `953fc5d396e7` |

**Skill source**: `agentii-investment-intelligence` @ `75ce82d`, installed flat to
`~/.claude/skills/agentii/` (70 skills, 248 reference files).

---

## Pins at generation

| pin | value | note |
|---|---|---|
| `constitution_pin` | **`1.3.0`** | P2 extended ~30→~31 names (SPCX added to the end-market layer); P8 PDCA added |
| `assumption_pin` | **`1`** | `assumptions.yaml` v1, effective 2026-09-10 |
| `corpus_version` | `agentii-2026-09-10` | Workspace retrieval snapshot |
| `as_of` | **2026-09-10** | Date of all retrieval in this plan |
| `skill_pin` | per-skill hashes (table above) | recorded to `skill_pins.jsonl` at implement (Q57) |
| `plan_rev` | `4` | rev.2 fixed the PIL-2 evidence gap + reconciled deployment sets; rev.3 fixed generator src:/purpose, added synthesis tasks, made tasks.md append-only; rev.4 constitution 1.3.0 re-examination: SPCX added to the universe, supply-chain row extended, tasks regenerated (26 tasks) |

**Reproducibility caveat.** A reader reconstructing this work at a later date must
supply `constitution_pin: 1.2.0` and `assumption_pin: 1`. If the constitution has
since been amended with a MINOR or MAJOR bump, this thesis is marked `stale` and the
re-examination dispatch applies (Q33) — the results are not reproducible against a
newer constitution without that review.

---

## Cited prices (evidence)

**None.** This thesis is `market_data_stage: none` and cites no prices. All evidence
is from SEC filings, XBRL facts, earnings transcripts, teardowns and trade press.

| ticker | price | price_basis | observed_at | snapshot path |
|---|---|---|---|---|
| — | — | — | — | *(no price evidence in this thesis)* |

> If Phase 5 produces trade ideas with price-based catalyst triggers, this section
> must be populated with `close`-basis quotes and snapshots written under
> `evidence/quotes/`, and the thesis re-planned as `market_data_stage: early`.

---

## Environment

| component | version / value |
|---|---|
| MCP endpoint | `https://mcp.agentii.ai/mcp` (health probe: HTTP 200 on 2026-09-10) |
| data plane | SEC filings, XBRL facts, earnings calendar, institutional holdings, insider trades |
| Python | `python3` for `data-tools/` CLI surfaces |
| Optional keys | `FRED_API_KEY` — **unset**; `fredapi` — **not installed**. Macro series were sourced from published research, not FRED. Recorded because it bounds what a reviewer can re-derive locally. |

---

## Reproduction steps

```bash
# 1. Workspace at the recorded pin
cd /Users/frank/B/agentii-physical_ai
git checkout c776860          # baseline: constitution v1.2.0 + 15 specs

# 2. Confirm the constitution pin matches this thesis
grep CONSTITUTION_VERSION constitution.md   # expect 1.2.0

# 3. Materialize tasks for this thesis
python3 scripts/agentii_cmd.py tasks \
  --thesis theses/001-physical-ai-technology-baseline/thesis.md \
  --spec   theses/001-physical-ai-technology-baseline/spec.md

# 4. Execute via the dispatch wrapper (implement)
#    Agent call tracing: include X-Agentii-Trace on every tool call.
```

---

## Known deviations from a clean reproduction

1. **`agentii_cmd.py plan` does not exist.** The `plan` skill's SKILL.md documents
   `python3 scripts/agentii_cmd.py plan --thesis <path>`, but argparse registers only
   `specify`, `tasks`, and `constitution`. This plan was authored by hand against
   `plan-template.md` rather than generated. Step 3 above uses `tasks`, which does
   exist.
2. **`frameworks` and `strategies` knowledge stores returned empty** for the
   NVDA/fundamental query on 2026-09-10. The brief records this rather than
   substituting invented references.
3. **`depth: deep` is unsafe for 62 of 71 skills.** `skill-registry.yaml` leaves
   `essentials_modes` empty for those skills, so `depth_to_modes` expands `deep` to
   the skill's `modes` list — but for these skills those slugs are **SKILL.md section
   headings** (`triggers`, `defaults`, `methodology`, `retrieval-scope`,
   `retrieval-strategy`), not analysis modes. A `deep` matrix row therefore generates
   tasks named after document structure. Skills with real modes (e.g. `business-model`:
   `business-model-classification`, `distribution-channel-analysis`, …) behave
   correctly. This thesis uses `standard` throughout. **Upstream fix needed**: populate
   `essentials_modes` for the 62 affected skills, or make `depth_to_modes` reject
   section-heading slugs.
4. **`tasks_from_spec()` dropped two fields** (fixed upstream): it hardcoded
   `{"pillar": "P1"}` so every task's `src:` was `P1` regardless of the pillar
   served, and it parsed away the matrix's Purpose column so every row read "per
   spec deployment matrix". Both defeated Q26 traceability.
5. **`agentii.clarify` scanner had two defects** (fixed upstream, kit commit
   `0b43378`): the subscription capture was not line-anchored, and its predicate
   accepted `skill × mode` in place of `TICKER × skill`. Together these produced one
   false positive per spec while missing every real violation.
6. **`dispatch.py` journals only the cwd-fallback path** (S1 scope; the full
   implement wrapper is upstream task T053). With `--thesis-dir` passed explicitly
   — the mandatory Q37 path — no journal line is written. The 24 dispatch records
   in `shards/run1.ndjson` were therefore written by the implementer via
   `journal.append_entry` with `thesis_resolution: explicit`, then reduced by
   `reduce_journals.py` (24 entries). Until T053 lands, implement must append
   explicit-path dispatch records itself or the reducer sees an empty journal.
