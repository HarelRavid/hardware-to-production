# Season 1 S1-C Claim Lock — EP08 Design for Test, Calibration and Traceability

status: CLAIM-LEVEL EVIDENCE LOCK COMPLETE
checked: 2026-09-19
shared_register: ../SOURCE_LOCK_SEASON_1_S1C_DFX_TEST_TOL_RELIABILITY_REGISTER.md

## EP08-C01
Production testability is partly a product-design property because access/interfaces/states/observability are created by design.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: S1C-S10 + DFX backbone.

## EP08-C02
Engineering debug access can accelerate DEV while hiding dependencies unsuitable for repeated production test.
Lock: DEPENDENCY — A6.

## EP08-C03
Production test should protect a defined requirement/CTQ/failure-mode/release claim rather than exist by habit.
Lock: V6 SYNTHESIS + A7/Wave02.

## EP08-C04
Measurement adequacy precedes strong pass/fail/trend/capability conclusions.
Lock: VERIFIED.
Sources: S1C-S07/S08/S09.

## EP08-C05
Calibration values/procedure/version are part of configuration evidence when materially affecting product behavior/acceptance.
Lock: DEPENDENCY — A8/Wave01 + S1C-S08/S09.

## EP08-C06
Relevant identity should link build/configuration/programming/calibration/test/deviation/rework evidence.
Lock: DEPENDENCY — A8/Wave05 genealogy.

## EP08-C07
More testing does not automatically mean better quality; coverage should follow consequential claims/failure modes and consider false decisions/cycle/economic burden.
Lock: V6 SYNTHESIS.

## EP08-C08
Production-test architecture should evolve with rate/automation/traceability/measurement/recovery needs.
Lock: V6 SYNTHESIS + later-wave dependencies.

## IEEE boundary-scan guard
IEEE 1149.1-2013 is Inactive-Reserved; P1149.1 is an active revision project. If boundary scan appears in narration it is an architectural example, not cited as a current active final standard.

## Decision
No universal MSA threshold/calibration interval/test-coverage target is required.

EP08 CLAIM LOCK: PASS FOR TECHNICAL REVIEW.