# Season 4 S4-A — Quality / Reliability / Traceability / Compliance Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP33 / EP34 / EP35 / EP36
governed_by: podcast/season-4/SEASON_4_CLAUDE_HANDOFF_DELIVERY_BOARD.md
dependencies: Waves 01/02/05 + Season 1 EP10 + Season 3 quality/ramp

## 1. Purpose

Lock the authoritative/public evidence required to teach nonconformance/CAPA, reliability/field evidence, genealogy and standards applicability without turning one QMS, regulator or industry model into a universal hardware requirement.

## 2. Quality-management vocabulary / QMS source family

### S4A-S01 — ISO 9000:2026
Owner: ISO
Title: Quality management — Fundamentals and vocabulary
Edition: 5
Published: 2026-05
Official:
https://www.iso.org/standard/9000

Public support:
- current ISO quality-management fundamentals/vocabulary;
- common quality-management language across ISO 9000 family.

Use:
EP33/EP36 terminology context.

### S4A-S02 — ISO 9001:2026
Owner: ISO
Title: Quality management systems — Requirements
Edition: 6
Published: 2026-09-16
Official:
https://www.iso.org/standard/9001

Current-status finding:
ISO 9001:2026 is now the current edition and replaced ISO 9001:2015.

Public support:
- quality management system requirements;
- process performance/evaluation/improvement;
- customer/regulatory requirement context;
- current QMS framework.

Use:
EP33/EP36 context.

Guardrail:
ISO 9001 certification/requirements are not universal product-compliance requirements.

### S4A-S03 — ISO international standards vs law
Official:
https://www.iso.org/foreword-supplementary-information.html

Public support:
ISO standards are voluntary unless incorporated/referenced contractually or legally; law takes precedence.

Use:
EP36 core authority/applicability distinction.

### S4A-S04 — ISO 10007:2017
Owner: ISO
Title: Quality management — Guidelines for configuration management
Edition: 3
Official:
https://www.iso.org/standard/70400.html

Current status checked:
- current/published;
- confirmed 2023;
- revision project ISO/WD 10007 underway.

Public support:
configuration management spans planning, identification, change control, status accounting and audit from concept to disposal.

Use:
EP35/EP36.

## 3. Reliability / field-evidence source family

### S4A-S05 — NIST/SEMATECH Reliability Handbook Chapter 8
Official:
https://www.nist.gov/publications/nistsematech-engineering-statistics-handbook-chapter-8-reliability

Support:
ongoing assessment/control of reliability; reliability modelling/analysis techniques.

Use:
EP34.

### S4A-S06 — NIST accelerated-life / failure-mode sources
Reuse from Season 1 EP10:
- accelerated life test planning;
- failure-mode basis for acceleration models;
- limitations of few/no failures.

Use:
EP34.

Guardrail:
no universal acceleration equation, sample size, confidence target or MTBF threshold.

## 4. Genealogy / traceability source family

### S4A-S07 — NIST IR 8536 final
Owner: NIST
Title: Supply Chain Traceability: Manufacturing Meta-Framework
Final: 2026-09-09
Official:
https://csrc.nist.gov/pubs/ir/8536/final

Support:
- traceability as linked/provenance-aware records;
- temporal ordering;
- interoperable traceability across manufacturing ecosystems;
- no requirement for one centralized database.

Use:
EP35.

### S4A-S08 — NIST Digital Thread for Manufacturing
Official:
https://www.nist.gov/programs-projects/digital-thread-manufacturing

Support:
lifecycle-linked product/manufacturing/quality information and persistent identity.

Use:
EP35.

## 5. Scoped regulatory example — medical devices

### S4A-S09 — FDA Quality Management System Regulation (QMSR)
Owner: U.S. FDA
Official:
https://www.fda.gov/medical-devices/postmarket-requirements-devices/quality-management-system-regulation-qmsr

Current status:
effective 2026-02-02.

Public support:
FDA's medical-device QMS regulation now incorporates ISO 13485:2016 by reference and replaced the old QS regulation framework.

Use:
EP36 as a scoped example of a standard becoming embedded in regulatory requirements.

Guardrail:
medical-device U.S. requirements are not generalized to other products/jurisdictions.

## 6. Shared S4-A claims

### S4A-C01 — correction/containment, disposition, root-cause analysis, corrective action and effectiveness are distinct engineering/quality steps
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: ISO 9000/9001 current framework + frozen quality backbone.

### S4A-C02 — final PASS or rework completion does not erase the original nonconformance/failure history
Status: GLOBAL INVARIANT.

### S4A-C03 — affected-population reconstruction depends on identity/configuration/material/process/test/rework genealogy, not serial number alone
Status: VERIFIED + V6 SYNTHESIS.
Sources: S4A-S04/S07/S08.

### S4A-C04 — reliability evidence is bounded by population/configuration/use/environment/failure mechanism
Status: VERIFIED.
Sources: S4A-S05/S06 + EP10.

### S4A-C05 — field failures are evidence only after segmentation/context; anecdote ≠ population conclusion
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: NIST reliability + genealogy sources.

### S4A-C06 — standards, regulation, customer requirement, internal specification and guidance are different authority classes
Status: VERIFIED + V6 SYNTHESIS.
Sources: S4A-S03/S09.

### S4A-C07 — applicability must include source identity, edition/status, product/process/site/jurisdiction/contract scope and evidence owner
Status: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S4A-S03/S04/S09.

### S4A-C08 — certificate/certification to a management-system standard does not automatically establish product/process compliance for every claim
Status: VERIFIED PREMISE.
Sources: S4A-S02/S03.

### S4A-C09 — standard revision/supersession can require reassessment where the changed source affects an active requirement/evidence dependency
Status: V6 SYNTHESIS + change-control invariant.

### S4A-C10 — effectiveness evidence asks whether future relevant populations changed as intended, not merely whether an action was completed
Status: V6 QUALITY INVARIANT.

## 7. Hard guardrails

1. ISO 9001:2015 is obsolete/currently withdrawn; use ISO 9001:2026 for current generic references.
2. ISO 9000:2015 is obsolete; use ISO 9000:2026.
3. no universal MRB authority/disposition rule.
4. no CAPA requirement generalized from regulated sectors.
5. no universal root-cause method.
6. no universal reliability threshold/sample size/life factor.
7. no universal traceability granularity/retention period.
8. no claim serial number alone equals genealogy.
9. no standard = law shortcut.
10. no certification = universal product compliance shortcut.
11. no FDA/QMSR requirement generalized beyond U.S. medical-device scope.
12. no paid normative clause paraphrase beyond verified access.

## 8. Episode mapping

EP33:
S4A-S01/S02 + quality backbone.

EP34:
S4A-S05/S06 + EP10/Wave02.

EP35:
S4A-S04/S07/S08.

EP36:
S4A-S02/S03/S04/S09.

## 9. Current generic blockers

No intended EP33–36 script requires protected clause-level text or product-specific legal advice.

Current generic-script P0 blockers: 0.
