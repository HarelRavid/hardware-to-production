# EP45 Script Review V1 — Automation Qualification, OEE and Maintenance

status: PASS TO SOURCE NOTES
review_date: 2026-09-19
script_reviewed: EP45_SCRIPT_DRAFT_V1.md
source_lock: evidence/source-lock/wave-04/
reviewer_type: internal technical/editorial + quantitative/safety-boundary review; independent external human review not claimed

## Decision
The script is technically coherent, current-source aware, quantitatively correct and source-safe for generic automation qualification/OEE narration.

PASS TO SOURCE-NOTE PACKAGING.

## Source/current-status audit
- IEC 62381:2024 used only for public FAT/FIT/SAT/SIT scope — PASS.
- ISO 12100:2010 current published/revision active — scope map only.
- ISO 13849-1:2023 / ISO 13849-2:2012 current publication statuses represented correctly.
- IEC 62061 current consolidated family includes AMD2:2026.
- ISO 10218-1/-2:2025 current.
- IEC 60204-1:2016+A1:2021 current public family.
- ISO 22400-2:2014+Amd1:2017 remains published while revision active.

## Quantitative audit
Availability = 378/420 = 0.9000 — PASS.
Performance = (45×470)/22,680 = 0.93253968 — PASS.
Quality = 451/470 = 0.95957447 — PASS.
OEE = 0.80535714 ≈80.54% — PASS.

Cell A:
0.82×0.99×0.99 = 0.803682 — PASS.
Cell B:
0.99×0.99×0.82 = 0.803682 — PASS.

## Technical findings
- FAT/SAT vs production-release boundary: PASS.
- OEE formula/open NIST support: PASS.
- OEE loss-lens vs root cause/capacity: PASS.
- recovery qualification: PASS.
- maintenance/economics: PASS.
- safety applicability map: PASS.
- restart vs full recovery: PASS.

## Recording-lock guards
- no 85% benchmark;
- no local OEE=system capacity;
- no universal predictive-maintenance claim;
- no exact PL/SIL/safeguarding instruction;
- no statement that IEC 62381 is universally applicable to all automation systems.

**EP45 SCRIPT REVIEW V1: PASS TO SOURCE NOTES**
