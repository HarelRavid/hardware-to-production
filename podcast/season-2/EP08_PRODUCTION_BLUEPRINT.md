# Episode 8 Production Blueprint — Design for Test, Calibration and Traceability

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 2 — Turn the Prototype into a Product

## Listener transformation
The listener learns to design testability, calibration and evidence linkage into the product architecture rather than bolting them onto the end of the line.

## Narrative hook
The engineering unit passes only when a laptop, debug console and one specific script are available. Calibration values live on a technician computer. A retested failed unit ends up recorded only as PASS. Production can build the unit, but cannot prove what happened to it.

## Teaching flow
1. Design for Test as a product-architecture topic.
2. Define the claim each test/calibration step protects.
3. Access, observable states, programming/configuration and fixture strategy.
4. Measurement adequacy before trusting PASS/FAIL or capability conclusions.
5. Unit identity and evidence linkage.
6. Unit Evidence Chain from definition through rework/release.
7. Test-Debt Scan.
8. Sentinel progression from engineering laptop to controlled LVP station.
9. Explain why more testing is not automatically better quality.

## Listener tools
**Production Test Architecture Map:** `Claim → Identity/configuration → State → Access → Stimulus/reference → Measurement → Criterion → Data → Reaction → Rework/retest → Cycle burden → Change trigger`.

**Unit Evidence Chain:** `Identity → Configuration → Programming → Calibration → Procedure/version → Result → Deviation/rework/retest → Release`.

## DEV/LVP/SVP
DEV: maximize observability and debug speed while labeling engineering-only dependencies. LVP: repeatable programming/calibration/test, identity, controlled criteria and failure history. SVP: rate, measurement-system control, fixture/reference recovery, automation and effectivity.

## Common mistakes
- Final test treated as a substitute for upstream control.
- Calibration data detached from unit/configuration identity.
- Retest erasing original failure history.
- Test criteria tighter than credible measurement capability.
- Serial traceability assumed to require enterprise MES immediately.

## Source/evidence backlog
MSA thresholds, calibration intervals, retention periods, sampling rules and sector-specific test requirements remain exact-source/applicability gated.

## Closing handoff
Episode 8 makes evidence observable and reconstructable. Episode 9 asks whether the specification and measurement system can cope with real dimensional variation across a population.
