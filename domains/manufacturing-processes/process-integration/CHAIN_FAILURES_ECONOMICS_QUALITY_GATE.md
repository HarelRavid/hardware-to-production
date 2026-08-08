# 3.15.4 Cross-Process Failures, Economics & Quality Gate

status: Researching
provenance: [GNR]

## Cross-process failure objects
- upstream contamination causing downstream bond/coating failure
- heat treatment causing loss of machining tolerance
- machining introducing stress released later
- welding distorting machined features
- coating changing fit/grounding/sealing
- cleaning chemistry attacking substrate/coating/seal
- packaging recontaminating verified-clean surfaces
- supplier process change altering downstream capability
- inspection after irreversible value-add
- process order eliminating rework/inspection access

## Process-chain economics
Total cost per good part should include:
- all conversion steps
- intermediate transport/handling
- external supplier logistics
- queue/lead time
- WIP
- inspection gates
- yield loss at each operation
- rework loops
- scrap value after accumulated value-add
- tooling/fixtures
- batch/furnace occupancy
- cleaning/finishing
- qualification and traceability
- capacity constraints

## Master chain questions
1. Can an operation be eliminated by changing the upstream process or design?
2. Can two operations be consolidated without losing control/inspectability?
3. Is the chosen near-net process reducing machining enough to justify tooling and variation?
4. Are inspection gates placed before expensive irreversible steps?
5. Does the supplier boundary break genealogy or process control?
6. Is local cycle-time optimization increasing whole-chain WIP or yield loss?

## Decision objects
### D-INT-CONS-001 — Consolidate, reorder or eliminate operations?
### D-INT-MAKEBUY-001 — Where should supplier/process boundaries be located?
### D-INT-COST-001 — Optimize total process-chain cost per good part
### D-INT-RISK-001 — Which process interactions dominate product risk?

## Architecture coverage
- process-chain state model: COMPLETE
- sequence effects: COMPLETE architecture
- datum migration: COMPLETE architecture
- cumulative variation: COMPLETE architecture
- inspection-gate placement: COMPLETE architecture
- rework loops: COMPLETE architecture
- cross-process failure taxonomy: COMPLETE architecture
- chain economics/yield: COMPLETE architecture
- integrated decision objects: COMPLETE architecture

## Open population work
- quantitative case studies across major process chains
- correlated variation examples
- tolerance allocation methods and evidence
- sequence-dependent standards/customer requirements
- supplier-boundary case studies
- cost-of-quality and late-detection evidence
- cross-process failure case studies
- top questions/decisions/mistakes/myths/lessons
- GNR verification

## Integrity gates before Podcast Ready
1. Intermediate product state is explicitly represented between operations.
2. Datum transfer/recreation is defined for critical features.
3. Downstream thermal/surface operations are included in dimensional strategy.
4. Cleaning/contamination state is included where it affects later operations.
5. Inspection gates consider value added and detectability.
6. Rework creates an explicit controlled path, not an informal loop.
7. Whole-chain economics include yield, WIP, logistics and rework.
8. Supplier boundaries preserve required traceability and specifications.
9. Integrated decisions expose assumptions/open questions.
10. GNR remains visible until verified.

## Status
Architecture: CLOSED
Knowledge population: OPEN
Evidence verification: OPEN
Podcast readiness: NOT READY

## Milestone
Section 3 — Manufacturing Processes architecture is now complete through 3.15 according to MASTER_WBS.md.

## Next canonical section
4. Production System Engineering — begin with 4.1 EBOM -> MBOM and 4.2 Process Flow / Routing, per MASTER_WBS.md.