# EP45 Script Outline V1 — Automation Qualification, OEE and Maintenance

status: SCRIPT OUTLINE COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
audience: automation / maintenance / manufacturing / quality / operations
lifecycle: Ramp → SVP
source_lock: Wave 04
technical_review: evidence/source-lock/wave-04/W4_INTERNAL_TECHNICAL_REVIEW.md

## Listener promise
Build a production-readiness pack for automated equipment that covers acceptance, representative operation, OEE loss decomposition, abnormal recovery, maintenance and controlled release.

## Cold open
[ILLUSTRATIVE] Machine hits quoted cycle at FAT. On site, sensor faults, jams, changeovers and cleaning cut accepted output. OEE falls, but the number does not say what to fix.

## Beat 1 — Acceptance layers
Claims: EP45-C01
Source: IEC 62381:2024 public scope.
FAT/FIT/SAT/SIT vs production-process release.

## Beat 2 — Release envelope
Claims: EP45-C02
Product/process/tooling/recipe/operators/material/conditions.

## Beat 3 — OEE formula
Claim EP45-C03
Sources: NIST W4-S11/S12.
A×P×Q; define boundaries.

## Beat 4 — Sentinel arithmetic
A=90%; P≈93.25%; Q≈95.96%; OEE≈80.54%.
Tags: [ILLUSTRATIVE] arithmetic verified.

## Beat 5 — Same OEE, different engineering problem
Claim EP45-C05.
Cell A reliability/recovery vs Cell B process/quality, both 80.3682%.

## Beat 6 — Loss tree and OEE boundary
Claims EP45-C04/C09.
OEE is not root cause or system capacity.

## Beat 7 — Fault/recovery qualification
Representative abnormal states; diagnosis, safe recovery, suspect product, restart, first-good-piece.

## Beat 8 — Maintenance/spares/config backup
Claim EP45-C06.
Predictive/preventive selected by mechanism/economics.

## Beat 9 — Safety applicability map
Public scope only: ISO 12100, ISO 13849/IEC 62061, ISO 10218, IEC 60204-1.
No PL/SIL design instruction.

## Beat 10 — Controlled release/change
Claim EP45-C07 + Wave 01.

## Listener tools
Automation Production-Readiness Pack + LOSS 8.

## Misconceptions
- FAT pass = production ready;
- OEE tells root cause;
- 85% OEE = universal world class;
- higher OEE = higher system throughput;
- predictive maintenance always best;
- restart = recovery.

## Closing action
Take last month's OEE and split the dominant 20% loss into named physical/recovery mechanisms before approving any improvement project.

## Handoff
EP46 asks whether this controlled automation is ready to be replicated and scaled.