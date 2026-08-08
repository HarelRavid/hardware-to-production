# 5.10 Ramp Exit Criteria & Section Quality Gate

status: Researching
provenance: [GNR]

## Purpose
Define evidence-based exit from pilot/ramp states rather than declaring production readiness because a date, shipment target or unit count was reached.

## Exit-criterion dimensions
- design/configuration stability
- open engineering changes
- MBOM/routing/WI release
- tooling/equipment qualification
- operator qualification
- supplier readiness
- material availability
- measurement/test-system capability
- process capability/yield
- defect Pareto and critical escapes
- rework/scrap burden
- cycle time/takt
- demonstrated capacity
- reliability/validation evidence
- traceability/genealogy
- maintenance/spares/support readiness
- open deviations/risks

## Exit states
- PASS: evidence supports advancement
- CONDITIONAL PASS: defined residual risks/actions with ownership and controlled limits
- HOLD: evidence does not support advancement

## Engineering principle
Ramp exit is a multidimensional risk decision. No single KPI — yield, quantity shipped, cycle time or schedule — can prove production readiness by itself.

## Decision object
### D-RAMP-EXIT-001 — Advance, conditional advance or hold?
Output:
- decision
- evidence by readiness dimension
- unmet criteria
- residual risks
- temporary controls
- owners/dates
- revalidation/follow-up requirements

## Section 5 architecture coverage
- 5.1 Pilot-build planning: COMPLETE architecture
- 5.2 Production validation build: COMPLETE architecture
- 5.3 Yield / FPY / RTY: COMPLETE architecture
- 5.4 Rework and scrap: COMPLETE architecture
- 5.5 Learning curve: COMPLETE architecture
- 5.6 Capacity and bottlenecks: COMPLETE architecture
- 5.7 Takt and line balance: COMPLETE architecture
- 5.8 Supplier readiness: COMPLETE architecture
- 5.9 Engineering changes during ramp: COMPLETE architecture
- 5.10 Ramp exit criteria: COMPLETE architecture

## Open population/evidence work
- pilot/PVT methodologies across industries
- yield/RTY definitions and counting examples
- learning-curve literature and limits
- capacity/bottleneck models and case studies
- line-balancing methods
- supplier production-readiness evidence
- change/effectivity case studies
- production-readiness/ramp exit frameworks
- top questions/decisions/mistakes/myths/lessons
- GNR verification

## Integrity gates before Podcast Ready
1. Every build has explicit learning/validation objectives.
2. Production-intent and temporary conditions are distinguished.
3. Engineering intervention/rework/retest is visible in metrics.
4. FPY/RTY/final yield are not conflated.
5. Capacity uses good-output assumptions and includes losses/rework.
6. Takt is not confused with cycle time.
7. Supplier readiness includes demonstrated quality/capacity evidence.
8. Ramp changes have effectivity and revalidation logic.
9. Exit is evidence-based and multidimensional.
10. GNR remains visible until verified.

## Status
Section 5 Architecture: COMPLETE
Knowledge population: OPEN
Evidence verification: OPEN
Podcast readiness: NOT READY

## Next section
Section 6 — Quality, Reliability & Compliance, beginning with 6.1 Quality Planning and 6.2 Incoming/Process/Final Inspection, per MASTER_WBS.md.