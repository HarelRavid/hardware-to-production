# EP08 Final Script Outline — Design for Test, Calibration and Traceability

status: FINAL SCRIPT OUTLINE COMPLETE — SEASON CONTINUITY PENDING
season: Season 1
audience: electronics / embedded / mechanical / test / NPI / quality
lifecycle: DEV → LVP → SVP
source_lock: evidence/source-lock/season-1/S1C_EP08_CLAIM_LOCK.md
technical_review: evidence/source-lock/season-1/S1C_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-1/EP08_PRODUCTION_BLUEPRINT.md
research: podcast/season-2/EP08_RESEARCH_PACK.md

## Listener transformation
Before:
“Production test is a tester we design at the end.”

After:
“I can design access, observability, programming, calibration, identity and evidence linkage into the product before repeated production depends on engineer-only tools.”

## Two-character opportunity
Rona:
“The engineering laptop and debug script already prove the unit works. Why build more infrastructure?”
Oz:
Because repeated production needs a controlled, reconstructable decision system.

## Cold open
[ILLUSTRATIVE]
Unit passes only with one laptop/debug console/script; calibration lives on a technician PC; retested fail becomes stored only as PASS.

## Beat 1 — Testability is architecture
Claim: EP08-C01.
Use boundary-scan concept only optionally; do not call IEEE 1149.1-2013 active current standard.

## Beat 2 — Engineering debug vs production test
Claim: EP08-C02.
Callback to A6.

## Beat 3 — What claim does this test protect?
Claim: EP08-C03.
Requirement / CTQ / failure mode / release decision.

## Beat 4 — Measurement adequacy first
Claim: EP08-C04.
Sources: NIST measurement process/traceability.

## Beat 5 — Calibration is configuration when it affects behavior/acceptance
Claim: EP08-C05.

## Beat 6 — Identity and evidence linkage
Claim: EP08-C06.
Unit Evidence Chain.

## Beat 7 — More test is not automatically better
Claim: EP08-C07.
Coverage / escape / false reject / cycle / economics.

## Beat 8 — Production Test Architecture Map
Claim → identity/config → state → access → stimulus/reference → measurement → criterion → data → reaction → rework/retest → cycle burden → change trigger.

## Beat 9 — DEV / LVP / SVP
DEV: debug visibility.
LVP: repeatable programming/calibration/test/identity.
SVP: rate, measurement control, recovery, automation, effectivity.

## Misconceptions
- final test replaces upstream control;
- calibration sticker proves measurement fitness;
- retest can erase original fail;
- tighter test limits always improve quality;
- serial traceability requires MES immediately.

## Closing action
Pick one production-relevant test and draw the full evidence chain from product identity to final release decision.

## Handoff
EP08 makes evidence observable.
EP09 asks whether the specification and measurement system can handle real population variation.
