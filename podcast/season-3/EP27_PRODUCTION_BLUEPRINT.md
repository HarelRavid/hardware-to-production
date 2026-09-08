# Episode 27 Production Blueprint — What a Production Validation Build Must Prove

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
lifecycle: Production Validation → Ramp

## Listener transformation
Before: treats a validation build as a more controlled pilot.
After: understands production validation as a system-level evidence event tying product, process, supplier, tooling, measurement, documentation, traceability and rate claims to a bounded configuration.

## Narrative hook
The product passes all functional tests, but the validation build still requires engineering intervention, supplier substitutions and manual test workarounds. Product evidence is strong; production-system evidence is not.

## Teaching flow
1. Separate product verification from production-system validation.
2. Freeze/bound the configuration being evaluated.
3. Validate process route, tooling/equipment and standard work.
4. Validate supplier/material readiness.
5. Validate measurement/test and traceability.
6. Capture yield/rework/interventions and abnormal recovery.
7. Evaluate rate/capacity evidence at the scale actually exercised.
8. Define open-gap disposition before ramp.
9. Decision: repeat, constrained release, or proceed.

## Core framework — Production Validation Evidence Matrix
`Claim → configuration/process envelope → evidence generated → deviation/intervention → result → gap → consequence → closure owner → release decision`.

## DEV/LVP/SVP
DEV: evidence can be claim-specific and exploratory. LVP: validation must increasingly exercise production-intent elements together. Ramp: the integrated system, not isolated subsystems, must support the next commercial commitment.

## Common mistakes
- calling the build “PVT” as proof;
- validating product on one configuration and process on another;
- ignoring engineer intervention in yield/capability conclusions;
- assuming supplier samples equal source readiness;
- extrapolating rate from a short best-case run.

## Source/evidence backlog
Customer-specific PVT/PPAP/run-at-rate/qualification requirements remain exact-source and applicability controlled. No universal validation sample size or duration.

## Closing handoff
Episode 27 defines what the build must prove. Episode 28 shows how yield, rework and scrap reveal where the production system still depends on rescue.
