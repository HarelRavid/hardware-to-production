# Season 1 S1-A Claim Lock — A6 Serious Electronics / Embedded Prototype

status: CLAIM-LEVEL EVIDENCE LOCK COMPLETE
checked: 2026-09-19
shared_register: ../SOURCE_LOCK_SEASON_1_S1A_OPENING_FOUNDATIONS_REGISTER.md

## A6-C01
Claim: electronics prototype maturity is multidimensional across function, margins, interfaces, firmware/configuration, components, assembly, testability and environment.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S1A-S06/S07.

## A6-C02
Claim: dev boards/lab equipment can accelerate learning while leaving product-specific power, timing/noise, thermal, EMC, programming and production-test dependencies unresolved.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S1A-S06/S07.
Guard: no claim every dev board hides every listed effect.

## A6-C03
Claim: hardware revision, BOM, firmware/configuration/calibration and test evidence need traceable linkage before repeated builds create ambiguity.
Lock: VERIFIED PREMISE + Wave 01.
Sources: S1A-S10/S11/S12.

## A6-C04
Claim: component selection eventually includes lifecycle/availability, package/assembly compatibility, alternate strategy and evidence-based substitution, not only electrical function.
Lock: V6 SYNTHESIS + supplier/change dependencies.
Guard: no universal AVL/lifecycle requirement.

## A6-C05
Claim: design-for-test/programming strategy should begin before repeated production becomes dependent on engineering-only debug access.
Lock: VERIFIED PREMISE + DFX source family.

## A6-C06
Claim: a passing bench test supports only the demonstrated configuration/test envelope, not automatically environmental/reliability/EMC/safety/serial-production performance.
Lock: VERIFIED.
Sources: S1A-S06/S07.

## A6-C07
Claim: bodge wires, jumpers, manual calibration, firmware workarounds and bench-only dependencies should remain visible development debt with owners/expiration conditions.
Lock: V6 SYNTHESIS.

## A6-C08
Claim: the next electronics build should retire consequential uncertainty rather than simply look cleaner.
Lock: V6 SYNTHESIS.

## Examples
- KiCad multi-file project: S1A-S10.
- Zephyr board-revision-aware build configuration: S1A-S11.
- Espressif hardware revision/software compatibility example: S1A-S12.

## Guardrails
No IPC/JEDEC/EMC/safety/compliance normative statement enters final narration unless separately source locked.

## Decision
Current conceptual-core P0 blockers: 0.

A6 CLAIM LOCK: PASS FOR TECHNICAL REVIEW.