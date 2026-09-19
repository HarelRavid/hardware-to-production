# EP44 Script Outline V1 — Automated Inspection and End-of-Line Test

status: SCRIPT OUTLINE COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
audience: test / quality / automation / manufacturing / NPI
lifecycle: LVP → Ramp → SVP
source_lock: Wave 04 + Wave 02 measurement lock
technical_review: evidence/source-lock/wave-04/W4_INTERNAL_TECHNICAL_REVIEW.md

## Listener promise
Treat automated test as a controlled measurement/decision system with its own configuration, drift, false decisions, retest and genealogy risks.

## Cold open
[ILLUSTRATIVE] 100% automated test reports 99.8% pass. A fixture contact degrades and good units fail; later a threshold edit lets marginal units pass.

## Beat 1 — Start from claim/failure consequence
Claims: EP44-C01.
100% coverage only covers what the test can detect reliably.

## Beat 2 — Automated test evidence chain
Claims: EP44-C02
requirement/CTQ → stimulus → fixture/sensor → reference/calibration → algorithm/limit version → unit result.

## Beat 3 — Drift belongs to the test system too
Claims: EP44-C06
fixture wear, reference drift, software changes, environment.

## Beat 4 — Golden/reference unit boundary
Claim EP44-C04 dependency from Wave 02.

## Beat 5 — False accept and false reject
Keep conceptual; no unsourced guard-band statistics.

## Beat 6 — Software/limit effectivity
Claims: EP44-C03
Wave 01 configuration change.

## Beat 7 — Retest/rework history
Claim EP44-C05.
Do not test-until-pass.

## Beat 8 — Test yield vs process yield
Claim EP44-C07.
Separate test-system faults/false rejects from actual product/process first-pass failures.

## Listener tools
Automated Test Architecture Map + Test-System Drift Review.

## Misconceptions
- 100% test = zero escapes;
- automated = objective;
- golden unit = calibration;
- threshold edit is software-only;
- final PASS erases prior FAIL;
- test pass rate = process yield.

## Closing action
Pick one automated station and list every versioned element that can change PASS/FAIL without changing the product.

## Handoff
EP45 asks whether the automated system is production-ready over time, faults, maintenance and real losses.