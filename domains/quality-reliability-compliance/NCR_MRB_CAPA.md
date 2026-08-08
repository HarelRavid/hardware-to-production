# 6.5 Nonconformance, MRB & CAPA

status: Researching
provenance: [GNR]

## Scope
Closed-loop control of nonconforming product/process states from detection through containment, disposition, root-cause investigation, corrective action and effectiveness verification.

## Core chain
Detection -> containment -> identification/traceability -> impact assessment -> disposition -> root cause -> corrective/preventive system action -> implementation -> effectiveness verification -> closure -> lessons learned.

## NCR objects
- affected product/lot/serial
- requirement/specification
- actual condition
- defect/nonconformance taxonomy
- detection point
- suspected creation point
- quantity/population at risk
- containment
- evidence/photos/data
- status/owner

## MRB disposition objects
- rework to specification
- repair boundary
- use-as-is/concession/deviation boundary
- return to supplier
- scrap
- additional inspection/sort
- engineering evaluation

## CAPA objects
- problem statement
- containment
- root cause
- escape/detection-system cause
- systemic cause boundary
- corrective action
- preventive/system action boundary
- owner/date
- implementation evidence
- effectiveness metric/window
- recurrence check

## Engineering principles
Disposition closes the product decision; it does not necessarily close the systemic problem.

Root cause should explain both why the defect was created and, where relevant, why existing controls failed to prevent or detect it before escape.

## Decision objects
### D-QRC-NCR-001 — Population at risk and containment scope
### D-QRC-MRB-001 — Disposition decision and engineering basis
### D-QRC-RCA-001 — Required depth of root-cause investigation
### D-QRC-CAPA-001 — Corrective action and effectiveness evidence

## Integrity rule
Do not close CAPA solely because an action was completed; verify that the targeted failure mechanism or recurrence signal actually changed.