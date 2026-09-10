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
| `secular-trends` | default | *(populated at implement)* |
| `business-model` | default | *(populated at implement)* |
| `operational-kpi` | default | *(populated at implement)* |
| `recent-quarter` | default | *(populated at implement)* |
| `risk` | default | *(populated at implement)* |
| `supply-chain` | deep | *(populated at implement)* |
| `unit-economics` | standard | *(populated at implement)* |

**Skill source**: `agentii-investment-intelligence` @ `75ce82d`, installed flat to
`~/.claude/skills/agentii/` (70 skills, 248 reference files).

---

## Pins at generation

| pin | value | note |
|---|---|---|
| `constitution_pin` | **`1.2.0`** | P2 corrected 12→15→~30 names; P7.1 (no leverage) and P7.2 (liquidity) added |
| `assumption_pin` | **`1`** | `assumptions.yaml` v1, effective 2026-09-10 |
| `corpus_version` | `agentii-2026-09-10` | Workspace retrieval snapshot |
| `as_of` | **2026-09-10** | Date of all retrieval in this plan |
| `skill_pin` | `75ce82d` | Kit commit; per-skill hashes populate at implement |

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
