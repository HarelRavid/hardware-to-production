# P2.04 — Pilot / PVT / Run-at-Rate / Capacity / Ramp Exit Criteria

**Status:** ACTIVE — QUANTITATIVE WORKED EXAMPLE STARTED

## Purpose
Turn pilot/PVT and ramp language into an evidence-based production-readiness decision model. The canonical worked example remains the fictional Sentinel Node.

## Core distinction
A successful batch is evidence that a batch was produced under those conditions. It is not, by itself, evidence of sustainable production capacity.

Production readiness must connect demand, takt, actual station cycle times, yield/rework, downtime, staffing, materials, controls, bottlenecks, WIP and sustained-rate evidence.

## External evidence backbone

### NASA Production Readiness Review
NASA PRR asks whether the developer is ready to efficiently produce the required number of systems. Entrance/success criteria include resolved production engineering problems/nonconformances, production documentation/plans, critical process controls/control limits/procedures, resources, BOM/critical parts, inspections/tests, costs/schedules and manufacturability.

Implication: production readiness is a system claim, not a statement that one product passed final test.

### Manufacturing readiness progression
Manufacturing-readiness frameworks distinguish pilot/low-rate/full-rate maturity and require increasing evidence that materials, manpower, tooling, test equipment, facilities, process capability, cost and planned production rate can be sustained.

### Yield/rework and capacity
NIST MEP case evidence demonstrates that rework/poor first-pass yield can consume substantial processing time and lead time; improving FPY can free effective capacity. This is used here as empirical support for treating rework as a capacity variable, not merely a quality KPI.

### Cycle time
Lean Enterprise Institute defines cycle time as actual measured time to produce a part or complete a process and distinguishes operator/machine/effective machine cycle time. This supports keeping takt, cycle time and total lead time separate.

## Sentinel Node production scenario

### Demand assumption
Customer/ramp requirement: 80 accepted units per 8-hour shift.

Nominal available shift time: 480 min.
Planned breaks/meetings/cleaning: 60 min.
Net planned production time: 420 min = 25,200 s.

Required takt based on net planned production time:

`takt = 25,200 / 80 = 315 s per accepted unit`

This is a demand-derived pacing target, not evidence that the line can achieve it.

## Initial station observations

| Station | Observed effective cycle time | Notes |
|---|---:|---|
| 10 PCB/firmware prep | 180 s | batch/programming dependencies excluded from naive stopwatch timing |
| 20 Mechanical assembly | 245 s | manual |
| 30 Connector installation | 275 s | includes seating verification |
| 40 Calibration + functional test | 360 s | current constraint candidate |
| 50 Seal/final inspection/pack | 210 s | manual |

A naive review says four stations are below takt and one is only 45 s above takt. The correct conclusion is not yet that capacity is nearly sufficient.

### Theoretical bottleneck capacity
If Station 40 is one serial resource at 360 s/unit:

`25,200 / 360 = 70 theoretical cycles/shift`

Even before losses and yield, this is below the requirement of 80 accepted units.

## Add real production losses
Pilot observation for Station 40:

- planned production time: 25,200 s
- unplanned tester downtime/restarts: 1,800 s
- effective running time: 23,400 s
- effective cycle time while running: 360 s
- theoretical completed test cycles during running time: 65

Assume 92% first-pass yield through calibration/final functional test:

`65 × 0.92 = 59.8 first-pass accepted units`

If 60% of failed units can be recovered during the same shift, and each rework consumes an average additional 300 s of constrained tester time, the rework loop must be modeled explicitly rather than credited as free recovery.

This demonstrates why accepted throughput cannot be inferred from nominal cycle time alone.

## Capacity vocabulary

### Takt
Demand-derived allowable production pace for the selected time basis.

### Cycle time
Observed time for a station/process/resource to complete its cycle.

### Throughput
Accepted output achieved per unit time under stated conditions.

### Capacity
Sustainable output potential under explicit assumptions about configuration, resources, availability, yield, changeovers, maintenance, staffing, material supply and product mix.

### Lead time
Elapsed time for product/work to traverse the relevant system boundary, including waiting/queues where applicable.

## Run-at-rate evidence model
A run-at-rate should record at minimum:

1. exact released product configuration and effectivity;
2. production route and equipment/tooling versions;
3. planned duration and time basis;
4. staffing and operator qualification;
5. product mix/batch assumptions;
6. raw-material and supplier state;
7. station cycle-time distributions, not only best observed cycles;
8. downtime by reason;
9. FPY, scrap and rework loops;
10. accepted throughput;
11. WIP/queue growth by station;
12. engineering intervention and workarounds;
13. maintenance/recovery events;
14. deviations/nonconformances;
15. resulting cost and schedule implications.

## Critical inference guardrail

**A short burst at target rate is not equivalent to sustainable capacity.**

A team may demonstrate 80 units/shift equivalent for 30 minutes by pre-staging material, skipping changeovers, using engineers, accumulating downstream WIP or postponing rework. That run may be useful evidence, but its applicability must be stated narrowly.

## Sentinel Node PVT intervention
Station 40 cannot meet required takt as configured. Candidate countermeasures are evaluated in order:

1. eliminate unnecessary calibration/test content only if requirements/evidence justify removal;
2. reduce handling/setup and software wait time;
3. improve test fixture/recovery robustness;
4. reduce upstream defects that create retest/rework load;
5. parallelize test resources if economics and measurement equivalence support it;
6. redesign product/test architecture only if needed.

The framework deliberately avoids jumping directly to 'buy another tester'.

## Ramp exit criteria — draft
A Sentinel Node ramp gate should not be passed merely because one target-rate shift succeeded. Candidate evidence categories:

- released/known configuration was built;
- critical production problems are closed or formally risk-accepted;
- CTQ measurement/control systems are adequate;
- required throughput demonstrated over a representative duration;
- bottleneck and queue behavior understood;
- FPY/rework/scrap are measured and compatible with the capacity/cost model;
- staffing and training are representative;
- maintenance/recovery can be performed without exceptional engineering support;
- supplier/material availability supports the planned rate;
- WIP does not grow without bound at the demonstrated schedule;
- cost assumptions are reconciled to observed production data;
- change-control/genealogy capture remains functional at rate.

These are a synthesized engineering decision framework, not a claim that NASA or another source mandates this exact checklist.

## Listener tool — RATE 8
Before saying 'we can make X per day', ask:

1. **Demand:** What accepted output is actually required?
2. **Time:** What net production time basis are we using?
3. **Constraint:** Which resource truly limits accepted flow?
4. **Availability:** What downtime/changeover/maintenance losses occur?
5. **Yield:** How much constrained capacity is consumed by failures and rework?
6. **Queues:** Is WIP stable or merely accumulating somewhere else?
7. **Representativeness:** Were normal people, tools, materials, configuration and controls used?
8. **Duration:** Was the evidence sustained long enough to expose realistic losses?

## Podcast myths to kill
- 'We made 10 units in an hour, therefore capacity is 80/shift.'
- 'Every station is under takt, therefore the line meets demand.'
- 'Rework does not affect capacity because the unit eventually passes.'
- 'Adding WIP increases capacity.'
- 'The bottleneck is always the station with the longest nominal cycle time.'
- 'A successful pilot batch proves ramp readiness.'
- 'Run-at-rate means running as fast as possible.'

## Provenance boundary
The quantitative Sentinel Node values, RATE 8, and proposed ramp-gate structure are worked-example synthesis. External sources support the underlying distinctions and readiness concepts; they do not prescribe these fictional numbers or this exact decision framework.

## Next depth tasks
- model rework recursion and effective accepted throughput quantitatively;
- add queue/WIP example showing hidden instability despite target output burst;
- build representative-duration run-at-rate scorecard;
- define PVT/ramp exit evidence by DEV/LVP/SVP stage;
- package P2.04 into a canonical listener tool.