# 1.4–1.6 Product vs Manufacturing Readiness, Production Intent & Exit Evidence

status: Researching
provenance: [GNR]

## Production-intent dimensions
A build may be production-intent in some dimensions and not others.

Track independently:
- design/configuration
- material specification
- supplier/site
- manufacturing process
- tooling/fixture
- equipment
- software/firmware
- inspection/test
- operator skill
- production environment
- rate/takt
- packaging/logistics

## Product-readiness dimensions
- requirements definition
- functional performance
- safety/risk controls
- environmental compatibility
- reliability/durability
- regulatory/compliance boundary
- configuration stability
- service/repair strategy

## Manufacturing-readiness dimensions
- MBOM/routing
- DFM/DFA closure
- tooling/equipment qualification
- process capability
- MSA/test readiness
- PFMEA/control plan
- operator qualification
- supplier readiness
- material availability
- yield/rework
- capacity/takt
- genealogy/traceability
- maintenance/spares

## Hardware Manufacturing Readiness Matrix
Each dimension should support states such as:
0 — undefined
1 — concept defined
2 — prototype method exists
3 — production-intent approach selected
4 — representative implementation demonstrated
5 — released/qualified for controlled production
6 — demonstrated stable at required production conditions

The numeric labels are an internal planning model, not a universal industry maturity standard.

## Engineering principle
Readiness is vector-valued, not one score. A strong average can hide one critical dimension that makes launch unsafe or economically unstable.

## Decision objects
### D-PDR-PI-001 — Which build dimensions are truly production-intent?
### D-PDR-MRM-001 — Manufacturing readiness by dimension
### D-PDR-EXIT-001 — What evidence is required to leave the current development state?

## Exit-evidence pattern
Objective -> required representative conditions -> evidence -> acceptance criterion -> owner/approver -> unresolved risk -> effectivity/configuration.

## Integrity rule
Do not average away a critical red readiness dimension.