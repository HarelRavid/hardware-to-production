# 4.7 PFMEA, Control Plans & Quality Gates

status: Researching
provenance: [GNR]

## Scope
Translate product/process risk into executable manufacturing controls, detection/prevention mechanisms, reaction plans and release gates.

## Core chain
Process step -> function/requirement -> failure mode -> effect -> cause/mechanism -> existing prevention -> existing detection -> risk prioritization -> action -> control-plan characteristic -> method/frequency -> reaction plan -> evidence/record.

## PFMEA objects
- process step
- process function
- failure mode
- failure effect
- severity
- failure cause
- occurrence basis
- prevention control
- detection control
- detection basis
- action priority/risk method boundary
- recommended action
- owner/date/status
- residual risk

## Control-plan objects
- product/process characteristic
- CTQ/criticality classification
- specification/acceptance basis
- measurement/test method
- sample size/frequency
- equipment/gauge
- control method/SPC boundary
- reaction plan
- record
- responsible role

## Quality-gate objects
- gate location
- entry criteria
- required evidence
- release authority
- pass/fail/conditional disposition
- containment/escalation
- downstream lock

## Engineering principles
PFMEA is not a static spreadsheet produced for an audit. It should be a living risk model linked to the actual routing, process controls, defects and production evidence.

Inspection is not automatically prevention. A downstream test may detect a defect while leaving the upstream process unstable and expensive.

## Decision objects
### D-PSE-FMEA-001 — Which process risks require engineered prevention versus detection?
### D-PSE-CP-001 — Which characteristics belong in the Control Plan?
### D-PSE-GATE-001 — Where should quality gates exist in the routing?
### D-PSE-REACT-001 — What happens immediately when a control fails?

## Change triggers
- product/design revision
- routing/process change
- tooling/equipment change
- supplier/material change
- new defect/escape
- capability deterioration
- customer/field failure
- automation change

## Cross-links
PFMEA <-> routing
PFMEA <-> defect taxonomy
Control Plan <-> WI
Control Plan <-> MSA/SPC
Quality Gate <-> genealogy
Reaction plan <-> NCR/MRB/CAPA
PFMEA <-> lessons learned

## Integrity rule
Risk scores/priorities must not replace engineering judgment or applicable customer/industry methodology.