# 4.6 Training & Operator Qualification

status: Researching
provenance: [GNR]

## Scope
Competence system that distinguishes awareness, training, supervised practice, demonstrated qualification and continued authorization for manufacturing operations.

## Competence objects
- role
- skill/operation
- prerequisite
- training module
- trainer/assessor
- supervised practice
- knowledge check
- practical demonstration
- qualification
- authorization
- expiry/requalification boundary
- restriction
- retraining trigger

## Competence states
Not trained -> trained/theory complete -> supervised -> demonstrated competent -> qualified/authorized -> suspended/expired -> requalified.

## Engineering principle
Attendance is not competence, and competence is not necessarily authorization. Critical/special processes may require demonstrated capability and controlled authorization beyond general training completion.

## Qualification dimensions
- correct setup
- correct tool/fixture use
- parameter/recipe selection
- execution sequence
- defect recognition
- measurement/inspection
- record/traceability completion
- reaction to abnormal conditions
- safety response

## Decision objects
### D-PSE-QUAL-001 — Which operations require formal qualification rather than training only?
### D-PSE-ASSESS-001 — Theory, practical demonstration, witnessed production, test piece or combination?
### D-PSE-REQUAL-001 — What triggers retraining/requalification?
### D-PSE-AUTH-001 — How is authorization enforced at point of use?

## Retraining/requalification triggers to evaluate
- long inactivity
- process/WI revision
- new equipment/tooling
- repeated defect/nonconformance
- failed audit/assessment
- safety event
- qualification expiry where applicable

## Matrix model
Person -> role -> operation/skill -> training revision -> qualification status -> restrictions -> assessor -> date -> expiry/review -> evidence.

## Cross-links
Training <-> WI revision
Qualification <-> special processes
Authorization <-> MES/access control boundary
Competence <-> quality escapes
Training <-> change control
Training <-> safety

## Integrity rule
A training matrix showing green cells does not by itself prove current production competence unless the qualification basis and evidence are defined.