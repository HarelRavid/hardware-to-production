# Wave 03 Claim Lock — EP26 / EP27 / EP28 / EP29 / EP30 / EP31

status: CLAIM-LEVEL EVIDENCE LOCK COMPLETE FOR CURRENT GENERIC SCRIPT SCOPE
checked: 2026-09-19
shared_register: ../SOURCE_LOCK_WAVE_03_RAMP_ECONOMICS_REGISTER.md

## Status vocabulary

- VERIFIED OPEN SOURCE — directly supported by open authoritative/practitioner source.
- VERIFIED + V6 SYNTHESIS — external source supports the premise; episode wording/tool remains ours.
- DEPENDENCY — owned by an earlier source-lock wave.
- CUSTOMER/SECTOR GATE — exact obligation depends on applicable customer/contract/industry.
- ILLUSTRATIVE ARITHMETIC VERIFIED — fictional teaching values independently recalculated.
- V6 LOCKED AS SYNTHESIS — internal framework/guidance; not attributed to external authority.

# EP26 — How to Plan a Pilot Build

## EP26-C01
Claim: a pilot build should be planned around explicit learning/decision objectives rather than quantity alone.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W3-S02/S03.
Boundary: NASA PRR supports production-readiness evidence categories; our pilot framing is not a NASA-defined universal phase.

## EP26-C02
Claim: configuration/process/supplier/tooling/test/operator representativeness should be stated for the pilot claim.
Lock: VERIFIED + V6 SYNTHESIS.
Source: W3-S02.

## EP26-C03
Claim: pilot quantity should be justified by the learning/evidence need; no universal unit count applies.
Lock: V6 LOCKED AS SYNTHESIS + SCRIPT GUARDRAIL.

## EP26-C04
Claim: engineering intervention/rework during a pilot is valid learning evidence only if it remains visible rather than being erased from the result.
Lock: DEPENDENCY — Wave 01 configuration/history + Wave 02 quality/rework.

## EP26-C05
Claim: changes during a pilot require identity/effectivity so results are not mixed across configurations.
Lock: DEPENDENCY — Wave 01.

## EP26-C06
Claim: stop/containment criteria should exist for repeated consequential failures.
Lock: V6 LOCKED AS SYNTHESIS.
No universal stop threshold.

## EP26-C07
Claim: pilot exit should state unresolved gaps and the evidence actually generated.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W3-S02/S03.

### EP26 gate
P0 generic blockers: 0.
Exact customer/sector pilot/PVT sample requirements: CUSTOMER/SECTOR GATE.

---

# EP27 — What a Production Validation Build Must Prove

## EP27-C01
Claim: production validation is an integrated production-system evidence event, not merely a product functional test.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W3-S02/S03.

## EP27-C02
Claim: product/configuration, process, tooling, suppliers, measurement/test, documentation, operators and support conditions should be considered together for production-readiness evidence.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Source: W3-S02.

## EP27-C03
Claim: engineer intervention/workarounds during the build limit what the run proves about normal production capability.
Lock: V6 LOCKED AS SYNTHESIS.
Support: representativeness principle from W3-S02.

## EP27-C04
Claim: a short best-case rate demonstration is weaker evidence than representative accepted throughput over conditions relevant to the claim.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W3-S02/S06.

## EP27-C05
Claim: the release decision may be proceed, repeat, or constrained release depending on open evidence gaps.
Lock: V6 LOCKED AS SYNTHESIS.

## EP27-C06
Claim: naming a build PVT does not itself prove production readiness.
Lock: V6 LOCKED AS SYNTHESIS.
No universal PVT definition asserted.

### EP27 gate
P0 generic blockers: 0.
Exact PVT/customer validation requirements: CUSTOMER/SECTOR GATE.

---

# EP28 — Yield, Rework, Scrap and the Learning Curve

## EP28-C01
Claim: first-pass yield and final yield answer different production questions.
Lock: VERIFIED + V6 SYNTHESIS.
Support: Wave 02 rework/history + W3 flow/capacity sources.

## EP28-C02
Claim: a final PASS should not erase initial failure/rework history.
Lock: DEPENDENCY — Wave 01/Wave 02 global invariant.

## EP28-C03
Claim: rework consumes time/cost and can consume bottleneck capacity.
Lock: VERIFIED + ILLUSTRATIVE ARITHMETIC.
Sources: W3-S07/S08 + W3 capacity model.

## EP28-C04
Claim: defect recurrence/effectiveness matters more than simply closing each individual unit.
Lock: DEPENDENCY — quality/effectiveness invariant from Wave 02/backbone.

## EP28-C05
Claim: yield figures should be segmented by relevant product/configuration/process population rather than blindly blended.
Lock: V6 LOCKED AS SYNTHESIS + Wave 01 identity dependency.

## EP28-C06
Claim: there is no universal acceptable FPY/yield threshold.
Lock: SCRIPT GUARDRAIL.

## EP28-C07
Claim: a learning curve should be tied to actual changes in design/process/tooling/skill/control rather than assumed automatically.
Lock: V6 LOCKED AS SYNTHESIS.

### EP28 gate
Generic script can proceed.
Any empirical universal learning-rate claim would require separate evidence.

---

# EP29 — Capacity, Bottlenecks, Takt Time and Line Balance

## EP29-C01
Claim: takt time is available production time divided by required customer demand and is not the same as measured cycle time.
Lock: VERIFIED OPEN SOURCE.
Sources: W3-S04/S05.

## EP29-C02
Claim: nominal station cycle time alone does not establish sustainable system capacity.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W3-S06/S07.

## EP29-C03
Claim: accepted sustainable throughput is more decision-relevant than a short peak rate.
Lock: VERIFIED + V6 GLOBAL INVARIANT.
Sources: W3-S02/S06.

## EP29-C04
Claim: improving a nonconstraint can increase local output/WIP without materially increasing system throughput.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W3-S06/S07.

## EP29-C05
Claim: the constraint can move after an improvement.
Lock: V6 LOCKED AS SYNTHESIS with manufacturing-flow support.

## EP29-C06
Claim: yield/rework can reduce accepted capacity while nominal machine speed remains unchanged.
Lock: ILLUSTRATIVE ARITHMETIC VERIFIED + V6.
Source: W3 capacity model.

## EP29-C07
Claim: growing WIP/queues can be evidence that arrivals exceed sustainable departures under the demonstrated condition.
Lock: VERIFIED OPEN SOURCE + V6.
Sources: W3-S06/S07.

## EP29-C08
Claim: formal Run-at-Rate criteria are customer/industry specific.
Lock: CUSTOMER/SECTOR GATE.

## EP29-C09
Claim: capacity expansion should compare simpler flow/process/labor/parallelization alternatives with automation economically.
Lock: VERIFIED AS DECISION SYNTHESIS.
Sources: W3-S10/S11/S14.

### EP29 arithmetic lock
- takt 315 s/unit for 80 accepted units / 420 min.
- 360 s constraint → 70 theoretical cycles.
- 90% availability → 63 first-pass cycles.
- 92% FPY → 57.96 first-pass accepted.
- queue growth ≈2.43 units/h in the stated simplified scenario.
Status: ILLUSTRATIVE ARITHMETIC VERIFIED.

---

# EP30 — Supplier Readiness and Contract-Manufacturer Management

## EP30-C01
Claim: prototype sample quality is not equivalent to production-source readiness.
Lock: DEPENDENCY — Wave 02 EP39/40 + W3-S02.

## EP30-C02
Claim: supplier readiness includes source/site/process/tooling/measurement/capacity/quality/change/traceability evidence.
Lock: VERIFIED PREMISE + DEPENDENCY.
Sources: W3-S02 + Wave 02 supplier lock.

## EP30-C03
Claim: theoretical machine capacity is not supplier capacity unless staffing, material, yield, downtime, mix and flow assumptions are demonstrated.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W3-S06 + capacity model.

## EP30-C04
Claim: incoming inspection can be useful but does not automatically substitute for source-process capability.
Lock: DEPENDENCY — Wave 02.

## EP30-C05
Claim: CM relationships require explicit ownership of process, tooling, test, rework, quality data and engineering change.
Lock: V6 LOCKED AS SYNTHESIS.

## EP30-C06
Claim: exact supplier approval/change-notification obligations depend on customer/sector/contract.
Lock: CUSTOMER/SECTOR GATE.

### EP30 gate
Generic script can proceed by reusing Wave 02 source lock; no duplicated PPAP/FAI research required.

---

# EP31 — Engineering Changes During Ramp-Up

## EP31-C01
Claim: engineering change during ramp is a controlled transition across product, process, supplier, tooling, test, WIP/inventory and evidence populations.
Lock: DEPENDENCY — Wave 01 + V6 synthesis.

## EP31-C02
Claim: effectivity must identify which population receives the change; release date alone may be insufficient where WIP/inventory spans the date.
Lock: DEPENDENCY — Wave 01.

## EP31-C03
Claim: inventory/WIP disposition is part of the engineering change because mixed populations can invalidate evidence and traceability.
Lock: VERIFIED + V6 SYNTHESIS.
Support: Wave 01 + W3 production-envelope logic.

## EP31-C04
Claim: change/reverification scope should be based on affected evidence dependencies rather than automatic full retest or no retest.
Lock: DEPENDENCY — Wave 01 global invariant.

## EP31-C05
Claim: emergency deviation should remain bounded and should not silently become the permanent baseline.
Lock: DEPENDENCY — Wave 01.

## EP31-C06
Claim: post-cut-in monitoring/effectiveness evidence matters during ramp because a technically plausible change can move yield/capacity/quality.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W3 ramp evidence + Wave 02 effectiveness logic.

## EP31-C07
Claim: customer/regulatory notification requirements for changes are application specific.
Lock: CUSTOMER/SECTOR GATE.

### EP31 gate
P0 generic blockers: 0.
Detailed formal ECO/ECN workflow remains organization specific.

---

# P2.05 Economics dependency lock

## W3-E01
Claim: NPV, IRR and payback are recognized manufacturing investment-analysis methods.
Lock: VERIFIED OPEN SOURCE.
Sources: W3-S10/S11/S12.

## W3-E02
Claim: simple payback is not equivalent to NPV.
Lock: VERIFIED.
Sources: W3-S10/S11.

## W3-E03
Claim: uncertainty/sensitivity analysis can materially change investment decisions.
Lock: VERIFIED.
Sources: W3-S11/S12.

## W3-E04
Claim: maintenance/support/downtime belong in material equipment-investment economics.
Lock: VERIFIED.
Sources: W3-S13.

## W3-E05
Claim: no universal 10% discount rate or fixed payback threshold is justified by these sources.
Lock: SCRIPT GUARDRAIL.

## W3-E06
Claim: break-even is pairwise and depends on the stated cost boundary.
Lock: ILLUSTRATIVE ARITHMETIC VERIFIED + V6 synthesis.

## W3-E07
Claim: forecast volume is not production evidence.
Lock: V6 GLOBAL GUARDRAIL.

# Decision

WAVE 03 CLAIM LOCK: PASS FOR INTERNAL TECHNICAL REVIEW.

No current generic episode requires customer-specific Run-at-Rate rules or organization-specific finance criteria to proceed.
