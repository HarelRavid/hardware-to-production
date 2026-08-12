# P2.04 — WIP, Queue Growth, Rework Recursion & Run-at-Rate Worked Example

Status: ACTIVE — NUMERICAL FLOW EXAMPLE CAPTURED

## Purpose
Show why a line can appear to run at target rate for a short window while being structurally incapable of sustaining that rate. The example extends the Sentinel Node PVT line.

## Baseline
Demand: 80 accepted units/shift
Net production time: 420 min/shift = 25,200 s
Required takt: 315 s/accepted unit

Constraint station: Calibration + Functional Test
Nominal cycle time: 360 s/cycle
Nominal maximum: 70 cycles/shift before downtime, failures, rework, changeover or interruptions.

Assume for the worked example:
- effective station availability during the run: 90%
- first-pass yield at the constraint: 92%
- failed units are eligible for one rework loop
- rework consumes the same constraint resource for 240 s per failed unit
- 75% of reworked units recover and become accepted product

## 1. First-pass constraint capacity
Available constraint time = 25,200 × 0.90 = 22,680 s

If all time were used only for first-pass tests:
22,680 / 360 = 63 first-pass cycles/shift

Expected first-pass accepted output:
63 × 0.92 = 57.96 ≈ 58 units

Expected first-pass failures:
63 × 0.08 = 5.04 ≈ 5 units

But the failed units create additional demand on the same constrained resource.

## 2. Rework recursion
A simple first-order approximation for constraint time per launched unit is:

T_effective ≈ T_first_pass + q × T_rework

where q is the probability of entering the rework loop.

Here:
T_effective ≈ 360 + 0.08 × 240 = 379.2 s per launched unit before considering repeat rework loops.

If repeat loops are possible, the resource burden becomes a geometric series and must be modeled from the actual routing probabilities rather than hidden inside FPY.

The important production lesson is that rework is not only a quality cost. If it returns to the bottleneck, it consumes bottleneck capacity.

## 3. Short target-rate burst that is not sustainable
Suppose upstream assembly releases 80 units/shift equivalent to the test station.
Arrival rate to test = 80 / 420 = 0.1905 units/min = 11.43 units/hour.

Nominal test service rate = 60/6 = 10 units/hour before availability loss.
At 90% availability, practical first-pass service opportunity is approximately 9 cycles/hour before rework burden.

Therefore arrivals exceed sustainable departures.

If operators pre-stage product and run the upstream stations at takt for two hours, the dashboard can show an apparent target production rhythm while the queue before calibration grows.

Illustrative queue growth ignoring rework:
arrival = 11.43 units/hour
effective service ≈ 9.0 units/hour
net queue growth ≈ 2.43 units/hour

After 4 hours, approximately 9.7 additional units are waiting at the constraint even though upstream stations may report good local performance.

Rework makes the condition worse because failed units re-enter the constrained resource.

## 4. Little's Law guardrail
For a stable system, WIP, throughput and average flow/cycle time are linked by Little's Law:

WIP = Throughput × Flow Time

NIST manufacturing research uses this relationship and notes that cycle/queue time and WIP can grow sharply as utilization increases.

Do not misuse Little's Law as permission to add WIP. Physical constraints bound throughput; excess WIP often manifests as longer queues and longer flow time rather than higher sustainable output.

## 5. Why the burst can fool a team
A short run can look successful if:
- material is pre-staged outside normal logistics;
- engineering staff intervene;
- failed units are moved aside and rework is deferred;
- changeovers are excluded;
- preventive maintenance is excluded;
- upstream stations continue producing into an expanding queue;
- inspection/test steps are temporarily bypassed or staffed above normal;
- the run ends before accumulated WIP, fatigue, downtime or replenishment problems become visible.

Therefore the observation "we hit 80/day equivalent for 30 minutes" is not evidence of 80/day sustainable capacity.

## 6. Run-at-Rate Scorecard
A defensible run-at-rate record should state at minimum:

1. Demand / required accepted output
2. Defined net available production time
3. Product mix and configuration
4. Normal staffing and skill assumptions
5. Normal equipment/tooling/fixtures
6. Material and supplier representativeness
7. Constraint station and measured cycle distribution
8. Downtime and availability losses
9. First-pass yield and accepted output
10. Rework quantity, routing and consumed resource time
11. Scrap
12. WIP/queue at start and end
13. Changeovers and replenishment
14. Engineering interventions / abnormalities
15. Run duration
16. Accepted throughput versus required takt

## 7. Queue Stability Test
For each critical buffer during a run, record:

Q_start
Q_end
Run duration
Arrival count
Departure count
Rework returns

A simple warning signal is:

Q_end > Q_start with persistent positive net inflow.

One observation is not enough to characterize the stochastic system, but a steadily growing queue is direct evidence that the tested operating condition is not in flow balance.

A line should not be declared sustainable merely because local stations achieved their target cycles while system WIP increased materially.

## 8. Sentinel Node worked conclusion
Under the stated assumptions, the calibration/test station is structurally below the demand rate before rework is fully accounted for. The correct ramp action is not to pressure upstream assembly to move faster.

Candidate actions include:
- reduce calibration/test cycle time;
- parallelize the constraint;
- improve test availability;
- improve FPY so fewer units consume rework capacity;
- redesign test architecture;
- change product/test requirements only through controlled engineering review;
- revise the demand/shift model if the business requirement allows it.

The constraint must be re-tested after the selected change.

## 9. Ramp Exit Gate — draft
Do not exit pilot/ramp solely because a planned quantity was eventually completed.

Evidence should demonstrate that, under representative conditions:
- accepted throughput meets the defined requirement;
- queues do not grow without bound;
- FPY/rework are understood and controlled;
- normal staffing can operate the process;
- equipment availability and maintenance assumptions are credible;
- supply/replenishment supports the rate;
- process controls and measurement remain active;
- abnormal engineering intervention is not required to maintain output;
- configuration and genealogy remain controlled;
- the run duration is sufficient to expose the failure modes relevant to the claim being made.

Run duration is claim-dependent. No universal number of hours is asserted here.

## 10. Podcast framing
Three different claims must remain separate:

"We reached the instantaneous target rate."
"We completed the target batch."
"We demonstrated sustainable accepted throughput under representative production conditions."

They are not equivalent.

## Evidence notes
- NIST manufacturing analytical work explicitly relates WIP, throughput and queue/cycle time using Little's Law and warns that cycle times and WIP can rise dramatically with utilization.
- NIST work on manufacturing inventory/flow time treats inventory, waiting and rework/defects as production wastes relevant to flow performance.
- Run-at-rate criteria in this document are an engineering synthesis and listener framework; they are not presented as a verbatim universal standard checklist.

## Next
Build the P2.04 canonical Run-at-Rate / Ramp Exit pack and connect this example to the earlier demand→takt→constraint capacity model.