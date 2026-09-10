What the reference case actually teaches

  Aschenbrenner's fund is cited for its research method, but I want to be precise about which half to copy:

  Copy: the Situational Awareness method — counting orders of magnitude, reason from physical constraints, find the bottleneck before consensus does. That is exactly our P3.

  Do not copy: the portfolio. His thesis was directionally correct (AI infrastructure bottleneck) and it still killed him — 4x leverage, concentration, correlation mismatch, and $45B trapped
  in illiquid small/mid caps. −67% in July, portfolio sold to Citadel at >10% discount.

  Our P7 already blocks most of this (8% max single, 12 positions). It does not explicitly prohibit leverage. Given the reference case, I think it should.

  Two findings that invert the obvious trade

  1. Compute is not where the money is. BOM teardowns, 2026:

  ┌────────────────────────────────────────┬────────────────────────┐
  │                 Layer                  │      Share of BOM      │
  ├────────────────────────────────────────┼────────────────────────┤
  │ Actuators + screws + reducers + motors │ 40–70%                 │
  ├────────────────────────────────────────┼────────────────────────┤
  │ Six-axis force/torque sensors          │ 11–18%                 │
  ├────────────────────────────────────────┼────────────────────────┤
  │ Compute / AI stack                     │ only 10–15%            │
  ├────────────────────────────────────────┼────────────────────────┤
  │ Battery                                │ ~0.5% (rounding error) │
  └────────────────────────────────────────┴────────────────────────┘

  Planetary roller screws alone run 19–35% — 14 units × ~$1,350–2,700. The market models physical AI as a compute story. The BOM says the value pool is actuation and sensing. That gap is the
  variant perception.

  2. The bottleneck is data, not compute. Robotics foundation models use ~1% of frontier training compute — not from GPU scarcity, but because there's no data to feed them. Embodied data sits
  ~10,000× behind LLM pretraining corpora; teleoperation is capped at 24h/robot/day. A ~7B-parameter "ossification" threshold has been observed, and Agibot pegs the GPT-3.5 moment at late
  2027–early 2028. Anyone underwriting a 2026 robotics revenue inflection is early.

  Also: Chinese supply delivers ~$46K BOM vs ~$131K non-Chinese — ~3×. That's a supply-chain dependency thesis in itself.

  Proposed architecture — 14 theses, 5 phases

  │   #   │               Slug               │ Phase │  Depends  │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-001 │ physical-ai-technology-baseline  │ 0     │ —         │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-002 │ value-chain-profit-pool-map      │ 1     │ T-001     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-003 │ actuation-motion-chokepoint      │ 1     │ T-001     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-004 │ perception-force-sensing         │ 1     │ T-001     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-005 │ embodied-data-model-layer        │ 1     │ T-001     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-006 │ critical-materials-rare-earth    │ 1     │ T-001     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-007 │ chokepoint-pricing-power         │ 2     │ T-002…006 │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-008 │ nvidia-physical-ai-compute       │ 3     │ T-007     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-009 │ qualcomm-edge-robotics           │ 3     │ T-007     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-010 │ parker-hannifin-motion           │ 3     │ T-007     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-011 │ vision-stack-amba-cgnx           │ 3     │ T-007     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-012 │ tesla-humanoid-optionality       │ 3     │ T-007     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-013 │ industrial-automation-incumbents │ 3     │ T-007     │
  ├───────┼──────────────────────────────────┼───────┼───────────┤
  │ T-014 │ portfolio-construction-hedge     │ 4     │ T-008…013 │
  └───────┴──────────────────────────────────┴───────┴───────────┘

  T-001 is the Aschenbrenner analogue — "Counting the OOMs" for embodied AI: what must be physically true about torque density, BOM cost curve, data volume, and reliability for humanoids to
  reach economic parity.

  One correction to my own work

  My P2 table said 15 analyzable names. I checked ~20 more and it's substantially wider — MBLY, MU, TXN, NXPI, HON, SYK, AMZN, INTC, TSM, KLAC, LRCX, APH, GE, MMM, F all return filings and
  documents. Roughly 30 names, enough for a real portfolio. P2 needs another amendment. (Still not retrievable: RRX, TKR, ALNT, NOVT, MOG.A, VPG, ROK, SYM, MP, ZBRA, MDT, TDY, TEL — the
  actuator pure-plays remain blocked.)

  Three decisions before I scaffold:

───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
←  ☒ Granularity  ☐ Uncovered names  ☐ Leverage rule  ✔ Submit  →

Thesis decomposition granularity — how many theses and at what split?

❯ 1. 14 theses / 5 phases  ✔      ┌───────────────────────────────────────────────────┐
    (Recommended)                 │ PHASE 0  T-001 technology baseline                │
  2. 10 theses / 4 phases         │ PHASE 1  T-002 profit pool map                    │
  3. 18 theses / 6 phases         │          T-003 actuation chokepoint               │
                                  │          T-004 perception/sensing                 │
                                  │          T-005 embodied data layer                │
                                  │          T-006 critical materials                 │
                                  │ PHASE 2  T-007 chokepoint synthesis               │
                                  │ PHASE 3  T-008 NVDA    T-011 vision               │
                                  │          T-009 QCOM    T-012 TSLA                 │
                                  │          T-010 PH      T-013 industrials          │
                                  │ PHASE 4  T-014 portfolio + hedge                  │
                                  │                                                   │
                                  │ 42 files (spec + thesis + checklist)              │
                                  └───────────────────────────────────────────────────┘


                                   Uncovered names  ☐ Leverage rule  ✔ Submit  →

The 9 actuator pure-plays (RRX, TKR, ALNT, NOVT, MOG.A, VPG, ROK, SYM, MP) have no retrievable agentii data. How should theses handle them?

 1. Dedicated watchlist thesis    ┌───────────────────────────────────────────────────┐
   (Recommended)                  │ T-00X  uncovered-actuator-watchlist               │
  2. Exclude entirely             │                                                   │
  3. Mention in map only          │ Pillar P1: RRX/TKR/ALNT are the consensus         │
                                  │            picks-and-shovels complex              │
                                  │   wrong_if: metric=agentii_xbrl_fact_count        │
                                  │             threshold=0                           │
                                  │             source=search_xbrl_facts              │
                                  │                                                   │
                                  │ Pillar P2: PH is the only analyzable              │
                                  │            motion-control proxy                   │
                                  │                                                   │
                                  │ Output: coverage-gap register +                   │
                                  │         data-acquisition request                  │
                                  └───────────────────────────────────────────────────┘


 ☐ Leverage rule  ✔ Submit  →

Add an explicit leverage prohibition to the constitution? The Aschenbrenner case is the direct precedent — a directionally correct thesis destroyed by 4x leverage.

 1. Yes — add P7.1                ┌───────────────────────────────────────────────────┐
   (Recommended)                  │ P7.1 — No leverage. The portfolio operates        │
  2. No — P7 already covers it    │ unlevered. No margin, no options-based            │
                                  │ implicit leverage, no borrow against              │
                                  │ positions. The Situational Awareness case         │
                                  │ (directionally correct thesis, −67% in one        │
                                  │ month at 4x) is the standing precedent.           │
                                  │                                                   │
                                  │ P7.2 — Liquidity. No position may exceed          │
                                  │ X% of 20-day ADV. $45B trapped in                 │
                                  │ small/mid caps was the terminal failure.          │
                                  └───────────────────────────────────────────────────┘


15 theses scaffolded, verified, ready

  All from the same build at 15:01 — nothing clobbered. 64 skill-matrix rows decompose with zero spurious entries, and all 47 wrong_if triples carry metric + threshold + source.

  PHASE 0  T-001  technology baseline          ← gates everything
  PHASE 1  T-002  value-chain profit pool map
           T-003  actuation / motion chokepoint
           T-004  perception / force sensing
           T-005  embodied data / model layer
           T-006  critical materials / rare earth
           T-007  uncovered actuator watchlist
  PHASE 2  T-008  chokepoint pricing power      ← gates Phase 3
  PHASE 3  T-009 NVDA   T-012 AMBA/CGNX
           T-010 QCOM   T-013 TSLA
           T-011 PH     T-014 industrials
  PHASE 4  T-015  portfolio construction + hedge

  Your 5 steps map to it directly: technology/science foundation → T-001; industry + supply-chain map → T-002–T-007; key technical/product chokepoints → T-003, T-004, T-008; listed +
  non-listed companies → T-007 (watchlist); company research → T-009–T-014; portfolio → T-015.

  Toward buy-side standard

  The Aschenbrenner method is encoded as T-001 — "Counting the OOMs" for embodied AI: what must be physically true about torque density, BOM cost, data volume, and reliability for parity.
  Every downstream thesis inherits its assumptions, and the specs state that its falsification triggers a MAJOR re-examination.

  P7.1 and P7.2 are now in force (constitution.yaml has 7 constraints incl. LEVERAGE and LIQUIDITY_ADV). The reference fund's method is copied; its financing is not.

  The 47 falsifiers are the real deliverable. Each is machine-checkable — e.g. T-003 P1: planetary_roller_screw_share_of_bom_pct < 15 kills the chokepoint thesis. That's the difference
  between a research document and a position you can be wrong about on purpose.

  Three things you should know

  1. Another session wrote macro-plan_0910-1457.md (13.8 KB) while I worked. I haven't touched it. It contains my analysis text — the Aschenbrenner framing, the BOM table, the two inversions
  — reformatted with box-drawing characters. Either it's a parallel session capturing this conversation, or it's a copy of my output. Worth confirming it's not duplicating work. The zip was
  also renamed 0910-1433-contitution-templates.zip → backup-contitution-templates_0910-1433.zip.

  2. I found and fixed a real bug in my own work, then found one upstream. My first frontmatter pass emitted flow-style YAML that broke on unquoted > and , — all 15 specs failed to parse. I
  rewrote it as block-style YAML via yaml.safe_dump and added a parse-before-write assertion. Separately, the kit's two spec templates disagree: spec-template.md emits a 7-dash separator
  (|-------|), while parse_spec_matrix only skips the exact string ---. Feeding a template-derived spec to agentii_cmd tasks yields a phantom row (skill='-------'). specify() is unaffected —
  it inlines a 3-dash header. That's an upstream fix for the same session that added the scaffold guard.

  3. My own verification was briefly wrong. A path typo (underscore vs hyphen) made me report "0 rows parsed" when the files were fine. I caught it by tracing the parser line-by-line rather
  than trusting the summary.

  The specs/ skill is at 70 skills — /agentii:plan is the next step, which turns each spec's phases into a dated task plan and hits gate 2. Want me to run it on T-001 first, or plan all 15?


