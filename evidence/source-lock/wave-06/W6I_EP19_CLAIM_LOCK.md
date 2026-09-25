# Wave 06I Claim Lock — EP19 Manufacturing Process Chains

status: CLAIM-LEVEL EVIDENCE LOCK COMPLETE
checked: 2026-09-25
shared_register: ../SOURCE_LOCK_WAVE_06I_PROCESS_CHAINS_REGISTER.md

# EP19 — Manufacturing Process Chains: The Sequence Is Part of the Design

## EP19-C01
Claim: a manufacturing route should be treated as a sequence of state transformations, not isolated operations.
Lock: V6 SYNTHESIS supported by Wave06A–06H.

## EP19-C02
Claim: output state from one operation becomes input state/constraint for the next.
Lock: V6 SYNTHESIS.

## EP19-C03
Claim: later operations can invalidate earlier dimensional/material/surface evidence when they alter dependencies.
Lock: DEPENDENCY — Wave01 + Wave06C/06H.

## EP19-C04
Claim: datum/reference strategy can migrate through sequence and should be reviewed at the stage that controls final function.
Lock: V6 SYNTHESIS + EP09/EP18 dependencies.

## EP19-C05
Claim: cleaning/surface/joining/thermal compatibility is sequence dependent.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Dependencies: Wave06D/06H.

## EP19-C06
Claim: rework loops add history and may create a new process/configuration state.
Lock: GLOBAL INVARIANT + Wave01/02.

## EP19-C07
Claim: inspection should be placed where evidence is actionable and remains valid for downstream state.
Lock: V6 SYNTHESIS + Wave02.

## EP19-C08
Claim: multiplying step yields is valid only as a model under explicit population/dependency assumptions.
Lock: V6 QUANTITATIVE GUARDRAIL.

## EP19-C09
Claim: chain economics should be evaluated per accepted final output, not isolated operation price.
Lock: DEPENDENCY — Wave03.

## EP19-C10
Claim: process-sequence changes can require effectivity/evidence reassessment.
Lock: DEPENDENCY — Wave01.

## EP19-C11
Claim: simplified DEV/LVP routes can be legitimate bridge chains when limits/expiration triggers are explicit.
Lock: DEPENDENCY — A4/Wave06A.

## EP19-C12
Claim: release evidence should reflect all state-changing operations relevant to the final product claim.
Lock: V6 SYNTHESIS.

## Decision
No new process-family standard or numeric threshold is required.

EP19 CLAIM LOCK: PASS FOR TECHNICAL REVIEW.
