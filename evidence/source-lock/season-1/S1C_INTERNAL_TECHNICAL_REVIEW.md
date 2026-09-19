# Season 1 S1-C Internal Technical Review — EP06 / EP07 / EP08 / EP09 / EP10

status: PASS TO FINAL SCRIPT OUTLINE
review_date: 2026-09-19
review_type: internal technical / standards-status / quantitative-boundary review
human_independent_review: NOT CLAIMED

inputs:
- SOURCE_LOCK_SEASON_1_S1C_DFX_TEST_TOL_RELIABILITY_REGISTER.md
- S1C_EP06–EP10 claim locks
- EP06–EP10 Production Blueprints
- DFX Source Map
- Waves 01/02/03
- Season 1 Full Review V2

## EP06 — DFM

Result: PASS.

Guards:
- DFM is process/material/equipment specific;
- no generic wall/draft/tolerance/capability heuristics;
- cost comparison uses accepted-good-output logic;
- supplier DFM advice is input, not automatic design authority;
- preserve requirement/change control.

Claude note:
Use a CNC-to-molding transition to show that DFM is process matching, not a checklist.

## EP07 — DFA / Mistake Prevention

Result: PASS.

Guards:
- DFA broader than part-count reduction;
- no formal poka-yoke hierarchy attributed without source;
- no generic torque/joint rule;
- distinguish design ambiguity from operator error;
- source detection/prevention framed as engineering options, not universal mandate;
- final controls still require effectiveness evidence.

Claude note:
The practitioner character should defend the expert assembler and ask why training is not enough.

## EP08 — DFT / Calibration / Traceability

Result: PASS.

Guards:
- testability is architecture + measurement + evidence;
- calibration alone does not prove measurement fitness;
- no universal MSA/GR&R threshold, calibration interval, coverage percentage or retention rule;
- IEEE 1149.1-2013 must not be called an active current standard;
- if boundary scan appears, it is an architecture example only;
- EP08 owns product/test architecture, not full metrology depth.

Claude note:
Anchor the dialogue in an engineering laptop/debug script/calibration file dependency.

## EP09 — Tolerance / GD&T / GPS

Result: PASS WITH STRICT STANDARD-SYSTEM BOUNDARY.

Current status verified:
- ASME Y14.5-2018 (R2024) remains in effect;
- ISO 8015:2011 current;
- ISO 1101:2017 current;
- ISO 5459:2024 current and replaces 2011;
- ISO 2692:2021 current.

Guards:
1. do not teach protected clause/default/modifier rules from memory;
2. do not blend ASME Y14.5 and ISO GPS rules;
3. datum concept may be taught generically; exact semantics stay system-specific;
4. RSS example requires explicit assumptions;
5. worst-case is not expected yield;
6. measurement adequacy before capability inference;
7. no universal capability ratio/threshold.

Illustrative arithmetic:
- Stack A worst-case ±0.45 mm; RSS ≈ ±0.2693 mm.
- Stack B worst-case ±0.20 mm; RSS ≈ ±0.1225 mm.
Arithmetic: PASS.

Claude note:
Use the enclosure/PCB/connector stack to show why tightening every tolerance is not the first solution.

## EP10 — Reliability / Service / Repair

Result: PASS.

Guards:
- reliability linked to failure mechanisms/use stresses/configuration;
- accelerated testing only supports mechanisms/models validly exercised;
- do not introduce universal Arrhenius/Weibull/MTBF/sample-size/confidence targets unless separately sourced;
- no “qualification passed = field reliability proven”;
- serviceability is product-strategy dependent;
- field events remain population-scoped and configuration-linked;
- repair preserves failure/repair history.

Claude note:
Use a field-return cluster with weak genealogy to close Season 1's evidence loop.

## Cross-episode ownership

EP06 owns:
product-process manufacturability fit.

EP07 owns:
assembly ambiguity / mistake prevention.

EP08 owns:
testability / calibration / traceable release evidence architecture.

EP09 owns:
functional tolerance / datum/reference / variation reasoning.

EP10 owns:
reliability / service / field feedback.

A5/A6 remain prototype-evidence owners.
EP23/24/32 remain deeper quality/metrology/SPC owners.
Season 2 remains process-family depth.

Result:
PASS — no overlap requiring restructuring.

## Decision

EP06: PASS TO FINAL SCRIPT OUTLINE.
EP07: PASS TO FINAL SCRIPT OUTLINE.
EP08: PASS TO FINAL SCRIPT OUTLINE.
EP09: PASS TO FINAL SCRIPT OUTLINE.
EP10: PASS TO FINAL SCRIPT OUTLINE.

**SEASON 1 S1-C TECHNICAL REVIEW: PASS**
