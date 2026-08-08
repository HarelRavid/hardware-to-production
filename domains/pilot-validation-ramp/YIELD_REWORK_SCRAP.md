# 5.3–5.4 Yield, FPY/RTY, Rework & Scrap

status: Researching
provenance: [GNR]

## Yield objects
- operation input quantity
- first-pass good
- rework
- retest
- scrap
- concession/use-as-is boundary
- final good output
- defect opportunity boundary

## Metrics
### First Pass Yield (FPY)
Units passing a defined operation without rework/retest divided by units entering that operation, with counting rules explicitly defined.

### Rolled Throughput Yield (RTY)
Chain-level probability/measure of passing the defined sequence first-pass, derived from operation-level first-pass performance under a defined model.

### Final yield
Must be distinguished from FPY because rework can make final shipment yield look healthy while production capability remains poor.

## Rework objects
- defect
- rework instruction
- authorization
- additional operations
- retest/reinspection
- added labor/material
- effect on qualification/reliability
- genealogy

## Scrap objects
- quantity/value
- defect/cause
- operation of discovery
- operation of creation where known
- material/recovery value
- disposition

## Engineering principles
Final pass rate can hide factory instability. A unit that passes after repeated adjustment, rework or retest is not first-pass good.

The point of discovery and the point of defect creation are different objects and should both be captured where possible.

## Decision objects
### D-RAMP-YIELD-001 — Yield metric/counting architecture
### D-RAMP-RWK-001 — Is rework allowed, qualified and economically rational?
### D-RAMP-SCRAP-001 — Scrap versus repair/rework decision
### D-RAMP-PARETO-001 — Prioritize defects by frequency, cost, risk and downstream impact

## Cross-links
Yield <-> routing
Rework <-> genealogy
Scrap <-> cost
Defects <-> PFMEA/CAPA
RTY <-> process chain
Yield <-> ramp exit

No universal acceptable FPY/RTY target is asserted.