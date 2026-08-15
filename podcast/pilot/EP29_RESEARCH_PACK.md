# Episode 29 Research Pack — Capacity, Bottlenecks, Takt Time and Line Balance

status: CLAIM SET STABLE
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

Verified source boundary: Lean Enterprise Institute defines takt time as available production time divided by customer demand and describes it as the production pace needed to match demand. For the episode, use this as authoritative lean-practice support, not as a statutory/normative requirement.

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

## 5. Core claim register — stable
| ID | Claim | Class | Priority | Status | Note |
|---|---|---|---|---|---|
| EP29-C01 | Takt time is demand-derived available production time per required good unit; it should not be confused with measured station cycle time. | V2/V6 | P0 | SOURCE LOCATED / CLAIM STABLE | Lean Enterprise Institute authoritative lean-practice source. |
| EP29-C02 | System capacity is not equal to the fastest or slowest isolated nominal machine rate without considering flow, availability, quality, rework and dependencies. | V6 + P2.04 | P0 | BACKBONE-STABLE | Quantitative examples checked. |
| EP29-C03 | Accepted sustainable throughput is a more decision-relevant output than short peak machine speed. | V6 + Global Invariant | P0 | BACKBONE-STABLE | Core backbone invariant. |
| EP29-C04 | Improving a non-constraint resource may increase local output/WIP without materially improving serial-system throughput. | V5/V6 | P0 | CLAIM STABLE / SOURCE ENRICHMENT OPEN | Demonstrated by serial-flow arithmetic; operations/TOC enrichment remains useful. |
| EP29-C05 | The system constraint can move after an improvement, so capacity must be re-measured/re-modeled. | V6 + MOVING CONSTRAINT LOOP | P0 | BACKBONE-STABLE | Stress-test repair. |
| EP29-C06 | Yield and rework can materially reduce good-unit capacity even when gross station cycle time is unchanged. | V3/V6 | P0 | ARITHMETIC VERIFIED | Worked examples independently checked. |
| EP29-C07 | OEE can help decompose equipment losses but does not prove root cause or system capacity. | V2/V6 + P2.07 | P0 | BACKBONE-STABLE / SOURCE PACK OPEN | Preserve P2.07 guardrail. |
| EP29-C08 | Capacity evidence should be representative of intended production conditions for the claim being made. | V2/V6 | P0 | CLAIM STABLE / SOURCE ENRICHMENT OPEN | Formal customer-specific Run-at-Rate requirements intentionally deferred unless scoped. |
| EP29-C09 | Capacity expansion decisions should compare simpler flow/process improvements, labor/shift changes, parallelization and automation economically rather than default to equipment purchase. | V6 + P2.05/P2.07 | P1 | BACKBONE-STABLE | Decision synthesis. |

## 6. Source verification note
### Verified/located support
Lean Enterprise Institute (LEI), Takt Time / Lean Lexicon:
- supports `takt time = available production time / customer demand`;
- frames takt as the pace/heartbeat used to match production with demand.

LEI Standardized Work guidance:
- explicitly uses process capacity sheets to calculate machine capacities in linked processes and identify bottlenecks;
- links standardized work to takt, work sequence and standard in-process inventory.

### Source-vs-synthesis boundary
The following remain repository synthesis unless a later episode/source pack explicitly adopts an external definition:
- Accepted Throughput as the preferred backbone output lens;
- Capacity Evidence Ladder;
- Capacity Reality Sheet;
- Constraint Hunt;
- MOVING CONSTRAINT LOOP;
- the rule that investment decisions should compare process/flow/labor/parallelization/automation alternatives.

### Formal Run-at-Rate boundary
Do not teach a universal formal Run-at-Rate procedure in this episode. Customer/industry-specific production-rate demonstrations belong only when the applicable method, customer requirement and acceptance criteria are identified.

## 7. Listener tool — Capacity Reality Sheet
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

## 8. Constraint Hunt — listener tool
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

## 9. Worked example A — basic takt
Illustrative assumptions:
- required output: 240 accepted units/8-hour shift;
- gross shift: 480 min;
- planned non-production time: 60 min;
- available production time: 420 min.

Takt:
`420 / 240 = 1.75 min/good unit = 105 s/good unit`

Arithmetic audit: PASS.

If a critical serial station has a sustained accepted-output interval of 130 s/unit, it cannot support the 105 s demand pace without a change in flow/capacity.

If its best demonstrated cycle is 80 s but recurring recovery/downtime/rework makes accepted output 130 s/unit, the 80 s number is not the capacity claim we need.

All numbers are pedagogical.

## 10. Worked example B — yield changes good capacity
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

Difference:
`352.8 - 324 = 28.8 good units/hour`

Arithmetic audit: PASS.

Nominal machine speed did not change, but first-pass good capacity fell by 28.8 units/hour.

If failed units consume rework capacity, the system penalty is larger and must be modeled as a loop rather than just multiplying by yield.

## 11. Worked example C — one-pass rework workload
Illustrative simplified loop:
- 100 units enter;
- 90% pass first time;
- 10% require one rework attempt;
- rework consumes 60% of the original station time per reworked unit;
- 80% of reworked units pass;
- only one rework opportunity is modeled.

Accepted units after one rework opportunity:
`90 + (10 × 0.80) = 98`

Process workload:
`100 + (10 × 0.60) = 106 unit-equivalents of station time`

Accepted units per original-time equivalent:
`98 / 106 ≈ 0.9245 accepted units per original unit-time equivalent`

Arithmetic audit: PASS.

Guardrail: this is not an infinite recursion model. If failed rework can re-enter the loop repeatedly, use a recurrence/geometric model and state its assumptions explicitly.

## 12. Worked example D — local improvement does not move system output
Three serial operations, simplified effective capacities:
- A = 100 good units/hour;
- B = 70 good units/hour;
- C = 90 good units/hour.

Under the simplified serial/no-buffer-loss assumption, the system ceiling is approximately 70 good units/hour because B is the current constraint.

Improving C from 90 → 120 leaves the simplified ceiling near 70 because B is unchanged.

Improving B from 70 → 95 changes the simplified limiting capacity to C at 90 good units/hour; the constraint has moved.

Arithmetic/logic audit: PASS.

Guardrail: real systems can include buffers, blocking/starving, batch behavior, shared labor, changeovers and reliability interactions; the example teaches the local-vs-system principle, not a universal line model.

## 13. Sentinel Node example
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

## 14. OEE boundary
If equipment OEE is used:
`OEE = Availability × Performance × Quality`

Use it to decompose losses for the equipment/workcell whose definitions are controlled.

Do not infer:
- root cause from OEE alone;
- system throughput from one machine OEE;
- economic justification for automation from a higher OEE target alone.

Exact OEE source/definition remains a Podcast-Ready verification item inherited from P2.07; Episode 29 does not need to settle competing implementation conventions to stabilize its claim set.

## 15. Capacity evidence ladder
### Estimate
Engineering estimate based on assumed cycle time/staffing/yield.

### Measured short-run
Observed under limited production-like conditions.

### Representative demonstrated rate
Production-intent configuration/material/process/staffing with measured losses and accepted output.

### Sustained operating evidence
Repeated performance over a period that captures meaningful variation/changeover/recovery conditions.

These are repository synthesis labels; do not present them as an external standard.

## 16. Applicability statement
This episode teaches general manufacturing-flow/capacity reasoning. Exact definitions of capacity, OEE and contractual production-rate demonstrations can vary by company, industry and customer requirement. Takt is used here in the lean-production sense supported by LEI. Any external required threshold or formal Run-at-Rate method must be sourced and scoped before publication.

## 17. What this episode must NOT claim
- takt equals cycle time;
- bottleneck is permanently the slowest nominal machine;
- 100% utilization is the goal for every resource;
- OEE is system capacity;
- peak rate proves sustainable capacity;
- a short run proves commercial production readiness;
- automation is the default capacity solution;
- one universal utilization/OEE target applies to all factories.

## 18. Quantitative gate — pilot result
1. Every equation/unit in the four worked examples independently checked. — PASS
2. All illustrative numbers explicitly pedagogical. — PASS
3. Gross vs net available time explicitly separated. — PASS
4. Input/gross/FPY/accepted output distinctions visible. — PASS
5. Rework modeled as capacity-consuming workload where material. — PASS
6. Sensitivity required later when an episode recommendation depends on uncertain real inputs. — RULE RETAINED
7. False precision from tiny time-study samples prohibited. — RULE RETAINED

## 19. Remaining work before EVIDENCE VERIFIED / PODCAST READY
1. Package final citation/source note for LEI takt/standardized-work support.
2. Add an authoritative OEE source in the P2.07/Episode source pack and preserve the equipment-vs-system boundary.
3. Optional: add operations/TOC literature for constraint/local-optimization enrichment without making the episode dependent on branded TOC terminology.
4. Technical review: manufacturing/process + operations/NPI.
5. Decide during scripting whether to include a sensitivity mini-example; do not add math merely for density.

## 20. Pilot-test objective
Episode 29 tests the packaging system under a quantitative practitioner topic.

Pilot PASS signal:
A listener should be able to take a real process flow and distinguish demand/takt, cycle time, nominal capacity, effective good capacity and the current constraint — then explain why the proposed local improvement would or would not increase accepted system output.

## 21. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: LOW-MEDIUM
Quantitative burden: HIGH
Backbone risk: LOW-MEDIUM after arithmetic/source-boundary audit
Source verification: PARTIAL / sufficient for CLAIM SET STABLE
Arithmetic verification: PASS

Next status target:
`CLAIM SET STABLE → PILOT BATCH AUDIT → EVIDENCE VERIFIED`
