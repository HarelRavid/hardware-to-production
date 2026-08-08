# 8.10 Scaling Without Automating Defects & Section Quality Gate

status: Researching
provenance: [GNR]

## Scaling principle
Scale the validated value stream, not the current volume of waste. Before automating or duplicating a process, distinguish required work from instability, inspection caused by poor capability, rework loops, manual adjustment and hidden engineering support.

## Scale-readiness dimensions
- stable product configuration
- understood CTQs/failure mechanisms
- capable process
- capable measurement/test
- controlled inputs/materials
- robust tooling/fixtures
- repeatable Standard Work
- known cycle-time distribution
- yield/rework transparency
- maintenance/support model
- changeover/product-mix need
- supplier capacity
- digital/traceability readiness

## Scale strategies
- improve manual process
- standardize
- error-proof
- parallel manual cells
- semi-automate bottleneck
- automate inspection/test
- dedicated automation
- flexible robotic automation
- duplicate validated cell/line
- redesign product/process for scalable manufacture

## Decision object
### D-AUTO-SCALE-001 — What should be stabilized, eliminated, redesigned, semi-automated, automated or replicated?

## Anti-patterns
- automating rework
- automating inspection because upstream process is unstable
- copying a line before the bottleneck/failure modes are understood
- maximizing local machine utilization while starving/blocking system flow
- removing operators without preserving diagnostic/process knowledge
- locking an immature product into expensive dedicated automation

## Section 8 architecture coverage
- when not to automate: COMPLETE architecture
- automation business case: COMPLETE architecture
- semi-automation: COMPLETE architecture
- robotics/cobots: COMPLETE architecture
- machine vision: COMPLETE architecture
- automated inspection/test: COMPLETE architecture
- EOL systems: COMPLETE architecture
- automation qualification: COMPLETE architecture
- OEE/maintenance/spares: COMPLETE architecture
- scaling without automating defects: COMPLETE architecture

## Open population/evidence work
- automation ROI case studies
- robot/cobot safety and application standards
- machine-vision validation evidence
- automated inspection MSA examples
- software/automation validation methods
- OEE definitions/case studies
- maintenance/reliability literature
- spare-parts optimization methods
- brownfield versus greenfield scale case studies
- top questions/decisions/mistakes/myths/lessons
- GNR verification

## Integrity gates before Podcast Ready
1. Automation is justified against an improved non-automated baseline.
2. Process stability/capability is visible before scale decisions.
3. Automation does not hide rework or engineering intervention.
4. Automated inspection is treated as a measurement system.
5. Software/model/recipe revisions are controlled.
6. Qualification covers representative product and fault/recovery states.
7. OEE definitions/counting rules are explicit.
8. Maintenance/spares preserve the qualified state and system constraint.
9. Scale decisions consider product change/mix and flexibility.
10. GNR remains visible until verified.

## Status
Section 8 Architecture: COMPLETE
Knowledge population: OPEN
Evidence verification: OPEN
Podcast readiness: NOT READY

## Next section
Section 9 — Manufacturing Data Hub / Manufacturing Atlas reconciliation against MASTER_WBS.md.