# 5.6–5.7 Capacity, Bottlenecks, Takt & Line Balance

status: Researching
provenance: [GNR]

## Capacity objects
- demand rate
- available production time
- takt time
- cycle time distribution
- uptime/availability
- changeover
- yield/rework load
- staffing
- machine capacity
- labor capacity
- batch/furnace capacity
- inspection/test capacity
- supplier capacity

## Bottleneck objects
- constraint resource
- queue/WIP before constraint
- starvation
- blocking
- downtime
- changeover loss
- quality loss
- shared-resource contention
- maintenance/calibration downtime

## Engineering principle
The bottleneck is a system property and can move as demand, product mix, yield, downtime or process improvements change. The slowest nominal cycle-time operation is not automatically the true system constraint.

## Takt model
Takt is demand-driven available time per required good unit under a clearly defined demand/time basis. It is not the same as machine cycle time.

## Line-balance objects
- work element
- precedence
- manual time
- machine automatic time
- walking/handling
- station assignment
- operator count
- utilization
- buffer/WIP
- product mix

## Questions
1. Is capacity calculated on good output or gross starts?
2. Are rework and retest consuming hidden capacity?
3. Are shared inspection/test resources the real constraint?
4. Is a batch process/furnace creating a different capacity logic than one-piece flow?
5. Does balancing average cycle time hide variability that creates queues?
6. What happens under actual product mix rather than a single SKU?

## Decision objects
### D-RAMP-CAP-001 — Required demonstrated capacity
### D-RAMP-BN-001 — Identify and protect the current constraint
### D-RAMP-TAKT-001 — Define valid takt basis
### D-RAMP-BAL-001 — Rebalance, add resource, reduce work content, buffer or automate?

## Cross-links
Capacity <-> yield
Capacity <-> OEE
Takt <-> Standard Work
Bottleneck <-> maintenance
Line balance <-> ergonomics
Capacity <-> supplier readiness

No universal utilization target or buffer size is asserted.