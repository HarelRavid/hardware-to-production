# Season 3 S3-A Claim Lock — EP20 From EBOM to MBOM and Process Flow

status: CLAIM-LEVEL EVIDENCE LOCK COMPLETE
checked: 2026-09-19
shared_register: ../SOURCE_LOCK_SEASON_3_S3A_PRODUCTION_SYSTEM_REGISTER.md

## EP20-C01
Claim: a released engineering product definition is not by itself an executable manufacturing system.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S3A-S01/S02/S03/S05.

## EP20-C02
Claim: manufacturing execution requires explicit tasks/operations, sequence, resources and constraints.
Lock: VERIFIED.
Sources: S3A-S02/S03.

## EP20-C03
Claim: EBOM, MBOM and routing are useful implementation concepts, but exact taxonomy/data ownership varies by organization/system.
Lock: V6 SYNTHESIS + S3A-S04 guardrail.

## EP20-C04
Claim: manufacturing structure can include subassemblies, kits, consumables, programming/configuration and packaging inputs not always represented the same way in the engineering BOM.
Lock: V6 SYNTHESIS.

## EP20-C05
Claim: each operation should have defined input state, transformation/output state, resource/tooling and evidence/inspection needs where relevant.
Lock: V6 SYNTHESIS supported by S3A-S02/S03.

## EP20-C06
Claim: routing and manufacturing definition must remain linked to product revision/effectivity when changes affect execution.
Lock: DEPENDENCY — Wave01.

## EP20-C07
Claim: alternate/rework routes add history and should not silently overwrite the normal route.
Lock: DEPENDENCY — Wave01/global invariant.

## EP20-C08
Claim: a process-flow review before tooling/WI investment can expose sequence/resource/evidence gaps.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S3A-S01/S03.

## Decision
No universal EBOM/MBOM/routing schema is required.

EP20 CLAIM LOCK: PASS FOR TECHNICAL REVIEW.