# Wave 06C Internal Technical Review — EP13

status: PASS TO SCRIPT OUTLINE WITH METAL-STATE/PROCESS GUARDRAILS
review_date: 2026-09-19
reviewer_type: internal technical/editorial review; independent external human review not claimed

inputs:
- SOURCE_LOCK_WAVE_06C_METALS_REGISTER.md
- W6C_EP13_CLAIM_LOCK.md
- EP13 Production Blueprint
- machining/heat-treatment domain maps
- Wave 06A process selection
- Waves 01–03 capability/economics/change dependencies

## Decision

EP13 can advance to script outline with current generic source support and without process-specific numerical folklore.

## Technical findings

### Casting
PASS.
Solidification/porosity framing is technically sound.
Do not reduce all casting risk to “porosity”; segregation, inclusions, filling/solidification and geometry matter.

### Forging/forming
PASS.
Grain-flow/material-state coupling is appropriately scoped to industry guidance.
Do not imply forging always produces superior properties.

### Sheet forming
PASS.
Springback tied to material/strain path is strongly supported by NIST.
Do not give generic compensation values.

### Machining
PASS.
Machine positioning spec and finished-part process capability are correctly separated.

### Material state
PASS.
Alloy/state/temper/heat treatment remains part of route definition.
Do not teach generic heat-treatment recipes here.

### Residual stress/distortion
PASS.
Mechanism is valid.
Keep quantitative example out unless material/process specific.

### Near-net + machining
PASS as synthesis.
Do not imply near-net always reduces cost; compare scrap/tooling/secondary operations/inspection.

### NDT/inspection
PASS.
Keep method/acceptance application-specific.

## Required script guards

1. no generic casting porosity limit;
2. no generic forging strength advantage;
3. no generic bend radius/springback compensation;
4. no generic machining tolerance based on machine spec;
5. no generic heat-treatment state;
6. no “same alloy = same properties” shortcut;
7. no route chosen from geometry alone;
8. no volume threshold that automatically selects casting/forging;
9. no universal NDT requirement;
10. process sequence and post-process state remain visible.

## Boundary with EP18/EP19

EP13 owns route-family comparison and material-state awareness.
EP18 owns heat-treatment/surface/cleaning depth.
EP19 owns full process-chain sequencing/evidence invalidation.

Result: PASS.

**WAVE 06C INTERNAL TECHNICAL REVIEW: PASS**
