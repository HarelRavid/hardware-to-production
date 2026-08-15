# Episode 10 Research Pack — Designing for Reliability, Service and Repair

status: RESEARCH PACK OPEN
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: reliability, mechanical, electronics, NPI, quality, service, operations
lifecycle: DEV → LVP → SVP
entry_point: DESIGNING FOR LIFECYCLE
technical_depth: practitioner

## 1. Episode promise
Help teams design beyond first-pass function by connecting failure mechanisms, usage/environment, serviceability, field evidence and repair strategy to product and production decisions.

Canonical listener question:
> The product works today — what must we design, test and record so it still works, can be diagnosed, and can be repaired or supported over its real life?

## 2. Navigation card
**You are here:** tolerance/variation → lifecycle reliability/service → manufacturing process selection.
**Best for:** teams moving from successful prototypes into repeated use, field trials, LVP or commercial support.
**Prerequisite:** Episode 9 helpful, not mandatory.
**You will leave with:** Reliability-Service Chain + Field Learning Loop + Repairability Review.
**Next:** Episode 11 Manufacturing Process Selection.

## 3. Core thesis
Reliability is not a final qualification test and serviceability is not a post-launch support problem. Both are architecture/design/process decisions influenced by loads, environment, variation, interfaces, materials, suppliers, assembly, diagnostics, access, configuration and field feedback.

A product can pass functional verification and still contain failure mechanisms that emerge only with time, cycles, environment, wear, contamination, misuse or accumulated variation.

## 4. Draft claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP10-C01 | Functional success at one time/configuration does not establish reliability over the intended life/environment. | P0 | BACKBONE-SUPPORTED |
| EP10-C02 | Reliability evidence should be linked to identified failure mechanisms, loads/environment/duty cycle and configuration. | P0 | BACKBONE-SUPPORTED |
| EP10-C03 | Design, manufacturing variation, suppliers and assembly/process conditions can all contribute to field reliability. | P0 | BACKBONE-SUPPORTED |
| EP10-C04 | Serviceability/repairability are product architecture considerations because access, replacement, calibration, diagnostics and configuration influence recovery cost/time. | P0 | BACKBONE-SUPPORTED |
| EP10-C05 | Field failures and returns should feed back into population segmentation, root cause, corrective configuration and effectiveness evidence. | P0 | FIELD EVIDENCE LOOP / BACKBONE-STABLE |
| EP10-C06 | Accelerated tests support only the failure mechanisms and acceleration assumptions they validly exercise; acceleration is not automatically equivalent to field life. | P0 | SOURCE VERIFICATION REQUIRED |
| EP10-C07 | A repaired/reworked unit retains failure and repair history; final PASS does not erase the event. | P0 | GLOBAL INVARIANT / STABLE |
| EP10-C08 | Repair strategy must consider economics, safety/compliance, spare availability, traceability and whether field action changes the released configuration. | P1 | BACKBONE/SYNTHESIS |

Publication guardrail: no universal life factor, acceleration model, MTBF target, confidence level or environmental test profile enters the script without exact technical/source applicability.

## 5. Reliability-Service Chain
Internal listener framework:
`Use case / mission → load/environment/duty cycle → failure mechanism → design/process/supplier contributors → detection/verification → life evidence → field signal → diagnosis → containment/repair → corrective change → revalidation → effectiveness check`.

## 6. Failure-mechanism review
For each important function ask:
1. What physically/electrically/chemically changes over time?
2. What loads, cycles, temperature, humidity, vibration, contamination or user actions accelerate it?
3. Which manufacturing variation or supplier attribute affects margin?
4. What early symptom could reveal degradation?
5. Can the failure be diagnosed without destructive teardown?
6. Is the affected module/part accessible and replaceable?
7. Does replacement require calibration/configuration pairing?
8. Which field data are needed to segment population and configuration?
9. What evidence would prove the corrective action effective?

## 7. Repairability Review
Capture:
`Failure/replaceable unit → access/disassembly path → special tools → hazardous energy/safety state → replacement part/configuration → firmware/calibration pairing → post-repair test → traceability → returned-part analysis → economic decision`.

The framework does not assume every product should be field-repairable. Sometimes sealed replacement is safer or more economical; the decision must be explicit.

## 8. Field Learning Loop
`Released population → field event/return → unit/configuration/lot identification → symptom/failure mode → containment → root cause → affected population → corrective design/process/supplier action → revalidation → field-effectiveness monitoring`.

This is the Season 2 introduction to the FIELD EVIDENCE LOOP; deeper QMS/CAPA treatment belongs later.

## 9. Worked example — Sentinel Node connector/environment failure
Initial functional and environmental tests pass on limited units. Later field returns cluster in one connector supplier lot after repeated temperature/humidity cycling.

Useful response is not merely “replace connector.” The team reconstructs affected HW/BOM/FW/lot/configuration, examines assembly variation and sealing interaction, confirms failure mechanism, contains affected population, qualifies the corrective configuration and monitors recurrence.

Service architecture matters too: if connector replacement requires destructive enclosure opening and recalibration, field cost and downtime may dominate the engineering decision.

## 10. DEV/LVP/SVP lens
**DEV:** expose likely failure mechanisms, instrument prototypes, preserve failure evidence and make service assumptions visible.
**LVP:** use repeated units/field trials to learn variation, maintain configuration/lot traceability, refine diagnostics and repair process.
**SVP:** maintain validated reliability/service evidence, field signal aggregation, controlled repair/change, spare/lifecycle strategy and effectiveness monitoring.

## 11. Standards/source boundary
Potential source families include product/industry-specific environmental and reliability standards, IEC/ISO/JEDEC/SAE/ASTM methods where applicable, manufacturer component qualification, and authoritative reliability engineering references.

No environmental profile, accelerated-life equation, sample size, confidence requirement or MTBF interpretation is universal. Exact methods belong behind Source Verification and applicability gates.

## 12. Boundary discipline
Episode 10 owns lifecycle reliability/service/repair thinking. Detailed reliability statistics, qualification planning, FRACAS/CAPA and environmental standards may be deeper later episodes/source packs. Episode 11 begins manufacturing-process selection and must not absorb reliability depth.

## 13. Applicability statement
General hardware reliability/service foundation. Required life, test methods, safety constraints, repair rights, retention and field-action obligations depend on product, industry, customer, jurisdiction and risk.

## 14. What this episode must NOT claim
- passing DVT/qualification proves lifetime reliability;
- MTBF equals product lifetime;
- accelerated testing always predicts field life;
- every product should be repairable in the field;
- component qualification proves assembled-system reliability;
- a repaired final PASS erases original failure;
- one returned unit proves a population-wide root cause.

## 15. Research backlog before CLAIM SET STABLE
1. Cross-check reliability/service domains in the canonical backbone.
2. Build authoritative source map for failure-mechanism and accelerated-test boundary claims.
3. Add one simple life/field-data example only after assumptions are explicitly defined and audited.
4. Preserve FIELD EVIDENCE LOOP mapping without duplicating later quality/CAPA content.
5. Technical review: reliability + design + manufacturing/NPI + service/quality.

## 16. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: HIGH when test methods are introduced
Quantitative burden: MEDIUM-HIGH in later evidence work
Backbone risk: LOW
Source verification: OPEN

Next status target: `RESEARCH PACK OPEN → CLAIM SET STABLE`
