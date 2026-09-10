# Research Tasks: Physical AI Technology Baseline

> **APPEND-ONLY (Q26)**: this file is never rewritten, renumbered, reordered or
> deleted from. `[x]` is written by `agentii.implement` on completion and is a
> display hint — `agentii.converge` evaluates artifact state, not `[x]`. Corrections
> arrive as appended `## Phase N: Convergence` sections.

Task format: `- [ ] T### [P] [pillar] TICKER × SKILL × MODE — purpose (src: …)`

- `[P]` = different files **and** no incomplete dependencies (cross-ticker
  `_cross/` tasks are never `[P]`).
- `mode: all` expands to N tasks at generation — never exists as one task (Q79).
- `src:` is the pillar the work serves, derived from the spec's `Subscribed:`
  lists (Q9). Multi-pillar skills cite `spec-<skill>`; the bracket lists every
  pillar the skill contributes to.

**Total**: 25 tasks — 13 parallelisable, 10 serialised, 2 synthesis (never `[P]`)

## Phase 1 — Physics and Literature Baseline

- [ ] T001 [P] [PIL-1/PIL-3/PIL-4] NVDA × secular-trends × evaluate-company-s-exposure-to-major-secular-technology-trends — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [ ] T002 [PIL-1/PIL-3/PIL-4] NVDA × secular-trends × deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [ ] T003 [PIL-1/PIL-3/PIL-4] NVDA × secular-trends × deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [ ] T004 [P] [PIL-1/PIL-3/PIL-4] ISRG × secular-trends × evaluate-company-s-exposure-to-major-secular-technology-trends — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [ ] T005 [PIL-1/PIL-3/PIL-4] ISRG × secular-trends × deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [ ] T006 [PIL-1/PIL-3/PIL-4] ISRG × secular-trends × deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [ ] T007 [P] [PIL-1/PIL-3/PIL-4] TSLA × secular-trends × evaluate-company-s-exposure-to-major-secular-technology-trends — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [ ] T008 [PIL-1/PIL-3/PIL-4] TSLA × secular-trends × deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [ ] T009 [PIL-1/PIL-3/PIL-4] TSLA × secular-trends × deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)

## Phase 2 — Component Economics and Dependency

- [ ] T010 [P] [PIL-2/PIL-4] TSLA × unit-economics × default — Per-unit cost structure; PH Motion Systems segment cost stack (src: spec-unit-economics)
- [ ] T011 [P] [PIL-2/PIL-4] ISRG × unit-economics × default — Per-unit cost structure; PH Motion Systems segment cost stack (src: spec-unit-economics)
- [ ] T012 [P] [PIL-2/PIL-4] PH × unit-economics × default — Per-unit cost structure; PH Motion Systems segment cost stack (src: spec-unit-economics)
- [ ] T013 [P] [PIL-1/PIL-2] NVDA × supply-chain × default — Physical dependency mapping; actuator/motion component chain (src: spec-supply-chain)
- [ ] T014 [P] [PIL-1/PIL-2] AMZN × supply-chain × default — Physical dependency mapping; actuator/motion component chain (src: spec-supply-chain)
- [ ] T015 [P] [PIL-1/PIL-2] PH × supply-chain × default — Physical dependency mapping; actuator/motion component chain (src: spec-supply-chain)

## Phase 3 — Reliability Evidence

- [ ] T016 [P] [PIL-3/PIL-4] ISRG × operational-kpi × default — Reliability and utilisation metrics (src: spec-operational-kpi)
- [ ] T017 [P] [PIL-3/PIL-4] AMZN × operational-kpi × default — Reliability and utilisation metrics (src: spec-operational-kpi)

## Phase 4 — Risk and Timing Synthesis

- [ ] T018 [P] [PIL-3] NVDA × risk × general-risk-factors-identification-assessment — Technology and execution risk (src: PIL-3)
- [ ] T019 [PIL-3] NVDA × risk × technology-disruption-risk-analysis — Technology and execution risk (src: PIL-3)
- [ ] T020 [PIL-3] NVDA × risk × regulatory-compliance-risk-assessment — Technology and execution risk (src: PIL-3)
- [ ] T021 [P] [PIL-3] TSLA × risk × general-risk-factors-identification-assessment — Technology and execution risk (src: PIL-3)
- [ ] T022 [PIL-3] TSLA × risk × technology-disruption-risk-analysis — Technology and execution risk (src: PIL-3)
- [ ] T023 [PIL-3] TSLA × risk × regulatory-compliance-risk-assessment — Technology and execution risk (src: PIL-3)

### Synthesis deliverables (spec §6 — never `[P]`)
- [ ] T024 [PIL-1/PIL-2/PIL-3/PIL-4] _cross/technology-baseline-synthesis — dated capability timeline with confidence band (src: spec-§6)
- [ ] T025 [PIL-1/PIL-2/PIL-3/PIL-4] snapshots/001-physical-ai-technology-baseline/2026-09-10_thesis.md — thesis snapshot, derived conviction (src: spec-§6)

<!-- agentii.converge appends below this point; never edit above it -->
