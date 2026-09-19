# Season 1 S1-C — DFX / Test / Tolerance / Reliability Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP06 / EP07 / EP08 / EP09 / EP10
governed_by: podcast/season-1/SEASON_1_CLAUDE_HANDOFF_DELIVERY_BOARD.md
dependencies: DFX_SOURCE_MAP + Waves 01/02/03 + Season 1 A4–A8

## 1. Purpose

Lock the authoritative/public evidence required to close Season 1 technical design-for-production topics without importing unsourced DFM heuristics, obsolete GD&T/GPS editions, unverified test standards, or reliability folklore.

## 2. DFM / process-planning source family

### S1C-S01 — NIST Conceptual Process Planning
Source:
https://www.nist.gov/publications/conceptual-process-planning-definition-and-functional-decomposition

Support:
- manufacturability and manufacturing cost should be evaluated during early design;
- process planning and conceptual design should be integrated.

Use:
EP06.

### S1C-S02 — NIST Incorporating Process Planning into Conceptual Design
Source:
https://www.nist.gov/publications/incoporating-process-planning-conceptual-design

Support:
early design/process-planning integration and communication.

Use:
EP06.

### S1C-S03 — NIST Manufacturing Process and Material Selection During Conceptual Design
Source:
https://www.nist.gov/publications/manufacturing-process-and-material-selection-during-conceptual-design

Support:
- material/process choices are coupled;
- multiple attributes and uncertain early requirements matter.

Use:
EP06.

## 3. DFA / assembly-design source family

### S1C-S04 — NIST Comparative Assembly Planning During Assembly Design
Source:
https://www.nist.gov/publications/comparative-assembly-planning-during-assembly-design

Support:
- assembly sequence/constraints can be evaluated during design;
- DFA/assembly planning can feed design iteration.

Use:
EP07.

### S1C-S05 — NIST Representations and Methodologies for Assembly Modeling
Source:
https://www.nist.gov/publications/representations-and-methodologies-assembly-modeling

Support:
assembly design includes constraints among parts, relative motion, fit requirements and joint-strength considerations.

Use:
EP07.

### S1C-S06 — NIST Combining Interactive Exploration and Optimization for Assembly Design
Source:
https://www.nist.gov/publications/combining-interactive-exploration-and-optimization-assembly-design

Support:
assembly design involves constraints, design history/rationale and exploration of alternatives.

Use:
EP07.

Guardrail:
NIST assembly research supports assembly-as-design-variable. The podcast's Assembly Risk Walk / Mistake-Proofing Ladder are internal synthesis.

## 4. DFT / metrology / calibration source family

### S1C-S07 — NIST Measurement Process Characterization
Source:
https://www.nist.gov/publications/nistsematech-engineering-statistics-handbook-chapter-2-measurement-process

Support:
repeatability, reproducibility, stability, calibration and uncertainty are properties of measurement processes.

Use:
EP08 / EP09.

### S1C-S08 — NIST Traceability Considerations for Measuring Systems
Source:
https://www.nist.gov/publications/traceability-considerations-characterization-and-use-measuring-systems

Support:
calibration/verification/measurement-system characterization and operating/influence conditions affect later measurement results and traceability claims.

Use:
EP08 / EP09.

### S1C-S09 — NIST Policy / FAQ on Metrological Traceability
Sources:
https://www.nist.gov/calibrations/traceability
https://www.nist.gov/metrology/metrological-traceability

Support:
- metrological traceability is a property of a measurement result;
- merely having an instrument calibrated is not enough to guarantee a traceable/fit-for-purpose result;
- measurement process/system and uncertainty matter.

Use:
EP08.

### S1C-S10 — IEEE 1149.1 current-status watch
IEEE 1149.1-2013 page:
https://standards.ieee.org/ieee/1149.1/4484/
P1149.1 revision project:
https://standards.ieee.org/ieee/1149.1/10977/

Current status checked:
- IEEE 1149.1-2013 is Inactive-Reserved as of 2024-03-21.
- P1149.1 is an active revision project intended to supersede 1149.1-2013.
- no current active final 1149.1 standard was shown by IEEE SA at the checked date.

Public support:
boundary-scan architecture demonstrates that test access/observability/programming can be designed into electronics architecture.

Use:
EP08 as optional architectural example only.

Guardrail:
do not call 1149.1-2013 the current active IEEE standard in narration.

## 5. GD&T / GPS current-status source family

### S1C-S11 — ASME Y14.5-2018 (R2024)
Official:
https://www.asme.org/codes-standards/find-codes-standards/dimensioning-and-tolerancing

Current status:
- ASME Y14.5-2018 reaffirmed R2024;
- remains in effect;
- placed on stabilized maintenance.

Public support:
symbols/rules/definitions/defaults/practices for dimensioning and tolerancing/GD&T.

Use:
EP09 standard-system context only.

### S1C-S12 — ISO 8015:2011
Official:
https://www.iso.org/standard/55979.html

Current status:
Edition 2; reviewed/confirmed 2021; remains current.

Public support:
fundamental GPS concepts/principles/rules.

### S1C-S13 — ISO 1101:2017
Official:
https://www.iso.org/standard/66777.html

Current status:
Edition 4; reviewed/confirmed 2022; remains current.

Public support:
geometrical tolerancing language for form/orientation/location/run-out.

### S1C-S14 — ISO 5459:2024
Official:
https://www.iso.org/standard/87855.html

Current status:
Edition 3, published 2024-10.
Replaces ISO 5459:2011.

Public support:
datums and datum systems terminology/rules/methodology.

### S1C-S15 — ISO 2692:2021
Official:
https://www.iso.org/standard/74592.html

Current status:
Edition 4, published 2021.

Public support:
MMR/LMR/RPR for defined features of size and functional use cases.

Guardrail for S1C-S11–S15:
- EP09 does not teach clause-level normative rules from public metadata;
- ASME Y14.5 and ISO GPS are not treated as interchangeable rule systems;
- exact symbol/default/modifier teaching requires licensed/current standards text and explicit chosen system.

## 6. Reliability / accelerated-life source family

### S1C-S16 — NIST accelerated-life testing
Source:
https://itl.nist.gov/div898/handbook/apr/section3/apr314.htm

Support:
- accelerated-life tests use higher stresses to obtain failure data and fit/project models;
- stress levels must not create different failure mechanisms from intended use;
- planning depends on stresses, samples, durations, mechanisms and models.

Use:
EP10.

### S1C-S17 — NIST failure-mode basis for reliability models
Source:
https://itl.nist.gov/div898/handbook/apr/section2/apr211.htm

Support:
life distributions/physical acceleration models generally make sense at the individual failure-mode level; failure-mode identification/root cause matters.

Use:
EP10.

### S1C-S18 — NIST lack-of-failures / reliability evidence
Source:
https://itl.nist.gov/div898/handbook/apr/section1/apr132.htm

Support:
few/no failures can provide weak information for estimating population failure behavior; accelerated testing introduces model assumptions.

Use:
EP10.

### S1C-S19 — NIST acceleration models
Source:
https://itl.nist.gov/div898/handbook/apr/section1/apr15.htm

Support:
acceleration models relate stress to time-to-failure and are typically tied to physics/chemistry of a failure mechanism.

Use:
EP10.

## 7. Shared S1-C claims

### S1C-C01 — DFM belongs during design and is process/material specific
Status: VERIFIED.
Sources: S1C-S01/S02/S03.

### S1C-C02 — assembly sequence/fit/joint/access constraints can be design variables
Status: VERIFIED PREMISE.
Sources: S1C-S04/S05/S06.

### S1C-C03 — mistake prevention/source detection should be treated as engineering design options, not universal hierarchy
Status: V6 SYNTHESIS informed by DFA/quality backbone.

### S1C-C04 — testability is partly a product-architecture property
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S1C-S10 + Wave02 measurement/test architecture.

### S1C-C05 — calibration alone does not establish full measurement-system fitness
Status: VERIFIED.
Sources: S1C-S07/S08/S09.

### S1C-C06 — nominal geometry/tolerance language is standards-governed and measurement capability matters
Status: VERIFIED PREMISE.
Sources: S1C-S11–S15 + S1C-S07/S08.

### S1C-C07 — one prototype cannot establish production variation/capability
Status: DEPENDENCY — Wave02 / global invariant.

### S1C-C08 — worst-case and statistical tolerance analyses answer different questions and require explicit assumptions
Status: V6 ENGINEERING FOUNDATION.
No universal probability interpretation is attached without assumptions.

### S1C-C09 — reliability models/tests should be connected to identified failure mechanisms and use conditions
Status: VERIFIED.
Sources: S1C-S16/S17/S19.

### S1C-C10 — accelerated testing does not automatically equal field-life evidence
Status: VERIFIED.
Sources: S1C-S16/S18/S19.

### S1C-C11 — service/repair/field history belongs in product architecture and evidence loop when relevant
Status: V6 SYNTHESIS + frozen Field Evidence Loop.

## 8. EP09 illustrative quantitative lock

Illustrative stack A:
contributors ±0.20 mm, ±0.15 mm, ±0.10 mm.
Worst-case magnitude:
0.20 + 0.15 + 0.10 = 0.45 mm.
RSS magnitude under explicit independence/statistical assumptions:
sqrt(0.20² + 0.15² + 0.10²) ≈ 0.2693 mm.

Illustrative stack B:
contributors ±0.10 mm, ±0.05 mm, ±0.05 mm.
Worst-case magnitude:
0.20 mm.
RSS magnitude under explicit assumptions:
sqrt(0.10² + 0.05² + 0.05²) ≈ 0.1225 mm.

Status:
ILLUSTRATIVE ARITHMETIC VERIFIED.
Boundary:
RSS is not presented as a universal confidence limit or replacement for process-distribution evidence.

## 9. Hard guardrails

1. no universal DFM wall/draft/tolerance rule;
2. no universal DFA part-count objective;
3. no formal poka-yoke hierarchy attributed without source;
4. no torque/joint numeric rule in EP07;
5. no universal MSA/GR&R threshold, calibration interval or test-coverage percentage;
6. IEEE 1149.1-2013 is not described as current active standard;
7. no ASME/ISO clause/symbol/default interpretation from memory;
8. ISO 5459:2011 is obsolete; current edition is ISO 5459:2024;
9. ASME Y14.5 and ISO GPS are not blended into one rule set;
10. no universal capability threshold;
11. no universal reliability target/MTBF/confidence/life factor;
12. accelerated testing must preserve failure-mechanism/model applicability;
13. field repair/failure history is not erased by final PASS;
14. exact product/industry qualification profiles remain application-specific.

## 10. Current generic blockers

No intended conceptual script requires proprietary clause text if the outlines preserve these guards.

EP09 may name current standards and explain their role, but exact normative teaching stays in show notes/source-controlled material unless licensed text is supplied.

Current generic-script P0 blockers: 0.
