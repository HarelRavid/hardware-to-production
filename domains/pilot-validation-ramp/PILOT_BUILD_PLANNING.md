# 5.1 Pilot-Build Planning

status: Researching
provenance: [GNR]

## Purpose
A pilot build is a structured experiment on the product-production system interface. It should expose unknowns and validate readiness assumptions before scale hides them behind expedites, rework and heroics.

## Build-definition objects
- build objective/questions
- quantity
- product configuration/revision
- material/supplier lots
- tooling/equipment revision
- routing/WI revision
- operators/training state
- inspection/test readiness
- data collection plan
- deviations/non-production-intent conditions
- success/exit criteria

## Representativeness dimensions
- product design
- material
- supplier
- manufacturing process
- tooling/fixture
- equipment
- software/firmware
- operator skill
- inspection/test
- production environment
- rate/takt

## Build questions
1. What exactly must this build teach or prove?
2. Which conditions are production-intent and which are temporary?
3. Which defects/metrics must be captured at operation level rather than only at EOL?
4. What sample/quantity is sufficient for the claim being made?
5. Are engineering experts allowed to intervene, and if so is that intervention recorded?
6. Are rework, touch labor and troubleshooting time captured?
7. Can every unit be traced to its actual process/configuration state?

## Decision objects
### D-RAMP-PILOT-001 — Pilot objective and evidence plan
### D-RAMP-REP-001 — Production-intent representativeness assessment
### D-RAMP-QTY-001 — Build quantity based on learning/validation objective
### D-RAMP-DEV-001 — Which temporary deviations are allowed and how do they limit conclusions?

## Integrity rule
A pilot built by engineering experts with hand-selected parts and undocumented adjustments cannot be presented as evidence of normal production capability.