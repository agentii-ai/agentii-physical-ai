# Research Tasks: Physical AI Technology Baseline

> **APPEND-ONLY (Q26)**: this file is never rewritten, renumbered, reordered or
> deleted from. `[x]` is written by `agentii.implement` on completion and is a
> display hint — `agentii.converge` evaluates artifact state, not `[x]`. Corrections
> arrive as appended `## Phase N: Convergence` sections.
> **Regeneration exception**: plan re-authoring under a constitution bump re-runs
> the `agentii.tasks` generator on the amended spec and re-derives the Convergence
> section via `agentii.converge` (rev. 4, 2026-09-10 — constitution 1.3.0 SPCX
> re-examination).

Task format: `- [ ] T### [P] [pillar] TICKER × SKILL × MODE — purpose (src: …)`

- `[P]` = different files **and** no incomplete dependencies (cross-ticker
  `_cross/` tasks are never `[P]`).
- `mode: all` expands to N tasks at generation — never exists as one task (Q79).
- `src:` is the pillar the work serves, derived from the spec's `Subscribed:`
  lists (Q9). Multi-pillar skills cite `spec-<skill>`; the bracket lists every
  pillar the skill contributes to.

**Total**: 26 tasks — 14 parallelisable, 10 serialised, 2 synthesis (never `[P]`)

## Phase 1 — Physics and Literature Baseline

- [x] T001 [P] [PIL-1/PIL-3/PIL-4] NVDA × secular-trends × evaluate-company-s-exposure-to-major-secular-technology-trends — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [x] T002 [PIL-1/PIL-3/PIL-4] NVDA × secular-trends × deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [x] T003 [PIL-1/PIL-3/PIL-4] NVDA × secular-trends × deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [x] T004 [P] [PIL-1/PIL-3/PIL-4] ISRG × secular-trends × evaluate-company-s-exposure-to-major-secular-technology-trends — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [x] T005 [PIL-1/PIL-3/PIL-4] ISRG × secular-trends × deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [x] T006 [PIL-1/PIL-3/PIL-4] ISRG × secular-trends × deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [x] T007 [P] [PIL-1/PIL-3/PIL-4] TSLA × secular-trends × evaluate-company-s-exposure-to-major-secular-technology-trends — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [x] T008 [PIL-1/PIL-3/PIL-4] TSLA × secular-trends × deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)
- [x] T009 [PIL-1/PIL-3/PIL-4] TSLA × secular-trends × deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure — Technology adoption curve and disruption timing (src: spec-secular-trends)

## Phase 2 — Component Economics and Dependency

- [x] T010 [P] [PIL-2/PIL-4] TSLA × unit-economics × default — Per-unit cost structure; PH Motion Systems segment cost stack (src: spec-unit-economics)
- [x] T011 [P] [PIL-2/PIL-4] ISRG × unit-economics × default — Per-unit cost structure; PH Motion Systems segment cost stack (src: spec-unit-economics)
- [x] T012 [P] [PIL-2/PIL-4] PH × unit-economics × default — Per-unit cost structure; PH Motion Systems segment cost stack (src: spec-unit-economics)
- [x] T013 [P] [PIL-1/PIL-2/PIL-4] NVDA × supply-chain × default — Physical dependency mapping; actuator/motion component chain; SPCX upstream capex/compute demand (timing evidence for PIL-4) (src: spec-supply-chain)
- [x] T014 [P] [PIL-1/PIL-2/PIL-4] AMZN × supply-chain × default — Physical dependency mapping; actuator/motion component chain; SPCX upstream capex/compute demand (timing evidence for PIL-4) (src: spec-supply-chain)
- [x] T015 [P] [PIL-1/PIL-2/PIL-4] PH × supply-chain × default — Physical dependency mapping; actuator/motion component chain; SPCX upstream capex/compute demand (timing evidence for PIL-4) (src: spec-supply-chain)
- [x] T016 [P] [PIL-1/PIL-2/PIL-4] SPCX × supply-chain × default — Physical dependency mapping; actuator/motion component chain; SPCX upstream capex/compute demand (timing evidence for PIL-4) (src: spec-supply-chain)

## Phase 3 — Reliability Evidence

- [x] T017 [P] [PIL-3/PIL-4] ISRG × operational-kpi × default — Reliability and utilisation metrics (src: spec-operational-kpi)
- [x] T018 [P] [PIL-3/PIL-4] AMZN × operational-kpi × default — Reliability and utilisation metrics (src: spec-operational-kpi)

## Phase 4 — Risk and Timing Synthesis

- [x] T019 [P] [PIL-3] NVDA × risk × general-risk-factors-identification-assessment — Technology and execution risk (src: PIL-3)
- [x] T020 [PIL-3] NVDA × risk × technology-disruption-risk-analysis — Technology and execution risk (src: PIL-3)
- [x] T021 [PIL-3] NVDA × risk × regulatory-compliance-risk-assessment — Technology and execution risk (src: PIL-3)
- [x] T022 [P] [PIL-3] TSLA × risk × general-risk-factors-identification-assessment — Technology and execution risk (src: PIL-3)
- [x] T023 [PIL-3] TSLA × risk × technology-disruption-risk-analysis — Technology and execution risk (src: PIL-3)
- [x] T024 [PIL-3] TSLA × risk × regulatory-compliance-risk-assessment — Technology and execution risk (src: PIL-3)

### Synthesis deliverables (spec §6 — never `[P]`)
- [x] T025 [PIL-1/PIL-2/PIL-3/PIL-4] _cross/technology-baseline-synthesis — dated capability timeline with confidence band (src: spec-§6)
- [x] T026 [PIL-1/PIL-2/PIL-3/PIL-4] snapshots/001-physical-ai-technology-baseline/2026-09-10_thesis.md — thesis snapshot, derived conviction (src: spec-§6)

<!-- agentii.converge appends below this point; never edit above it -->

## Phase 1: Convergence
- [ ] T001 [Convergence] Re-run NVDA × secular-trends × evaluate-company-s-exposure-to-major-secular-technology-trends: artifact missing (src: converge:missing id=0568ffcf4d55)
- [ ] T002 [Convergence] Re-run NVDA × secular-trends × deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure: artifact missing (src: converge:missing id=1e862a804fc2)
- [ ] T003 [Convergence] Re-run NVDA × secular-trends × deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure: artifact missing (src: converge:missing id=0806939027c2)
- [ ] T004 [Convergence] Re-run ISRG × secular-trends × evaluate-company-s-exposure-to-major-secular-technology-trends: artifact missing (src: converge:missing id=6dd027635a44)
- [ ] T005 [Convergence] Re-run ISRG × secular-trends × deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure: artifact missing (src: converge:missing id=9cd16dc59c1a)
- [ ] T006 [Convergence] Re-run ISRG × secular-trends × deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure: artifact missing (src: converge:missing id=a8548fe0a36f)
- [ ] T007 [Convergence] Re-run TSLA × secular-trends × evaluate-company-s-exposure-to-major-secular-technology-trends: artifact missing (src: converge:missing id=8d5f7aaa9e76)
- [ ] T008 [Convergence] Re-run TSLA × secular-trends × deep-dive-ai-trend-assessment-for-companies-with-identified-ai-exposure: artifact missing (src: converge:missing id=2b8a38c9dfe8)
- [ ] T009 [Convergence] Re-run TSLA × secular-trends × deep-dive-data-value-trend-assessment-for-companies-with-identified-data-exposure: artifact missing (src: converge:missing id=87b1fc0c7fca)
- [ ] T010 [Convergence] Re-run TSLA × unit-economics × default: artifact missing (src: converge:missing id=d58f1dd6983f)
- [ ] T011 [Convergence] Re-run ISRG × unit-economics × default: artifact missing (src: converge:missing id=b0b0910d63d8)
- [ ] T012 [Convergence] Re-run PH × unit-economics × default: artifact missing (src: converge:missing id=3731775d5db9)
- [ ] T013 [Convergence] Re-run NVDA × supply-chain × default: artifact missing (src: converge:missing id=2b77bfa107e5)
- [ ] T014 [Convergence] Re-run AMZN × supply-chain × default: artifact missing (src: converge:missing id=1feee3ff8799)
- [ ] T015 [Convergence] Re-run PH × supply-chain × default: artifact missing (src: converge:missing id=bfcc74c3f17a)
- [ ] T016 [Convergence] Re-run SPCX × supply-chain × default: artifact missing (src: converge:missing id=d0f9e3d5e95e)
- [ ] T017 [Convergence] Re-run ISRG × operational-kpi × default: artifact missing (src: converge:missing id=905aba8ac2da)
- [ ] T018 [Convergence] Re-run AMZN × operational-kpi × default: artifact missing (src: converge:missing id=db81df758e3d)
- [ ] T019 [Convergence] Re-run NVDA × risk × general-risk-factors-identification-assessment: artifact missing (src: converge:missing id=9a6ec8a3a1fb)
- [ ] T020 [Convergence] Re-run NVDA × risk × technology-disruption-risk-analysis: artifact missing (src: converge:missing id=c4662dd4211a)
- [ ] T021 [Convergence] Re-run NVDA × risk × regulatory-compliance-risk-assessment: artifact missing (src: converge:missing id=c098764b7171)
- [ ] T022 [Convergence] Re-run TSLA × risk × general-risk-factors-identification-assessment: artifact missing (src: converge:missing id=59ae46de8a1a)
- [ ] T023 [Convergence] Re-run TSLA × risk × technology-disruption-risk-analysis: artifact missing (src: converge:missing id=24f5db3bfc6a)
- [ ] T024 [Convergence] Re-run TSLA × risk × regulatory-compliance-risk-assessment: artifact missing (src: converge:missing id=7c90e394ccf3)
