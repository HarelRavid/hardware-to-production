# EP45 Source Notes V1 — Automation Qualification, OEE and Maintenance

status: SOURCE NOTES COMPLETE — READY FOR WAVE 04 PUBLICATION GATE
checked: 2026-09-19
script: EP45_SCRIPT_DRAFT_V1.md
script_review: EP45_SCRIPT_REVIEW_V1.md
source_lock: evidence/source-lock/SOURCE_LOCK_WAVE_04_AUTOMATION_SAFETY_OEE_REGISTER.md

## Acceptance / qualification source
### IEC 62381:2024
Automation systems in the process industry — FAT, SAT and SIT
Edition 3, 2024-07-30.
https://webstore.iec.ch/en/publication/67572
Use:
public scope only; FAT/FIT/SAT/SIT demonstrate automation-system requirements against applicable specification.
Boundary:
not automatic manufacturing-process release.

## OEE sources
- NIST AMS 300-11:
  https://nvlpubs.nist.gov/nistpubs/ams/NIST.AMS.300-11.pdf
- NIST AMS 100-18:
  https://nvlpubs.nist.gov/nistpubs/ams/NIST.AMS.100-18.pdf
Use:
OEE = Availability × Performance × Quality and maintenance context.

## OEE arithmetic
Sentinel main example:
A=0.9000
P=0.93253968
Q=0.95957447
OEE=0.80535714 ≈80.54%

Equal-OEE:
Cell A=80.3682%
Cell B=80.3682%
All values illustrative and independently checked.

## Safety current-status map
- ISO 12100:2010 — current published; revision active.
- ISO 13849-1:2023 — current Part 1.
- ISO 13849-2:2012 — current Part 2; revision active.
- IEC 62061:2021+A1:2024+A2:2026 — current consolidated family.
- ISO 10218-1/-2:2025 — current robot/application standards.
- IEC 60204-1:2016+A1:2021 — current public family.

Use:
scope/current-status only. No protected clause content or legal obligation asserted.

## Claim map
- FAT/SAT vs production release → IEC 62381 scope + V6.
- OEE formula → NIST.
- OEE loss lens/not capacity/root cause → NIST + Wave 03.
- maintenance/recovery → NIST maintenance + V6.
- safety applicability → public standards scope only.

## Guardrails
No 85% benchmark.
No predictive-maintenance universal superiority.
No PL/SIL calculation or legal-compliance claim.
No restart=full recovery shortcut.

**EP45 SOURCE NOTES V1: COMPLETE**
