# 3.15.3 Cumulative Variation, Yield & Inspection Placement

status: Researching
provenance: [GNR]

## Objects
- incoming variation
- process capability by operation
- datum-transfer error
- thermal distortion
- coating buildup
- assembly variation
- measurement uncertainty
- rework loop
- scrap point
- value-added accumulation
- escape risk
- inspection gate

## Engineering principle
Final variation is produced by the complete process chain. It is not generally valid to treat downstream capability as independent from incoming state or to combine unrelated capability indices without a model of the sequence.

## Questions
1. Which operation contributes most to final CTQ variation?
2. Where should an inspection gate be placed to detect failure before more value is added?
3. Which characteristic should be controlled upstream rather than sorted at final inspection?
4. Does rework reset the process state or create a new genealogy/qualification path?
5. Is the bottleneck actually process time, yield, inspection, rework, or furnace/batch occupancy?

## Decision objects
### D-INT-VAR-001 — Allocate tolerance/variation budget across the process chain
### D-INT-GATE-001 — Place inspection/control gates
### D-INT-YIELD-001 — Improve local process capability or redesign the chain?
### D-INT-RWK-001 — Define rework loop and release criteria

## Cross-links
Variation <-> GD&T
Variation <-> SPC/MSA
Inspection placement <-> cost of quality
Rework <-> genealogy
Yield <-> capacity/OEE

Quantitative stack/capability models require actual distributions, correlation assumptions and process data.