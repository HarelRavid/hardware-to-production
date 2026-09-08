# Episode 44 Production Blueprint — Automated Inspection and End-of-Line Test

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
lifecycle: LVP → Ramp → SVP
maps_to: MASTER_WBS 8.6, 8.7

## Listener transformation
Before: assumes 100% automated inspection means strong quality control.
After: treats the automated test system as a measurement/decision process that itself requires capability, calibration, configuration, false-pass/fail control and traceable evidence.

## Narrative hook
Every unit is automatically tested and the dashboard shows 99.8% pass. A fixture contact degrades slowly and good units begin failing; later, a software threshold change lets marginal units pass. Coverage was 100%, but decision integrity was not.

## Teaching flow
1. Define the product claim and defect consequence before test architecture.
2. In-process versus EOL test and what each can still influence.
3. Sensor/fixture/interface stability and calibration.
4. Test coverage versus actual failure mechanisms.
5. Reference/golden units and limits of their use.
6. False accept and false reject as engineering/economic risks.
7. Software/configuration identity for test recipes and limits.
8. Retest/rework logic without erasing failed history.
9. Unit-level result linkage to genealogy.
10. Monitoring drift in the test system itself.

## Core framework — Automated Test Evidence Chain
`Requirement/CTQ → stimulus/measurement → fixture/sensor → calibration/reference → algorithm/limit version → unit result → false-pass/fail risk → reaction/retest logic → genealogy → monitoring`.

## Listener tools
- Automated Test Architecture Map.
- Test-System Drift Review: reference behavior, fixture wear, calibration, software/limit changes, environment, correlation and retest patterns.

## DEV / LVP / SVP
DEV: instrumentation can be flexible and diagnostic. LVP: repeatable fixtures and captured results become necessary. SVP: test configuration, measurement adequacy, maintenance, change control and genealogy must support release decisions at rate.

## Common mistakes
- 100% test = zero escape risk;
- golden unit treated as calibration by itself;
- thresholds changed without effectivity/evidence review;
- repeated retest until PASS;
- test yield used as process yield without separating test-system failures;
- automated data captured without unit/configuration context.

## Quantitative/source gate
Any GR&R/MSA thresholds, guard-band rules, uncertainty ratios, acceptance statistics or mandated calibration intervals require authoritative source, assumptions and applicability. Numerical false-pass/fail examples require audited arithmetic.

## Closing handoff
Episode 45 asks whether the automation and test systems are actually production-ready over time: qualification, OEE loss visibility and maintenance/recovery.
