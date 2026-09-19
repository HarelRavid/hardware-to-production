# Wave 04 Claim Lock — EP41 / EP42 / EP43 / EP44 / EP45 / EP46

status: CLAIM-LEVEL EVIDENCE LOCK COMPLETE FOR CURRENT GENERIC SCRIPT SCOPE
checked: 2026-09-19
shared_register: ../SOURCE_LOCK_WAVE_04_AUTOMATION_SAFETY_OEE_REGISTER.md

## Status vocabulary

- VERIFIED OPEN SOURCE — directly supported by open authoritative/public source.
- VERIFIED PUBLIC SCOPE — current standard identity/scope verified from ISO/IEC public metadata; no protected clause detail used.
- VERIFIED + V6 SYNTHESIS — source supports premise; episode framework/wording remains ours.
- DEPENDENCY — source burden belongs to prior Wave 01/02/03 lock.
- STANDARD CLAUSE GATE — exact normative requirement/PL/SIL/guarding/design detail requires licensed current standard and applicability.
- LEGAL/JURISDICTION GATE — exact legal obligation requires jurisdiction-specific source.
- ILLUSTRATIVE ARITHMETIC VERIFIED — fictional teaching values independently checked.
- V6 LOCKED AS SYNTHESIS — internal framework/guidance.

# EP41 — When Not to Automate

## EP41-C01
Claim: automation should start from a defined manufacturing problem, not from the assumption that more automation equals greater maturity.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W4-S14/S15 + Wave 03 economics.

## EP41-C02
Claim: process/design instability, inadequate measurement, unknown constraint and high change frequency can weaken an automation business/technical case.
Lock: VERIFIED + V6 SYNTHESIS.
Dependencies: Wave 02/03 + W4-S15/S16.

## EP41-C03
Claim: robot repeatability does not by itself establish process capability.
Lock: VERIFIED OPEN SOURCE + DEPENDENCY.
Source: W4-S18 + Wave 02 measurement/capability.
Boundary: process capability includes product/process/measurement interactions.

## EP41-C04
Claim: fixture/poka-yoke/assisted/semi-automatic alternatives should be compared before dedicated/full automation where they can solve the dominant mechanism.
Lock: VERIFIED AS DECISION SYNTHESIS.
Sources: W4-S14 + Wave 03 economics.

## EP41-C05
Claim: automation can preserve or amplify an unresolved defect mechanism if the mechanism is not understood/controlled.
Lock: V6 LOCKED AS SYNTHESIS supported by Wave 02/03 system logic.
Do not present as universal empirical law.

## EP41-C06
Claim: readiness must include safety/recovery/maintenance ownership, not only nominal cycle feasibility.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W4-S12/S14/S15.

### EP41 gate
P0 generic blockers: 0.
Exact machinery-safety requirement language: STANDARD CLAUSE/LEGAL GATE.

---

# EP42 — Building the Business Case for Automation

## EP42-C01
Claim: automation economics should compare alternatives including manual, assisted/semi-automatic, full automation and staged/defer options.
Lock: DEPENDENCY — Wave 03 P2.05 + V6 synthesis.

## EP42-C02
Claim: labor savings alone are an incomplete automation business case.
Lock: VERIFIED + DEPENDENCY.
Sources: W4-S12/S14 + Wave 03 investment sources.

## EP42-C03
Claim: CapEx/NRE, integration, qualification, maintenance, downtime, yield, utilization, product change and lifecycle support can materially affect automation economics.
Lock: VERIFIED + DEPENDENCY.
Sources: W4-S12 + Wave 03 economics.

## EP42-C04
Claim: lowest steady-state unit cost does not automatically produce the highest investment value.
Lock: DEPENDENCY — Wave 03 verified NPV/payback/sensitivity logic.

## EP42-C05
Claim: staged CapEx can preserve option value where demand/product/process uncertainty is high.
Lock: V6 LOCKED AS SYNTHESIS.
No claim that staged investment always dominates.

## EP42-C06
Claim: no universal payback/hurdle/OEE/volume threshold determines automation approval.
Lock: SCRIPT GUARDRAIL.

### EP42 gate
P0 generic blockers: 0.
Real organization finance/tax/accounting rules: application specific.

---

# EP43 — Semi-Automation, Robotics and Machine Vision

## EP43-C01
Claim: automation should be decomposed by function—handling, locating, transformation, verification and decision—rather than framed only as manual vs fully automatic.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W4-S15/S16.

## EP43-C02
Claim: human judgement/adaptability may remain valuable where variability is not sufficiently modeled, while machines may add repeatability/precision for well-defined tasks.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W4-S15/S16.

## EP43-C03
Claim: robot/cobot component safety does not establish integrated application/cell safety.
Lock: VERIFIED PUBLIC SCOPE.
Sources: W4-S05/S06.

## EP43-C04
Claim: collaborative-operation safety is task/application dependent.
Lock: VERIFIED OPEN SOURCE.
Source: W4-S17.

## EP43-C05
Claim: robot repeatability and accuracy are distinct.
Lock: VERIFIED OPEN SOURCE.
Source: W4-S18.

## EP43-C06
Claim: machine-vision feasibility depends on sensing/lighting/pose/feature/reference-truth conditions, not algorithm choice alone.
Lock: V6 LOCKED AS SYNTHESIS; technical support from robotics/measurement sources.
Any formal vision acceptance statistics remain separate source gate.

## EP43-C07
Claim: feeding/fixturing/end-effector/integration/recovery can dominate robotic-cell practicality.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W4-S15/S16.

### EP43 gate
Generic script can proceed.
Exact robot/cell safety design requirements: STANDARD CLAUSE + LEGAL/JURISDICTION GATE.

---

# EP44 — Automated Inspection and End-of-Line Test

## EP44-C01
Claim: 100% automated test coverage does not imply zero false accept/escape risk.
Lock: DEPENDENCY — Wave 02 measurement-system logic + V6 synthesis.

## EP44-C02
Claim: automated test is a measurement/decision system including fixture, sensor, reference/calibration, software/limit version and unit/configuration identity.
Lock: DEPENDENCY — Wave 02 + Wave 01.

## EP44-C03
Claim: automated test configuration changes can invalidate historical comparability or release evidence where they affect the decision.
Lock: DEPENDENCY — Wave 01/02.

## EP44-C04
Claim: golden/reference units are not automatically calibration standards.
Lock: DEPENDENCY — Wave 02.

## EP44-C05
Claim: retest/rework logic should preserve initial failure history.
Lock: DEPENDENCY — Wave 01/02.

## EP44-C06
Claim: automated test drift should be monitored as part of sustaining release evidence.
Lock: VERIFIED + DEPENDENCY.
Support: W4-S18 + Wave 02 measurement system.

## EP44-C07
Claim: machine/test yield must be separated from product/process yield when test-system faults or false rejects are material.
Lock: V6 LOCKED AS SYNTHESIS.

### EP44 gate
P0 generic blockers: 0.
Guard bands/uncertainty ratios/GR&R thresholds/calibration intervals remain exact-source gated.

---

# EP45 — Automation Qualification, OEE and Maintenance

## EP45-C01
Claim: FAT/SAT/SIT are requirements/specification-based automation acceptance layers and do not automatically equal production-process qualification/release.
Lock: VERIFIED PUBLIC SCOPE + V6 SYNTHESIS.
Source: W4-S08.

## EP45-C02
Claim: automation release evidence should include representative product/process envelope, quality, accepted throughput, abnormal-state/recovery and maintainability evidence.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W4-S08/S12 + Wave 02/03.

## EP45-C03
Claim: OEE = Availability × Performance × Quality for the episode's equipment-centric analysis.
Lock: VERIFIED OPEN SOURCE.
Sources: W4-S11/S12.

## EP45-C04
Claim: OEE is a composite loss lens and not by itself root-cause analysis or system-capacity proof.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W4-S11/S12 + Wave 03 capacity.

## EP45-C05
Claim: equal OEE values can reflect different dominant loss mechanisms and require different engineering actions.
Lock: ILLUSTRATIVE ARITHMETIC VERIFIED + V6 SYNTHESIS.

## EP45-C06
Claim: maintenance/recovery data are part of sustaining automation readiness/economics.
Lock: VERIFIED.
Sources: W4-S12/S15.

## EP45-C07
Claim: safe restart/recovery should preserve or restore product state, configuration/genealogy and quality/release trust where relevant.
Lock: DEPENDENCY — Wave 01/02 + V6 automation application.

## EP45-C08
Claim: no universal "85% OEE is world class" threshold should be presented as engineering truth.
Lock: SCRIPT GUARDRAIL.

## EP45-C09
Claim: local OEE can improve without increasing system accepted throughput.
Lock: DEPENDENCY — Wave 03 constraint/capacity.

### EP45 arithmetic lock
Main example:
A=0.90; P≈0.93253968; Q≈0.95957447; OEE≈0.80535714 = 80.54%.

Equal-OEE:
Cell A = 80.3682%.
Cell B = 80.3682%.

Status: ILLUSTRATIVE ARITHMETIC VERIFIED.

---

# EP46 — Scaling Without Automating Defects

## EP46-C01
Claim: duplicating/accelerating a production system can multiply unresolved defects, rework and evidence weaknesses as well as output.
Lock: VERIFIED AS SYSTEM SYNTHESIS.
Dependencies: Wave 02/03 + W4 integration sources.

## EP46-C02
Claim: scale readiness should re-confirm configuration stability, measurement adequacy, process capability, accepted throughput and recovery/maintenance before replication.
Lock: DEPENDENCY + V6 synthesis.
Sources: Waves 01–03 + W4.

## EP46-C03
Claim: parallel/replicated cells should not be treated as equivalent without checking machine/fixture/software/calibration/material/operator/environment differences relevant to the claim.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W4-S16/S18 + Wave 01/02.

## EP46-C04
Claim: increasing automation on a nonconstraint may raise local utilization/output without improving system throughput.
Lock: DEPENDENCY — Wave 03.

## EP46-C05
Claim: scaling should be staged and re-measured because the system constraint can move.
Lock: DEPENDENCY — Wave 03 moving-constraint loop.

## EP46-C06
Claim: scale expansion should stop/reassess if evidence quality or control deteriorates.
Lock: V6 LOCKED AS SYNTHESIS.

### EP46 gate
P0 generic blockers: 0.
Exact machinery/legal/safety requirements inherit Wave 04 applicability gates.

---

# Safety/current-standard lock

Current publication/status metadata is locked for:
- ISO 12100:2010
- ISO 13849-1:2023
- ISO 13849-2:2012 + active revision
- IEC 62061:2021+A1:2024+A2:2026
- ISO 10218-1:2025
- ISO 10218-2:2025
- IEC 60204-1:2016+A1:2021
- IEC 62381:2024
- ISO 22400-2:2014+Amd1:2017 + active revision

These records support scope/current-status narration only unless exact licensed clause content is separately verified.

# Decision

WAVE 04 CLAIM LOCK: PASS FOR INTERNAL TECHNICAL REVIEW.

Current generic scripts do not require clause-level machinery-safety calculations or jurisdiction-specific legal claims to proceed.
