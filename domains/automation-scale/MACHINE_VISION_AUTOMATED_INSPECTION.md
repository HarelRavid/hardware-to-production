# 8.5–8.6 Machine Vision & Automated Inspection/Test

status: Researching
provenance: [GNR]

## Machine-vision objects
- camera
- lens
- field of view
- depth of field
- illumination
- polarization/filter boundary
- trigger
- fixture/presentation
- image preprocessing
- algorithm/model
- threshold/classification
- reference/golden sample boundary
- confidence/score
- false accept/false reject
- data retention

## Automated-inspection objects
- dimensional vision
- presence/absence
- orientation/assembly verification
- cosmetic/defect inspection
- OCR/barcode/data-matrix
- thermal/IR boundary
- automated electrical/functional test
- leak/pressure test
- force/torque/displacement test
- sensor calibration/test

## Engineering principle
A vision or automated-test system is a measurement/decision system and therefore requires validation against the defect/characteristic population it is expected to classify. High algorithm accuracy on a curated dataset does not prove production detection performance.

## Questions
1. Are defect classes and acceptance criteria objectively defined?
2. Does lighting/part presentation remain stable across production variation?
3. What are false-accept and false-reject consequences?
4. Are boundary/ambiguous examples represented in validation?
5. How are software/model/threshold revisions controlled?
6. Is the system measuring the actual CTQ or merely a correlated visual proxy?
7. What happens when the automated decision and human review disagree?

## Decision objects
### D-AUTO-VIS-001 — Is machine vision appropriate for the characteristic?
### D-AUTO-VAL-001 — Validation dataset and acceptance evidence
### D-AUTO-LIMIT-001 — Decision threshold / guard-band strategy
### D-AUTO-HUMAN-001 — Human review/escalation architecture
### D-AUTO-DATA-001 — Image/raw-data retention strategy

## Cross-links
Vision <-> MSA
Vision <-> defect taxonomy
Automated test <-> production test/calibration
Vision <-> traceability
Vision <-> AI/model governance boundary

No universal model accuracy or false-accept threshold is asserted.