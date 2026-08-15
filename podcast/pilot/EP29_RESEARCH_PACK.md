# Episode 29 Research Pack — Capacity, Bottlenecks, Takt Time and Line Balance

status: RESEARCH PACK OPEN
season: Season 3 — Build the Production System
primary_audience: Audience B — NPI / manufacturing / operations teams
secondary_audience: founders, process engineers, automation engineers, finance/ops leads
lifecycle: LVP-FIRST / CROSS-STAGE
entry_point: INDEPENDENT PRACTITIONER ENTRY WITH SHORT RECAP
technical_depth: practitioner-quantitative
backbone_anchor: P2.04 Capacity / Ramp + P2.05 Economics + P2.07 OEE

## 1. Episode promise
Teach a listener to distinguish required pace, theoretical machine speed and sustainable accepted system throughput — then identify the true constraint before adding people, equipment or automation.

Canonical listener question:
> We need more output. What exactly is limiting us, and how much capacity do we really have after downtime, yield, rework and flow losses?

## 2. Navigation card
**You are here:** Controlled LVP → production validation → ramp.

**Best for:** a team building tens/hundreds and starting to miss output, add shifts, debate automation, or discover WIP queues.

**You should already know:** basic process flow. No prior statistics episode required; equations are introduced from first principles.

**You will leave with:** Capacity Reality Sheet + Constraint Hunt + RATE 8 mini-check.

**Prototype shortcut:** rough stopwatch cycle-time measurements and engineering estimates can guide early LVP decisions.

**Shortcut expires when:** hiring, equipment purchase, customer delivery, line design or release/ramp decisions depend on the estimate.

**Next:** Episode 28 Yield/Rework → Episode 42 Automation Business Case → later OEE/loss/recovery episodes.

## 3. Audience contract
### DEV takeaway
Do not optimize rate before the product/process route is stable enough that cycle-time data mean something.

### Prototype shortcut
A few manual time studies are sufficient for rough learning if assumptions are visible.

### Shortcut expiration
When output commitments or CapEx depend on the result, measure distributions, availability, yield/rework and actual operating conditions.

### LVP change
Model the entire accepted-flow path, including bottleneck, labor, queue, inspection, rework and downtime.

### SVP evidence
Capacity claims require representative sustained runs, production-intent staffing/equipment/material, measured losses and acceptable quality.

### Manufacturing-debt prevention
Avoid buying automation to solve a local speed problem before proving that station is the system constraint.

## 4. Core distinctions

### Demand rate
Required good units over available production time.

### Takt time
A planning pace:
`available production time / required good units`

Guardrail: takt is demand-derived, not the measured cycle time of a station.

### Cycle time
Elapsed time needed by a process/station/unit operation under defined conditions. Use distributions, not only one best observed value, once the decision becomes consequential.

### Theoretical capacity
Maximum output implied by ideal cycle time and scheduled time, before real losses.

### Effective capacity
Output after relevant availability/performance/quality/rework/flow constraints.

### Accepted throughput
Good released units per time interval. This is the primary system output lens.

### Bottleneck / constraint
The resource or condition currently limiting accepted system throughput. It can move after an improvement.

## 5. Core claim register — draft
| ID | Claim | Class | Priority | Status | Note |
|---|---|---|---|---|---|
| EP29-C01 | Takt time is demand-derived available production time per required good unit; it should not be confused with measured station cycle time. | V2/V6 | P0 | OPEN | Source needed; equation/arithmetic straightforward. |
| EP29-C02 | System capacity is not equal to the fastest or slowest isolated nominal machine rate without considering flow, availability, quality, rework and dependencies. | V6 + P2.04 | P0 | BACKBONE-STABLE | Quantitative examples required. |
| EP29-C03 | Accepted sustainable throughput is a more decision-relevant output than short peak machine speed. | V6 + Global Invariant | P0 | BACKBONE-STABLE | Core backbone invariant. |
| EP29-C04 | Improving a non-constraint resource may increase local utilization/WIP without materially improving system throughput. | V5/V6 | P0 | OPEN | Source enrichment from Theory of Constraints/operations literature useful. |
| EP29-C05 | The system constraint can move after an improvement, so capacity must be re-measured/re-modeled. | V6 + MOVING CONSTRAINT LOOP | P0 | BACKBONE-STABLE | Stress-test repair. |
| EP29-C06 | Yield and rework can materially reduce good-unit capacity even when gross station cycle time is unchanged. | V3/V6 | P0 | BACKBONE-STABLE | Show math. |
| EP29-C07 | OEE can help decompose equipment losses but does not prove root cause or system capacity. | V2/V6 + P2.07 | P0 | BACKBONE-STABLE | Cross-link automation/OEE. |
| EP29-C08 | Run-at-rate or capacity evidence should be representative of intended production conditions for the claim being made. | V2/V6 | P0 | OPEN | Source terminology/applicability verification required. |
| EP29-C09 | Capacity expansion decisions should compare simpler flow/process improvements, labor/shift changes, parallelization and automation economically rather than default to equipment purchase. | V6 + P2.05/P2.07 | P1 | BACKBONE-STABLE | Decision synthesis. |

## 6. Listener tool — Capacity Reality Sheet

Record for each major operation:

| Field | Meaning |
|---|---|
| Demand good units/shift | Customer/plan requirement |
| Available minutes/shift | Net scheduled production time assumption |
| Takt | available time / demanded good units |
| Cycle-time distribution | not only best cycle |
| Staffing | operators/resources required |
| Planned downtime | breaks/changeovers/maintenance where modeled |
| Unplanned downtime | measured or assumption |
| FPY | first-pass good fraction |
| Rework rate | fraction requiring another loop |
| Scrap | lost units |
| Queue/WIP | observable flow symptom |
| Effective good rate | measured/modelled accepted output |
| Evidence class | measured / demonstrated / assumed |

## 7. Constraint Hunt — listener tool

1. Map process flow from released input to accepted unit.
2. Put demand/takt at the top.
3. Measure cycle-time distributions at major steps.
4. Add downtime/changeover/staffing constraints.
5. Add FPY, scrap and rework loops.
6. Observe where WIP/queues accumulate.
7. Compare effective good rate, not nominal equipment rate.
8. Identify the current system constraint.
9. Improve or protect that constraint.
10. Re-measure because the constraint may move.

## 8. Worked example A — basic takt
Illustrative assumptions:
- required output: 240 accepted units/8-hour shift;
- gross shift: 480 min;
- planned non-production time: 60 min;
- available production time: 420 min.

Takt:
`420 / 240 = 1.75 min/good unit = 105 s/good unit`

If a critical station has a sustained good-output interval of 130 s/unit, it cannot support demand without another change in flow/capacity.

If its best demonstrated cycle is 80 s but recurring recovery/downtime/rework makes accepted output 130 s/unit, the 80 s number is not the capacity claim we need.

All numbers are pedagogical.

## 9. Worked example B — yield changes good capacity
Station nominal process rate:
- 360 units/hour gross output.

Scenario 1:
- FPY = 98%;
- assume no capacity-consuming rework loop for the simplified first calculation.

First-pass good output:
`360 × 0.98 = 352.8 good units/hour`

Scenario 2:
- FPY = 90%.

First-pass good output:
`360 × 0.90 = 324 good units/hour`

Nominal machine speed did not change, but first-pass good capacity fell by 28.8 units/hour.

If failed units consume rework capacity, the system penalty is larger and must be modeled as a loop rather than just multiplying by yield.

## 10. Worked example C — rework recursion
Illustrative simplified loop:
- 100 units enter;
- 90% pass first time;
- 10% require one rework attempt;
- rework consumes 60% of the original station time per unit;
- 80% of reworked units pass.

Accepted units after one rework opportunity:
`90 + (10 × 0.80) = 98`

But process workload is not 100 unit-equivalents:
`100 + (10 × 0.60) = 106 unit-equivalents of station time`

Therefore accepted output per unit of constrained resource is lower than an FPY-only view suggests.

The episode should later show the generalized recurrence only if it improves understanding; do not bury the listener in math.

## 11. Worked example D — local improvement does not move system output
Three serial operations, simplified effective capacities:
- A = 100 good units/hour;
- B = 70 good units/hour;
- C = 90 good units/hour.

System ceiling is approximately constrained by B at 70 good units/hour, absent other flow effects.

Improving C from 90 → 120 does not make the serial system a 100/120-unit-per-hour line; B still constrains near 70.

Improving B from 70 → 95 may cause C or A to become the next constraint. Re-run the Constraint Hunt.

## 12. Sentinel Node example
Illustrative LVP route:
1. PCB programming;
2. connector insertion;
3. enclosure assembly;
4. calibration;
5. final functional test.

Observed symptom: WIP piles before calibration, while insertion station utilization looks high and management proposes automating connector insertion.

Capacity review shows:
- insertion has short cycle time but frequent small waits;
- calibration has longer effective good-unit interval and limited fixture channels;
- final test has acceptable average rate but significant re-test burden.

Decision:
do not buy insertion automation solely from local utilization. First protect/expand calibration constraint, reduce retest causes, then re-measure. If the constraint moves to insertion, automation can be reconsidered with current evidence.

## 13. OEE boundary
If equipment OEE is used:
`OEE = Availability × Performance × Quality`

Use it to decompose losses for the equipment/workcell whose definitions are controlled.

Do not infer:
- root cause from OEE alone;
- system throughput from one machine OEE;
- economic justification for automation from a higher OEE target alone.

## 14. Capacity evidence ladder

### Estimate
Engineering estimate based on assumed cycle time/staffing/yield.

### Measured short-run
Observed under limited production-like conditions.

### Representative demonstrated rate
Production-intent configuration/material/process/staffing with measured losses and accepted output.

### Sustained operating evidence
Repeated performance over a period that captures meaningful variation/changeover/recovery conditions.

These are repository synthesis labels; do not present them as an external standard.

## 15. Applicability statement
This episode teaches general manufacturing-flow/capacity reasoning. Exact definitions of takt, capacity, run-at-rate, OEE and contractual production-rate demonstrations can vary by company, industry and customer requirement. Any external required threshold or formal Run-at-Rate method must be sourced and scoped before publication.

## 16. What this episode must NOT claim
- takt equals cycle time;
- bottleneck is permanently the slowest nominal machine;
- 100% utilization is the goal for every resource;
- OEE is system capacity;
- peak rate proves sustainable capacity;
- a short run proves commercial production readiness;
- automation is the default capacity solution;
- one universal utilization/OEE target applies to all factories.

## 17. Quantitative gate
Before CLAIM SET STABLE / EVIDENCE VERIFIED:
1. independently verify every equation and unit;
2. label all illustrative numbers;
3. define gross vs net available time explicitly;
4. distinguish input units, gross output, FPY, accepted output and shipped/released output;
5. model rework as a capacity-consuming loop where material to the conclusion;
6. perform sensitivity if a recommendation changes with uncertain availability/yield/demand;
7. avoid false precision from tiny time-study samples.

## 18. Research/source backlog before CLAIM SET STABLE
1. Package authoritative support for takt/cycle-time distinctions.
2. Package operations/constraint support for local-vs-system optimization.
3. Verify OEE definition/source and preserve P2.07 guardrails.
4. Decide whether any formal Run-at-Rate methodology belongs here or later supplier/pilot episodes.
5. Independently check all worked-example arithmetic.
6. Cross-check P2.04 capacity/ramp and P2.05 economics examples.
7. Technical review: manufacturing/process + operations/NPI.

## 19. Pilot-test objective
Episode 29 tests the packaging system under a quantitative practitioner topic.

Pilot PASS signal:
A listener should be able to take a real process flow and distinguish demand/takt, cycle time, nominal capacity, effective good capacity and the current constraint — then explain why the proposed local improvement would or would not increase accepted system output.

## 20. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: LOW-MEDIUM
Quantitative burden: HIGH
Backbone risk: MEDIUM — arithmetic/definition discipline required
Source verification: OPEN

Next status target:
`RESEARCH PACK OPEN → CLAIM SET STABLE`
