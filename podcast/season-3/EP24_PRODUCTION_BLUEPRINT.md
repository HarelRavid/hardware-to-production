# Episode 24 Production Blueprint — Production Testing and Measurement-System Capability

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
lifecycle: LVP → Production Validation → Ramp

## Listener transformation
Before: assumes a test is useful if it produces a PASS/FAIL result.
After: can judge whether the measurement system, fixture, method, criteria and traceability are capable of supporting the production decision.

## Narrative hook
Two stations test the same unit and disagree. The process is blamed for instability, but the real variation is fixture alignment, instrument drift and operator setup. The factory is reacting to measurement noise as if it were product truth.

## Teaching flow
1. Test claim and decision first.
2. Measurement error versus process/product variation.
3. Repeatability, reproducibility, bias, stability and resolution concepts.
4. Fixture/reference/calibration state.
5. Guard bands and false accept/reject concepts.
6. Golden/reference units and verification routines.
7. Production cycle-time/economic burden.
8. Failure/retest history and traceability.
9. When measurement-system evidence must be re-established after change.

## Core framework — Measurement Decision Chain
`Claim/CTQ → method → instrument/fixture → reference/calibration → uncertainty/variation contribution → acceptance rule → reaction → data identity → retest/rework history → change trigger`.

## DEV/LVP/SVP
DEV: engineering instruments may be adequate for learning if limitations are visible. LVP: repeatable fixtures/methods and measurement evidence become necessary. SVP: measurement capability, maintenance, calibration, automation and effectivity must support rate and risk.

## Common mistakes
- tighter test limits than credible measurement capability;
- PASS/FAIL with no raw/traceable evidence where needed;
- GR&R threshold applied blindly across contexts;
- golden unit treated as calibration standard without control;
- retest erasing original failure;
- confusing instrument calibration with complete measurement-system capability.

## Source/evidence backlog
AIAG MSA, ISO/IEC 17025 concepts, JCGM/GUM and sector-specific metrology requirements require exact source/applicability. No universal GR&R threshold enters script without context.

## Closing handoff
Episode 24 makes production decisions trustworthy. Episode 25 arranges people, material and equipment so the process can flow safely and efficiently.
