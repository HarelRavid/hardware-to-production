# Episode 29 Production Blueprint — Capacity, Bottlenecks, Takt Time and Line Balance

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
lifecycle: Production Validation → Ramp

## Listener transformation
Before: estimates capacity from nominal cycle times or the fastest operator.
After: can reason about takt, constraints, accepted throughput, downtime, rework, parallel resources and moving bottlenecks at system level.

## Narrative hook
Every station individually appears fast enough, yet customer demand is missed. One calibration step queues work, rework steals technician time and material shortages idle downstream stations. Machine speed was never system capacity.

## Teaching flow
1. Demand and available production time.
2. Takt time versus cycle time.
3. Constraint/bottleneck identification.
4. Good-output capacity versus gross cycles.
5. Rework, downtime, changeover and availability losses.
6. Parallel stations and labor sharing.
7. Line balance and WIP as symptoms, not goals.
8. Moving constraint after improvement.
9. Capacity evidence before capital/automation investment.

## Core framework — Capacity Reality Sheet
`Demand → available time → takt → station cycle distributions → availability/changeover → FPY/rework load → effective good capacity → constraint → improvement option → new constraint → evidence`.

## DEV/LVP/SVP
DEV: rough estimates are enough for architecture decisions. LVP: measure actual cycles, interruptions and rework. Ramp: demonstrated accepted throughput and recovery behavior must support commercial demand.

## Common mistakes
- takt and cycle time treated as synonyms;
- fastest observed cycle used as capacity;
- improving a nonconstraint and expecting throughput gain;
- ignoring rework labor/equipment load;
- adding WIP to hide imbalance;
- buying automation before identifying the actual constraint.

## Quantitative gate
Takt, FPY/good-capacity, rework-load and constraint examples require independent arithmetic audit and explicit assumptions.

## Source/evidence backlog
Lean terminology should be sourced to authoritative references when attributed. Run-at-rate/customer capacity requirements remain applicability gated.

## Closing handoff
Episode 29 establishes internal production capacity. Episode 30 checks whether external suppliers and contract manufacturers can support the same ramp.
