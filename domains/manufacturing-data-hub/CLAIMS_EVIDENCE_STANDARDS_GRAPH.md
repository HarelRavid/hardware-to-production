# 9.8 Claims, Evidence & Standards Graph

status: Researching
provenance: [GNR]

## Purpose
Connect engineering knowledge to operational/manufacturing evidence while preserving the distinction between a Claim, a Source, a Standard requirement, an Observation and a Decision.

## Core objects
- Engineering Claim
- Source
- Standard / Regulation
- Clause / Requirement
- Applicability Statement
- Evidence Item
- Operational Observation
- Test/Measurement Result
- Case Study
- Assumption
- Knowledge Conflict
- Engineering Decision
- Decision Instance

## Core relationships
Claim --supportedBy--> Source/Evidence
Claim --boundedBy--> Applicability/Assumption
Claim --conflictsWith--> Claim/KnowledgeConflict
StandardRequirement --supports/mandates--> Claim/Control
Evidence --generatedBy--> Test/Inspection/OperationExecution
Evidence --appliesTo--> Product/Process/Material/Revision/Environment
DecisionInstance --uses--> Claim/Evidence/Assumption/Observation
DecisionInstance --produces--> SelectedOption/Action

## Evidence scope dimensions
- material/alloy/compound
- process family and specific process
- equipment/machine class or asset
- geometry/size/thickness
- temperature/pressure/environment
- production volume/rate
- test method
- revision/edition
- industry/application
- supplier/site

## Normative distinction
Standard requirement, informative guidance, supplier recommendation, academic evidence and internal operating data must retain their evidence class and authority. They are not interchangeable merely because they support the same conclusion.

## Operational evidence bridge
The Manufacturing Atlas may expose operational data to support or challenge a Claim, but raw correlation does not automatically become engineering causation. Promotion from observation to Claim requires review and explicit provenance.

## Revision principle
Standards and source documents require edition/revision/effective-date metadata. A Claim should retain which edition/source revision supported it when reviewed.

## Decision objects
### D-DH-EVID-001 — What evidence class and scope support this Claim?
### D-DH-NORM-001 — Is a cited requirement actually normative/applicable to this product/process?
### D-DH-OBS-001 — When can operational observations be promoted into reusable engineering knowledge?

## Integrity rule
Do not collapse citations into hyperlinks without structured applicability, evidence class and claim-level relationships.