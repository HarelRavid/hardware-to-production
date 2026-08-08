# 6.7 Traceability & Genealogy

status: Researching
provenance: [GNR]

## Scope
Maintain sufficient identity and relationship data to reconstruct what a product is, what went into it, what happened to it, which evidence applies and which population is affected by a discovered problem.

## Genealogy graph
Finished unit/serial -> subassemblies -> component/material lots -> suppliers -> revisions/effectivity -> routing operations -> machines/tools/fixtures -> operators/qualifications -> process parameters/recipes -> inspections/tests -> rework/deviations -> release/shipment.

## Traceability levels
- batch/lot
- serialized unit
- serialized critical component
- material heat/batch
- process load/batch
- software/firmware/configuration
- calibration/test reference boundary

## Engineering principle
Traceability should be designed from the decisions it must support: containment, root cause, recall, reliability analysis, compliance and configuration reconstruction. Capturing every possible datum without a decision purpose creates cost without necessarily creating usable genealogy.

## Questions
1. What population must be isolatable if a supplier lot is defective?
2. Can a finished serial be mapped to actual material/process/test history?
3. Can a process excursion identify every potentially affected unit?
4. Are rework and deviations preserved in genealogy?
5. Does software/configuration revision belong in the physical product genealogy?
6. Are split/merge operations and bulk materials represented correctly?

## Decision objects
### D-QRC-TRACE-001 — Required traceability granularity
### D-QRC-GEN-001 — Required genealogy relationships
### D-QRC-RET-001 — Retention/access requirements by evidence type
### D-QRC-CONTAIN-001 — Can the system identify the minimum defensible affected population?

## Integrity rule
Traceability is not merely a serial number printed on the product; it is the recoverable relationship graph behind that identity.