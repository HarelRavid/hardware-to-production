# 2.7–2.8 Prototype Representativeness, Cross-Process Decisions & Section Quality Gate

status: Researching
provenance: [GNR]

## Prototype-to-production representativeness
Prototype evidence transfers only to the dimensions for which the prototype is representative.

## Representativeness vector
- geometry
- material
- manufacturing process
- surface/finish
- joining/assembly
- tooling
- supplier
- process variation
- inspection/test
- software/configuration
- environment/load
- production rate

### Example principle
A CNC-machined prototype of a future casting may validate geometry/function while providing little evidence about casting porosity, residual stress, draft, surface, tooling variation or production economics.

## Evidence-transfer decision
### D-DFX-REP-001 — Which conclusions from this prototype remain valid for the production-intent route?
Output:
- transferable evidence
- non-transferable evidence
- changed failure mechanisms
- required revalidation
- assumptions/open questions

## Cross-process design decision framework
Evaluate candidate design/process architectures on whole-system dimensions:
- function/performance
- material compatibility
- geometry
- tolerance/GD&T
- surface
- assembly/joining
- testability
- reliability/service
- volume/takt
- tooling/NRE
- process capability/yield
- supplier maturity
- automation potential
- traceability/quality
- cost per good part/lifecycle economics
- change flexibility

## Decision object
### D-DFX-CROSS-001 — Select design/process architecture across competing manufacturing chains

Do not optimize one process in isolation when another process, assembly, test or lifecycle step absorbs the cost/risk.

## Section 2 architecture coverage
- 2.1 DFM principles/process-driven design: COMPLETE architecture
- 2.2 DFA/mistake prevention: COMPLETE architecture
- 2.3 DFT/calibration/traceability by design: COMPLETE architecture
- 2.4 tolerances/GD&T/variation: COMPLETE architecture
- 2.5 material selection for manufacturing: COMPLETE architecture
- 2.6 reliability/service/repair: COMPLETE architecture
- 2.7 prototype-to-production representativeness: COMPLETE architecture
- 2.8 cross-process design decision framework: COMPLETE architecture

## Existing detailed knowledge retained by reference
Process-specific DFM rules remain in their process domains; Section 2 supplies the common framework and cross-process decision logic.

## Open population/evidence work
- Boothroyd-Dewhurst and other DFA/DFM methodology evidence/applicability
- tolerance-stack and GD&T references
- robust design/variation literature
- DFT/diagnostic design practices by product type
- serviceability/repairability case studies
- material/process selection methodologies
- prototype representativeness case studies
- quantitative cost-of-tolerance evidence
- top questions/decisions/mistakes/myths/lessons
- GNR verification

## Integrity gates before Podcast Ready
1. DFM is linked to actual candidate production processes.
2. DFA includes error opportunity and verification, not only part-count reduction.
3. DFT is designed before EOL/test-fixture lock-in.
4. Tolerances protect function and reflect process/measurement capability.
5. Material selection includes manufacturing/supply-chain consequences.
6. Reliability/service considerations feed architecture decisions early.
7. Prototype evidence states its representativeness limits.
8. Cross-process optimization uses whole-chain economics/risk.
9. Detailed process rules are referenced rather than duplicated.
10. GNR remains visible until verified.

## Status
Section 2 Architecture: COMPLETE
Knowledge population: OPEN
Evidence verification: OPEN
Podcast readiness: NOT READY

## Next section
Section 10 — Case Studies & Podcast Synthesis architecture, followed by whole-WBS architecture gap audit.