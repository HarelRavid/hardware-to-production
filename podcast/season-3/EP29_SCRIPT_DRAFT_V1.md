# EP29 Full Script Draft V1 — Capacity, Bottlenecks, Takt Time and Line Balance

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 3 — Build the Factory Before You Need the Factory
source_outline: EP29_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-03/
spoken_normative_standard_claims: NONE
formal_run_at_rate_rules: EXCLUDED

## Production note — not spoken

Lean Enterprise Institute is used for takt/cycle-time definitions. NIST supports WIP/throughput/queue and capacity-system reasoning. All Sentinel numbers are illustrative and independently recalculated.

# SPOKEN SCRIPT

## Opening

Every station on the line looks fast enough.

PCB preparation: fast.

Assembly: fast.

Connector installation: fast.

Final inspection: fast.

The only station that looks slightly slow is calibration and functional test.

Management asks:

“Why are we still missing the daily target?”

The answer is sitting on the floor.

A queue of units waiting for test.

Some failed units are coming back for rework.

The tester restarts twice a shift.

Material is pre-staged to make short runs look smooth.

The line has plenty of local speed.

It does not have enough sustainable accepted throughput.

That distinction is the heart of capacity engineering.

So this episode asks:

**How many good units can the system really deliver under the conditions we plan to operate?**

Not the best cycle.

Not the brochure rate.

Not the fastest operator.

The system.

---

## 1. Start with demand: takt time

Lean Enterprise Institute defines takt time as available production time divided by customer demand.

It is a planning pace.

How frequently does an accepted unit need to leave the system to meet demand?

Take the Sentinel Node example.

We need 80 accepted units in one shift.

The shift is eight hours: 480 minutes.

But planned breaks, cleaning and meetings remove 60 minutes from the production-time basis.

So we use 420 planned production minutes.

That is 25,200 seconds.

25,200 divided by 80 equals:

315 seconds per accepted unit.

That is the takt for this example.

It does not tell us what any station actually takes.

It tells us the demand pace.

---

## 2. Cycle time is what the process actually takes

Cycle time is different.

Lean Enterprise Institute defines cycle time as the time required to produce a part or complete a process, measured in operation.

If a station needs 245 seconds per unit, that is a cycle-time observation.

If another station needs 360 seconds, that is another.

Takt says:

What pace does demand require?

Cycle time says:

What pace does the process currently deliver under the measured conditions?

Do not use the words interchangeably.

They answer different questions.

---

## 3. The longest nominal cycle is a candidate constraint—not always the whole answer

Our Sentinel stations have illustrative effective cycle times:

180 seconds.

245.

275.

360.

210.

The 360-second calibration/test station immediately looks like the constraint.

And in this simple serial example, it is a strong candidate.

But real systems have variability.

Shared operators.

Parallel machines.

Downtime.

Changeovers.

Product mix.

Rework loops.

Material shortages.

A station with a shorter nominal cycle can become the actual constraint if it is unreliable or shares a scarce resource.

So do not identify bottlenecks from the process chart alone.

Observe flow.

Where does WIP grow?

Which resource is saturated?

What actually limits accepted output?

---

## 4. Theoretical capacity is only the first calculation

If the tester takes 360 seconds per cycle and we have 25,200 planned production seconds:

25,200 divided by 360 equals:

70 theoretical test cycles per shift.

Demand is 80 accepted units.

So even before downtime or yield loss, one serial tester is below the demand requirement.

That is already enough to tell us something.

But 70 is still not accepted capacity.

It is ideal cycles under the stated time basis.

Now add reality.

---

## 5. Availability changes the opportunity to produce

Suppose the tester is available 90 percent of the planned production time.

22,680 seconds of effective running time remain.

At 360 seconds per cycle:

63 first-pass test cycles.

Now add first-pass yield.

Suppose 92 percent pass the calibration/final test on first attempt.

63 times 0.92 equals:

57.96.

Call it roughly 58 first-pass accepted units in expectation for the teaching example.

The nominal station speed did not change.

The good-unit output did.

This is why nameplate or stopwatch capacity is only the beginning.

---

## 6. Rework creates new demand on the bottleneck

Now look at the failed units.

Eight percent of first-pass tests fail.

If reworked units return to the same tester, they create additional workload.

In our simplified example, a rework retest consumes 240 seconds at the constrained resource.

A first-order way to see the burden is:

360 seconds first pass

plus 0.08 times 240 seconds expected rework burden.

That equals:

379.2 seconds per launched unit equivalent before repeat loops.

This is deliberately simplified.

Real rework routing can branch.

Some units scrap.

Some need multiple loops.

Some use a different resource.

The point is not the exact model.

The point is:

**rework is capacity consumption.**

It cannot be credited as free recovery.

---

## 7. WIP tells you where flow balance is failing

Now imagine upstream assembly releases work at the pace needed for 80 units in a seven-hour planned production window.

That is about 11.43 units per hour arriving at test.

The tester, at six minutes nominal and 90 percent availability, has roughly nine first-pass cycle opportunities per hour before rework.

Arrivals exceed departures.

What happens?

Queue.

In the simplified deterministic illustration:

11.43 minus 9 equals about 2.43 extra units per hour waiting at the constraint.

After several hours, upstream stations can look productive while the queue grows.

Local efficiency looks good.

System flow is not balanced.

NIST manufacturing research uses relationships among throughput, WIP and cycle/queue time and shows why high utilization can drive WIP and waiting sharply upward.

The lesson is not:

“WIP is always bad.”

The lesson is:

WIP is not capacity.

If the physical constraint cannot process work fast enough, adding inventory before it only makes the queue larger.

---

## 8. Little's Law: useful, but do not misuse it

A classic average-flow relationship is:

WIP equals throughput times flow time.

That is Little's Law.

It is powerful.

But it is not a magic transient-queue predictor.

Use it for appropriate stable average-flow relationships.

Do not say:

“If I add WIP, throughput must go up.”

The physical system still constrains throughput.

Extra WIP often shows up as longer flow time.

The relationship helps explain the system.

It does not remove the constraint.

---

## 9. Short target-rate burst is not sustainable capacity

A team can hit the target rate for thirty minutes.

Material is pre-staged.

Engineers stand at the line.

Failed units are placed aside.

No changeovers occur.

Maintenance is ignored.

Downstream WIP grows.

Then the run ends.

Did the team achieve target pace?

Yes, for that window.

Did it prove sustainable capacity?

No.

Those are different claims.

A credible capacity demonstration has to state:

Duration.

Product mix.

Staffing.

Material state.

Downtime.

Yield.

Rework.

WIP start and end.

Engineering intervention.

Maintenance/recovery.

Accepted throughput.

This is why formal Run-at-Rate requirements are often customer specific.

The concept is general.

The exact acceptance method is not.

---

## 10. The bottleneck moves

Suppose we improve the tester.

Cycle time drops.

Availability improves.

Great.

Are we done?

Maybe the connector station is now the constraint.

Or material replenishment.

Or final data upload.

Or supplier delivery.

This is the moving-constraint loop.

After a meaningful improvement, re-measure the system.

Do not keep optimizing the old bottleneck because the dashboard still has its name highlighted.

The objective is system output.

Not local perfection.

---

## 11. Capacity before CapEx

Now somebody says:

“Buy a second automated tester.”

Maybe.

But before spending capital, compare alternatives.

Remove unnecessary test content only if engineering evidence supports removal.

Reduce setup and handling.

Improve tester recovery.

Improve first-pass yield so rework stops consuming constraint time.

Add a second simpler fixture.

Change staffing or shift pattern.

Parallelize.

Redesign the test architecture.

Then compare the economics.

NIST manufacturing investment guidance gives us tools like NPV, IRR, payback and sensitivity analysis for material investments.

And NIST investment-return research shows that bottleneck reduction and scheduling can be high-return categories in the studied manufacturing dataset.

That does not mean “never automate.”

It means:

**Do not automate a forecast. Automate the demonstrated constraint after the evidence earns the investment.**

---

## 12. The Capacity Reality Sheet

Here is the listener tool.

Start with demand good units per shift.

Net available production time.

Takt.

Then for each important station or resource:

Cycle-time distribution.

Staffing.

Downtime.

Changeover.

FPY.

Rework load.

Scrap.

Queue or WIP.

Accepted output.

Evidence class: measured, demonstrated or assumed.

Then ask:

What is the current system constraint?

What happens if we improve it?

What is the next constraint?

That is capacity reasoning.

---

## 13. DEV to LVP to ramp

In DEV, rough time estimates are often enough.

You are choosing architecture.

In LVP, start measuring actual cycles, interruptions, yield and rework.

In production validation and ramp, capacity claims need representative people, tools, materials, test content and enough duration to expose the losses relevant to the claim.

The maturity progression is simple:

Estimate.

Measure.

Demonstrate.

Sustain.

Do not skip from estimate to commitment.

---

## 14. Six traps to avoid

Takt equals cycle time.

No.

Longest nominal cycle always equals the system bottleneck.

Not always.

Fastest observed cycle equals capacity.

No.

WIP increases capacity.

Not by itself.

Rework is free because the unit eventually passes.

No.

Thirty minutes at target pace proves run-at-rate.

Only for a very narrow claim.

---

## 15. The action after this episode

Go to the current constraint.

Not the station with the scariest spreadsheet.

The resource where work actually queues or output is truly limited.

Calculate:

Available time.

Actual cycle distribution.

Downtime.

First-pass yield.

Rework time.

Accepted units per hour.

Then compare that with demand.

That is the number to bring to the next CapEx discussion.

---

## Closing

Episode 29 established the internal capacity story.

But your factory is not the only production system.

A supplier can make ten beautiful samples and still fail at ramp.

A contract manufacturer can quote enormous machine capacity and still lack the staffing, measurement, material flow or change discipline to deliver it.

So Episode 30 asks:

**Is the external production system actually ready for the same ramp?**

Supplier Readiness and Contract-Manufacturer Management.

# End spoken script

## Draft source anchors — not spoken

- W3-S04 — Lean Enterprise Institute Takt Time.
- W3-S05 — Lean Enterprise Institute Cycle Time.
- W3-S06 — NIST manufacturing analytical services / Little's Law and utilization/WIP.
- W3-S07 — NIST inventory and flow time.
- W3-S10/S11/S14 — investment-analysis and bottleneck-investment context.
- All Sentinel arithmetic is illustrative and independently verified.
