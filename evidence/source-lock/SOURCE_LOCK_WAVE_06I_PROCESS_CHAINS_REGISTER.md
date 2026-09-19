# Source-Lock Wave 06I — Manufacturing Process Chains Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP19 — Manufacturing Process Chains: The Sequence Is Part of the Design
dependencies:
- Wave 06A process selection
- Wave 06B polymers
- Wave 06C metals
- Wave 06D joining
- Wave 06E composites
- Wave 06F ceramics/powder/sintering
- Wave 06G additive
- Wave 06H surface/cleaning/heat treatment
- Wave 01 configuration/change
- Wave 02 quality/measurement
- Wave 03 yield/capacity/economics

## 1. Purpose

Lock the generic engineering premises required to treat a manufacturing route as a sequence of state transformations rather than isolated process operations.

EP19 does not define a universal routing standard.

## 2. External / prior-source basis

### W6I-S01 — NIST Conceptual Process Planning
Dependency:
Wave 06A.

Support:
process planning includes process selection, resource selection, cost and time estimation and belongs with design.

### W6I-S02 — Wave 06B–06H process-family source locks
Support:
each operation can change geometry, material state, surface state, joining state, inspection evidence and downstream compatibility.

### W6I-S03 — Wave 01 configuration/change
Support:
changes require dependency-based evidence reassessment and effectivity.

### W6I-S04 — Wave 02 measurement/quality
Support:
measurement adequacy and failure/rework history must remain visible.

### W6I-S05 — Wave 03 yield/economics
Support:
rework/yield/capacity/cost per accepted good unit are system-level outcomes.

## 3. EP19 engineering claims

### W6I-C01 — a manufacturing route is a chain of state transformations, not merely a list of independent processes
Status: V6 SYNTHESIS supported by W6I-S01/S02.

### W6I-C02 — the output state of one operation becomes the input state/constraint of the next
Status: V6 SYNTHESIS.

### W6I-C03 — later operations can invalidate earlier dimensional/surface/material evidence when they change a dependency that evidence relied on
Status: DEPENDENCY — Wave01 + Wave06C/06H.

### W6I-C04 — datum/reference strategy can migrate through process sequence and should be reviewed at the stage where final function is established
Status: V6 SYNTHESIS + EP09/EP18 dependencies.

### W6I-C05 — cleaning/surface/joining/thermal compatibility is sequence dependent
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Dependencies: Wave06D/06H.

### W6I-C06 — rework loops add history and can create a new process/configuration state
Status: GLOBAL INVARIANT + Wave01/02.

### W6I-C07 — inspection should be placed where the measurement is both actionable and still valid for the later product state
Status: V6 SYNTHESIS + Wave02.

### W6I-C08 — cumulative final yield can be modeled by multiplying step yields only when the population/step assumptions make that model appropriate
Status: V6 QUANTITATIVE GUARDRAIL.

### W6I-C09 — chain economics should be evaluated per accepted final output, not by optimizing isolated operation cost
Status: DEPENDENCY — Wave03.

### W6I-C10 — process-sequence changes require effectivity/evidence review when they alter the demonstrated product/process state
Status: DEPENDENCY — Wave01.

### W6I-C11 — DEV/LVP simplified routes can be legitimate bridge chains when evidence limits/expiration are explicit
Status: DEPENDENCY — A4/Wave06A.

### W6I-C12 — final release evidence belongs after all state-changing operations relevant to the product claim
Status: V6 SYNTHESIS.

## 4. Illustrative cumulative-yield rule

If independent/conditional step-yield assumptions are explicitly appropriate:

Final yield = product of step yields.

This is a teaching model only.

Do NOT infer:
- independence automatically;
- stable populations automatically;
- no rework loops;
- no correlated defects;
- no shared upstream causes.

Any numerical example must state its assumptions and be independently checked.

## 5. Hard guardrails

1. no universal routing standard;
2. no universal operation sequence;
3. no assumption each process can be optimized independently;
4. no measurement treated as permanently valid after later state-changing operations;
5. no cumulative-yield multiplication without assumptions;
6. no final PASS erasing intermediate fail/rework history;
7. no process-sequence change without impact/effectivity review;
8. no one process-family standard generalized across the whole route;
9. no local cost improvement accepted as system economics without downstream effects;
10. no “inspect everything at the end” default.

## 6. Episode gate

EP19 can proceed using already verified process-family/source locks and system-level invariants.

Current generic-script P0 blockers: 0.
