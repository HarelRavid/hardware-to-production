# 4.4 Work Instructions

status: Researching
provenance: [GNR]

## Scope
Controlled operator-facing execution information that translates routing/process requirements into an unambiguous, safe and repeatable manufacturing action.

## Work-instruction object
- WI ID
- revision/effectivity
- operation/routing link
- product/variant applicability
- prerequisite state
- required operator qualification
- tools/fixtures/equipment
- materials/consumables
- PPE/safety prerequisites
- setup
- ordered steps
- parameter/recipe reference
- visuals
- quality checks
- acceptance criteria
- required records
- reaction/escalation
- output state

## Design principles
- instruction at point of use
- one authoritative current revision
- separate requirement from explanation where useful
- visual communication for orientation/location/defect examples
- explicit critical parameters rather than tribal knowledge
- defined stop/escalation conditions
- variant/effectivity clarity
- usable with actual gloves, lighting, tools and takt constraints

## Key distinction
A Work Instruction defines how a specific operation is executed. Standard Work defines the best current repeatable work pattern and time/sequence relationship for the production system. They are linked but not identical objects.

## Questions
1. What can the operator reasonably infer, and what must be explicit?
2. Which steps are safety-, quality- or traceability-critical?
3. Which parameter values belong in the WI versus a controlled recipe/process specification?
4. How are product variants prevented from using the wrong instruction?
5. What happens when the real process cannot be completed exactly as written?
6. Is the WI validated at the workstation by representative users?

## Decision objects
### D-PSE-WI-001 — Required instruction depth
### D-PSE-VIS-001 — Which steps require visual standards/examples?
### D-PSE-REC-001 — Which execution evidence must be recorded?
### D-PSE-EXC-001 — Operator exception/escalation path

## Change control
Engineering/process change -> impact assessment -> routing/tooling/parameter/WI updates -> training impact -> effectivity -> release -> obsolete revision removal.

## Integrity rule
A signed training record does not prove that an unclear or incorrect Work Instruction is executable.