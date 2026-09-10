# Reproduce — Value Chain Profit Pool Map

> Q8 contract 5 / Q36: the thesis-level reproduction recipe. This is the **one file**
> an external reviewer needs to reconstruct the work. Every artifact's own
> frontmatter carries its pins; this file aggregates them.

**Thesis**: `theses/002-value-chain-profit-pool-map/`
**Generated**: 2026-09-10
**Workspace**: `/Users/frank/B/agentii-physical-ai`
**Git**: branch `main` (per workspace directive)

---

## Skills used

| skill | mode | version_hash (skill_pin) |
|---|---|---|
| `supply-chain` | standard | `8cb3ac1de486` |
| `unit-economics` | standard | `e87ee63269a2` |
| `competitive-positioning` | standard | `61f794be22a5` |
| `revenue-decomp` | standard | `037b396ab004` |
| `business-model` | standard (3 essentials modes) | `9479220eef91` |

**Skill source**: `agentii-investment-intelligence` installed flat to
`~/.claude/skills/agentii/`.

---

## Pins at generation

| pin | value | note |
|---|---|---|
| `constitution_pin` | **`1.3.0`** | P2 extended ~30 → ~31 names (SPCX added); P8 PDCA added |
| `assumption_pin` | **`1`** | `assumptions.yaml` v1, effective 2026-09-10 |
| `corpus_version` | `agentii-2026-09-10` | Workspace retrieval snapshot |
| `as_of` | **2026-09-11** | Date of all retrieval (artifacts carry 2026-09-11; plan/spec authored 2026-09-10) |
| `skill_pin` | per-skill hashes | recorded to `skill_pins.jsonl` at implement (Q57) |
| `plan_rev` | `5` | rev. 1: clarify rounds 2–3 resolved (pin re-ratified 1.3.0, 7-name universe, equal weights, standard depth, 4 falsifiers with round-3 evaluation rules). rev. 2 optimization: four orphan matrix pairs subscribed to P1 (15 matrix = 15 subscriptions), competitive-positioning moved to Phase 3 (spec §7 durability semantics), brief.md installed-base figure corrected. rev. 3 optimization: PIL-1b falsifier re-scoped from a level ratio to a trend metric (`motion_model_gm_gap_change_pp < -10`, clarify round 4 — the level comparison was pre-falsified by T-001's audited anchors); YAML subscriptions synced to prose. rev. 4 optimization: stale falsifier reference in the T-001-inputs section corrected; risk note 7 added (PIL-1a range straddles the 55% threshold; PIL-1b gap-change requires like-for-like fiscal-period pairing across five calendars). rev. 5 optimization: side-artifacts table's stale plan_rev reference corrected; spec §5 T-008 parenthetical fixed (pricing power); Q29 pre-flag section added (CHK003 structurally N/A for a fixed 7-name map; P6 checklist flag recorded) |

**Reproducibility caveat.** A reader reconstructing this work at a later date must
supply `constitution_pin: 1.3.0` and `assumption_pin: 1`. A MINOR/MAJOR
constitution bump marks this thesis `stale` and dispatches re-examination (Q33).

---

## Cited prices (evidence)

**None.** This thesis is `market_data_stage: none` and cites no prices. All evidence
is from SEC filings, XBRL facts, and earnings transcripts.

> If a later phase introduces price-based triggers, the thesis must be re-planned
> as `market_data_stage: early` and `entities.md` extended with the bars schema
> before implement (Q42).

---

## Environment

| component | version / value |
|---|---|
| MCP endpoint | `https://mcp.agentii.ai/mcp` (health probe: HTTP 200 on 2026-09-10, carried from T-001) |
| data plane | SEC filings, XBRL facts, earnings calendar |
| Python | `python3` for `data-tools/` CLI surfaces |

---

## Reproduction steps

```bash
# 1. Workspace at the recorded pin
cd /Users/frank/B/agentii-physical-ai
git log --oneline -3 constitution.md     # expect 1.3.0 (SPCX in P2)

# 2. Confirm the constitution pin matches this thesis
grep CONSTITUTION_VERSION constitution.md   # expect 1.3.0

# 3. Materialize tasks for this thesis
python3 scripts/agentii_cmd.py tasks \
  --thesis theses/002-value-chain-profit-pool-map/thesis.md \
  --spec   theses/002-value-chain-profit-pool-map/spec.md

# 4. Execute via the dispatch wrapper (implement) — explicit --thesis-dir;
#    journal records appended via journal.append_entry (see deviation 2)
```

---

## Known deviations from a clean reproduction

1. **`agentii_cmd.py plan` does not exist.** The `plan` skill's SKILL.md documents
   `python3 scripts/agentii_cmd.py plan --thesis <path>`, but argparse registers only
   `specify`, `clarify`, `tasks`, and `constitution`. This plan was authored by hand
   against `plan-template.md` rather than generated (carried from T-001 deviation #1).
2. **`dispatch.py` journals only the cwd-fallback path** (carried from T-001
   deviation #6): with `--thesis-dir` explicit — the mandatory Q37 path — no
   journal line is written. The dispatcher must append dispatch records itself via
   `journal.append_entry` with `thesis_resolution: explicit` before reduction.
3. **Depth hazard** (carried from T-001 deviation #3): `deep` expands to
   SKILL.md section-heading slugs for skills with empty `essentials_modes`
   (`supply-chain`, `unit-economics`, `competitive-positioning`, `revenue-decomp`).
   This thesis runs `standard` on every matrix row; `business-model` is the only
   skill with real essentials modes (3 modes at standard).
4. **AMBA/CGNX single revenue concept**: both tag only
   `RevenueFromContractWithCustomerExcludingAssessedTax`; `us-gaap:Revenues`
   returns zero facts. P2.1 is satisfied by multi-period facts reconciled to
   income-statement tables — the pattern T-001 documented for ISRG/TSLA/PH/SPCX.
5. **PIL-2's China-ratio claim is an industry estimate** (macro-plan teardowns,
   $46K vs $131K) that cannot trace to agentii data — Deviation Register entry,
   expiry 2026-10-10, governed by the clarify round-3 evaluation rules.
