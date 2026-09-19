# A6 Final Script Outline — Serious Electronics & Embedded Prototype

status: FINAL SCRIPT OUTLINE COMPLETE — SEASON CONTINUITY PENDING
season: Season 1
audience: founders / electronics / embedded / test / NPI
lifecycle: DEV → early LVP bridge
source_lock: evidence/source-lock/season-1/S1A_A6_CLAIM_LOCK.md
technical_review: evidence/source-lock/season-1/S1A_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-1/A6_PRODUCTION_BLUEPRINT.md
research: podcast/season-1/A6_RESEARCH_PACK.md

## Listener transformation
Before:
“The circuit and firmware work on the bench.”

After:
“I can identify the controlled hardware/firmware/configuration evidence required before repeated builds and production-test decisions become trustworthy.”

## Two-character opportunity
Speaker B:
“The dev board works perfectly. Why not just copy the schematic?”
Speaker A:
Because the dev platform supplies infrastructure and assumptions that may not exist in the product.

## Cold open
[ILLUSTRATIVE]
Dev-board demo is flawless; custom PCB resets under load, firmware differs between units, programming needs one engineer’s laptop and calibration constants live in a folder.

## Beat 1 — Bench success includes invisible infrastructure
Claim: A6-C02.
Power / clock / protection / reset / debugger / programming / logging / access.
Guard:
examples, not universal dev-board failure modes.

## Beat 2 — Electronics maturity is multidimensional
Claim: A6-C01.
Function / margins / interfaces / FW config / components / assembly / testability / environment.

## Beat 3 — Controlled build identity
Claim: A6-C03.
Unit ID → PCB/HW rev → BOM rev → firmware/build → config/calibration → programming method → test result → deviations/rework.
Use KiCad/Zephyr/Espressif examples as practical corroboration.

## Beat 4 — Hardware and firmware can be co-configured
Sources: S1A-S11/S12.
Guard:
specific tools/vendors are examples only.

## Beat 5 — Component maturity
Claim: A6-C04.
Electrical function → package/assembly → source/lifecycle/alternate → substitution impact.
No universal AVL policy.

## Beat 6 — Design for programming/test early
Claim: A6-C05.
Do not duplicate EP08 production-test architecture; focus on avoiding engineer-only dependency before LVP.

## Beat 7 — Bench test evidence boundary
Claim: A6-C06.
No automatic EMC/safety/reliability/serial-production inference.

## Beat 8 — Workarounds as visible debt
Claim: A6-C07.
Bodge wires / jumpers / manual calibration / firmware flags / bench-only power.

## Beat 9 — Next build retires uncertainty
Claim: A6-C08.

## Beat 10 — DEV / LVP / SVP
DEV: visibility/learning.
LVP: controlled BOM/FW/config + repeatable programming/test.
SVP preview: released configuration + supplier/process/test/compliance evidence.

## Listener tool execution
Run Electronics Prototype Debt Scan on Sentinel Node:
dev board dependency / bodge / untracked FW / manual flashing / no test access / undefined identity / silent rework / unreviewed substitution.

## Misconceptions
- custom PCB means production intent;
- component datasheet compliance proves system compliance;
- firmware is separate from hardware configuration;
- production test can be invented after board freeze;
- final PASS erases rework history.

## Closing action
For the current electronics prototype, create one build identity record linking hardware, BOM, firmware, calibration and test result.

## Handoff
A5/A6 create serious prototype evidence.
A7 now asks what exact claim must be verified, under which conditions, and for which decision.
