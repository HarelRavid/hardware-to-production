# Episode 10 Production Blueprint — Designing for Reliability, Service and Repair

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 1 — Build the Right Hardware Before Production Finds Your Mistakes

## Listener transformation
The listener learns to treat reliability, diagnostics, serviceability and repair evidence as product-architecture inputs before launch, and to turn field events into controlled engineering learning.

## Narrative hook
The product passes validation and ships. Months later a small cluster of field units fails intermittently. The team has return labels but poor configuration, exposure and repair history. They cannot tell whether the issue is supplier lot, environment, assembly, firmware or service intervention. The field is producing data, but not usable evidence.

## Teaching flow
1. Reliability versus one-time functional success.
2. Failure mechanisms, stresses, environment and duty cycle.
3. Architecture/component/interface/process contributors.
4. Diagnostics and service access as design decisions.
5. Repairability trade-offs: field repair, depot/factory repair, sealed replacement.
6. Configuration/calibration implications of service and replacement.
7. Field Evidence Loop: identity → configuration → exposure → failure → containment → root cause → corrective action → affected population → verification/effectiveness.
8. Sentinel connector/environment failure example.
9. Explain evidence limits of accelerated testing and final qualification.
10. Close the season by linking product design to lifetime feedback.

## Listener tools
**Reliability-Service Chain:** `Use/mission → Stress/environment → Failure mechanism → Design/process/supplier contributors → Detection → Life evidence → Field signal → Diagnosis → Containment/repair → Corrective change → Revalidation → Effectiveness`.

**Repairability Review:** access, hazardous state, replaceable unit, configuration/calibration pairing, post-repair test, traceability, returned-part analysis and economic decision.

## DEV/LVP/SVP/FIELD
DEV: expose likely mechanisms, instrument prototypes and make service assumptions visible. LVP: learn across repeated units/field trials and preserve configuration/lot evidence. SVP: control qualification, repair/change, spares and field signal aggregation. FIELD: convert failures into population evidence instead of anecdotes.

## Common mistakes
- Passing qualification interpreted as proof of all field reliability.
- MTBF treated as product lifetime.
- Component qualification treated as system qualification.
- Final PASS after repair erasing prior failure.
- One returned unit generalized to the whole population.
- Assuming every product should be field-repairable.

## Source/evidence backlog
Environmental profiles, accelerated-life equations, sample sizes, confidence targets, MTBF/Weibull claims and product-specific standards require exact method/source/applicability verification.

## Closing handoff
Season 1 ends with a product designed not only to function, but to be manufactured, assembled, tested, specified and supported as a population over time. Season 2 asks the next practical question: which manufacturing processes should actually create the parts and assemblies?
