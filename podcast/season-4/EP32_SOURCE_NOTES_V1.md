# EP32 Source Notes V1 — Process Capability, SPC and Knowing Whether Production Is Stable

status: SOURCE NOTES COMPLETE — READY FOR WAVE 02 PUBLICATION GATE
checked: 2026-09-19
script: EP32_SCRIPT_DRAFT_V1.md
script_review: EP32_SCRIPT_REVIEW_V1.md
source_lock: evidence/source-lock/SOURCE_LOCK_WAVE_02_QUALITY_SUPPLIER_REGISTER.md

## Source-use statement
EP32 uses NIST/SEMATECH as the generic technical authority for capability concepts and Cp/Cpk formulas. The 2026 AIAG/VDA SPC Manual is named only as current automotive method context.

## Primary sources actually used

### EP32-S01 — NIST Process Capability
URL: https://www.itl.nist.gov/div898/handbook/pmc/section1/pmc16.htm
Supports:
- capability compares stable/in-control process behavior with specification limits;
- Cp/Cpk definitions;
- model/distribution/sample considerations.

### EP32-S02 — NIST Assessing Process Capability
URL: https://www.itl.nist.gov/div898/handbook/ppc/section4/ppc46.htm
Supports:
- capability vs specification;
- Cp and Cpk formulas;
- Cpk response to off-centering.

### EP32-S03 — NIST measurement sources
EP24-S01/EP24-S03.
Use:
measurement adequacy prerequisite.

### EP32-S04 — AIAG/VDA SPC Manual current public status
Owner: AIAG + VDA
Release: Jul 2026
Public source:
https://www.aiag.org/about-aiag/newsroom/articles/2026/07/01/international-cooperation-for-higher-quality--vda-and-aiag-publish-joint-standard-for-statistical-process-control-in-the-automotive-industry
Use:
current automotive-method context only.

## Quantitative declaration

Illustrative Sentinel inputs:
- LSL 4.80 mm
- USL 5.20 mm
- s 0.04 mm

Formula:
Cp=(USL-LSL)/(6s)
Cpk=min[(USL-xbar)/(3s),(xbar-LSL)/(3s)]

Independent arithmetic check:
- xbar=5.00 → Cp=Cpk≈1.67
- xbar=5.10 → Cp≈1.67, Cpk≈0.83

These values are fictional teaching data, not measured production evidence or acceptance criteria.

## Claim-to-source map
- stable vs capable → EP32-S01/S02.
- specification vs process-behavior/control limits → NIST process-monitoring/capability family.
- Cp/Cpk → EP32-S01/S02.
- measurement adequacy first → EP32-S03.
- no universal Cpk threshold → applicability guardrail/V6.

## Internal synthesis
Stability-to-Capability Decision Chain, reaction-plan card and Sentinel time-sequence story are Hardware-to-Production synthesis.

## Publication re-check
1. verify AIAG/VDA SPC public status remains current if named in show notes;
2. ensure no late edit inserts a universal Cpk threshold;
3. ensure no proprietary control-chart signal rules are added;
4. preserve explicit illustrative-data label.

## Gate
Current generic script source blockers: NONE.

**EP32 SOURCE NOTES V1: COMPLETE**
