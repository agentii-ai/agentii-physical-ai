# Research Tasks: Value Chain Profit Pool Map

> **APPEND-ONLY (Q26)**: this file is never rewritten, renumbered, reordered or
> deleted from. `[x]` is written by `agentii.implement` on completion and is a
> display hint — `agentii.converge` evaluates artifact state, not `[x]`. Corrections
> arrive as appended `## Phase N: Convergence` sections.
> **Regeneration exception**: plan re-authoring under a constitution bump re-runs
> the `agentii.tasks` generator on the amended spec and re-derives the Convergence
> section via `agentii.converge`.

Task format: `- [ ] T### [P] [pillar] TICKER × SKILL × MODE — purpose (src: …)`

- `[P]` = different files **and** no incomplete dependencies (cross-ticker
  `_cross/` tasks are never `[P]`).
- `mode: all` expands to N tasks at generation — never exists as one task (Q79).
- `src:` is the pillar the work serves, derived from the spec's `Subscribed:`
  lists (Q9). Multi-pillar skills cite `spec-<skill>`; the bracket lists every
  pillar the skill contributes to.

**Total**: 21 tasks — 15 parallelisable, 4 serialised (business-model modes 2–3), 2 synthesis (never `[P]`)
**Generated**: 2026-09-10, from spec pin 1.3.0 (plan rev. 5; clarify rounds 2–4)

## Phase 1 — Layer Definition

- [x] T001 [P] [PIL-3] PH × business-model × business-model-classification — Business-model classification of layer economics (src: PIL-3)
- [x] T002 [PIL-3] PH × business-model × distribution-channel-analysis — Business-model classification of layer economics (src: PIL-3)
- [x] T003 [PIL-3] PH × business-model × revenue-composition-and-concentration — Business-model classification of layer economics (src: PIL-3)
- [x] T004 [P] [PIL-3] ISRG × business-model × business-model-classification — Business-model classification of layer economics (src: PIL-3)
- [x] T005 [PIL-3] ISRG × business-model × distribution-channel-analysis — Business-model classification of layer economics (src: PIL-3)
- [x] T006 [PIL-3] ISRG × business-model × revenue-composition-and-concentration — Business-model classification of layer economics (src: PIL-3)

## Phase 2 — Profit Quantification

- [x] T007 [P] [PIL-1/PIL-2] NVDA × supply-chain × default — Value-chain mapping and dependency (src: spec-supply-chain)
- [x] T008 [P] [PIL-1/PIL-2] PH × supply-chain × default — Value-chain mapping and dependency (src: spec-supply-chain)
- [x] T009 [P] [PIL-1/PIL-2] ISRG × supply-chain × default — Value-chain mapping and dependency (src: spec-supply-chain)
- [x] T010 [P] [PIL-1/PIL-2] AMBA × supply-chain × default — Value-chain mapping and dependency (src: spec-supply-chain)
- [x] T011 [P] [PIL-1/PIL-2] CGNX × supply-chain × default — Value-chain mapping and dependency (src: spec-supply-chain)
- [x] T012 [P] [PIL-1/PIL-2] SPCX × supply-chain × default — Value-chain mapping and dependency (src: spec-supply-chain)
- [x] T013 [P] [PIL-1] ISRG × unit-economics × default — Cost stack decomposition (src: PIL-1)
- [x] T014 [P] [PIL-1] TSLA × unit-economics × default — Cost stack decomposition (src: PIL-1)
- [x] T015 [P] [PIL-3] PH × revenue-decomp × default — Revenue mix and mix-shift (src: PIL-3)
- [x] T016 [P] [PIL-3] ISRG × revenue-decomp × default — Revenue mix and mix-shift (src: PIL-3)

## Phase 3 — Durability Assessment and Synthesis

- [x] T017 [P] [PIL-1/PIL-2] PH × competitive-positioning × default — Layer-level competitive structure (src: spec-competitive-positioning)
- [x] T018 [P] [PIL-1/PIL-2] NVDA × competitive-positioning × default — Layer-level competitive structure (src: spec-competitive-positioning)
- [x] T019 [P] [PIL-1/PIL-2] AMBA × competitive-positioning × default — Layer-level competitive structure (src: spec-competitive-positioning)

### Synthesis deliverables (spec §6 — never `[P]`)
- [x] T020 [PIL-1/PIL-2/PIL-3] _cross/002-value-chain-profit-pool-map_synthesis — layer profit-pool map with pillar verdicts and the four falsifier test results (src: spec-§6)
- [x] T021 [PIL-1/PIL-2/PIL-3] snapshots/002-value-chain-profit-pool-map/2026-09-10_thesis.md — thesis snapshot, derived conviction (src: spec-§6)

<!-- agentii.converge appends below this point; never edit above it -->
