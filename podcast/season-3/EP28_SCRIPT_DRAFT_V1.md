# EP28 Full Script Draft V1 — Yield, Rework, Scrap and the Learning Curve

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 3 — Build the Factory Before You Need the Factory
source_outline: EP28_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-03/
spoken_normative_standard_claims: NONE
universal_yield_thresholds: NONE

## Production note — not spoken

Yield terminology varies by organization. This script explicitly defines the meanings it uses and avoids universal FPY/RTY thresholds. Rework-history principles reuse Wave 01/02.

# SPOKEN SCRIPT

## Opening

A factory reports 96 percent yield.

That sounds excellent.

Then you walk the line.

One unit fails final test.

It is opened.

A connector is reseated.

It passes.

Another unit fails calibration.

A technician adjusts it.

It passes.

Another fails leak test.

The seal is replaced.

It passes.

By the end of the week, almost everything shipped.

The final yield looks strong.

But one in three units did not pass the process the first time.

The factory is producing good product.

It is also producing a lot of rescue.

That is why yield can become a dangerous number when we do not say which yield we mean.

This episode is about making production learning visible.

First-pass success.

Rework.

Repair.

Scrap.

Retest.

Recurrence.

Time.

Cost.

Capacity.

Because a final PASS does not erase the path that got there.

---

## 1. Define the language before reading the dashboard

Different companies use yield terminology differently.

So for this episode, we will use a simple definition.

**First-pass yield** means the fraction of units that pass the defined process or test the first time without rework or repair.

**Final accepted output** means units that eventually meet release criteria after any permitted recovery path.

These are both useful.

They answer different questions.

Final accepted output tells us what we eventually shipped or released.

First-pass success tells us how much of the process worked without rescue.

If you show only the final number, you can hide a production system that is still unstable, labor intensive or dependent on technicians.

So every yield number needs a definition and a boundary.

Which process?

Which population?

Which configuration?

Which time period?

Before or after rework?

---

## 2. A final PASS is not the whole history

This is one of the global rules of the series.

Rework adds history.

It does not erase history.

Suppose a Sentinel Node fails final communication test.

The unit is opened.

A connector pin is corrected.

The product passes retest.

What is the unit's state now?

PASS.

What is the unit's history?

Initial fail.

Rework.

Retest.

Final pass.

Both matter.

If the database stores only the final state, the factory loses the evidence that a process mechanism exists.

The next week, the same defect appears.

Then again.

But because each unit eventually passed, the organization thinks it has isolated incidents instead of a recurring mechanism.

This is why rework records are not paperwork residue.

They are process-learning data.

---

## 3. Rework is not free capacity

Now connect quality to flow.

Imagine the production constraint is calibration and final functional test.

A failed unit comes back after rework.

It uses the same tester again.

The product eventually passes.

From the customer's perspective, good.

From the capacity perspective, the tester spent time twice.

That second pass consumed scarce production time.

This is the hidden capacity cost of rework.

Even if the replacement material is cheap.

Even if the technician fixes it quickly.

Even if scrap is zero.

The resource burden can still be substantial.

That is why rework belongs in the capacity model.

It is not only a cost-of-quality number.

If rework returns to the constraint, it directly reduces the amount of new good product the system can process.

Episode 29 will quantify this.

---

## 4. Rework, repair, scrap and deviation are not interchangeable

Organizations use these words differently, so I am not going to pretend there is one universal taxonomy.

But the semantic distinctions matter.

Rework generally means processing the product again so it conforms to the original requirement or approved definition.

Repair may restore usability through a different condition or method, depending on the organization's definition and approval system.

Scrap removes the unit from usable production.

A deviation or concession may authorize a bounded departure under defined conditions.

The exact local terminology can vary.

The important thing is that the disposition path remains explicit.

Why?

Because different paths have different effects on:

Product configuration.

Reliability.

Cost.

Capacity.

Traceability.

Customer approval.

Future root-cause analysis.

If all of them disappear into one field called “fixed,” the evidence is gone.

---

## 5. Use defect recurrence as the learning signal

A defect is found.

Contain it.

Good.

Now ask:

Did the corrective action change future populations?

Suppose connector damage falls from 12 occurrences to 2.

Useful.

Are those two the same mechanism?

Different supplier lot?

Different operator?

Different fixture state?

If the mechanism continues, the action may have reduced frequency without removing the cause.

That may be acceptable.

Or not.

The point is to measure effectiveness.

A closed NCR is administrative closure.

A changed future population is engineering evidence.

So when you build a defect Pareto, do not only count defects.

Connect them where practical to:

Process step.

Configuration.

Supplier or lot.

Operator or equipment.

Rework path.

Corrective action.

Recurrence after action.

That turns the Pareto into a learning system.

---

## 6. Segment yield when the population matters

A single yield number can hide important differences.

Rev A and Rev B.

Supplier 1 and Supplier 2.

Shift 1 and Shift 2.

Tool 1 and Tool 2.

Old fixture and new fixture.

Before and after process change.

This does not mean you should slice every dataset into meaningless tiny groups.

Segment where the identity can plausibly affect the failure mechanism or the decision.

If the product/process population changed, ask whether combining the data is still legitimate.

This is where configuration management meets quality.

Without identity, yield can become an average of unlike systems.

---

## 7. The learning curve is not automatic

Teams often assume ramp naturally improves.

The first build is slow.

The tenth is faster.

The hundredth is better.

Sometimes.

But improvement is not magic.

Ask what changed.

Operators learned a motion.

The fixture was improved.

The work instruction became clearer.

A supplier defect was removed.

A design feature was simplified.

The test station became more reliable.

The maintenance plan improved.

If nothing changes except calendar time, do not assume the curve will improve.

And do not teach a generic percentage learning rate without evidence.

The useful ramp question is:

**Which interventions should disappear as maturity increases?**

Designer-assisted assembly?

Manual parameter edits?

Extra inspection?

Rework loops?

Supplier expediting?

If those do not disappear, the process may be scaling rescue rather than scaling capability.

---

## 8. The Yield Learning Ledger

Here is the listener tool.

For each relevant production population, record:

Unit or build population.

First result.

Defect mode.

Process step or source.

Containment.

Rework or repair.

Retest result.

Time and cost burden.

Root-cause action.

Affected population.

Recurrence.

Effectiveness.

Let's use the Sentinel connector.

Population:

First 50 LVP units.

First-pass failures:

Eight communication failures.

Process step:

Connector installation.

Rework:

Open enclosure, reseat connector, retest.

Burden:

Technician time plus second tester cycle.

Action:

Fixture alignment feature added and assembly sequence changed.

Next population:

50 units after fixture change.

Now ask:

What happened to first-pass success?

What happened to rework minutes?

Did the failure mechanism recur?

That is learning evidence.

---

## 9. Yield connects quality, capacity and economics

Yield is not owned by the quality department.

It affects production flow.

Suppose the process launches 100 units.

Ninety pass first time.

Ten require rework.

If those ten re-enter a constrained station, the line now has more than 100 operations to complete for 100 launched units.

If some scrap, material consumption rises.

If rework takes engineering support, labor cost rises.

If retest delays release, lead time rises.

If rework hides a supplier problem, field risk may rise.

That is why cost per launched unit and cost per accepted unit are not necessarily the same.

And why nominal cycle rate is not good-unit capacity.

Quality data are inputs to economics and capacity.

Not separate dashboards.

---

## 10. DEV to LVP to ramp

In development, rescue can be perfectly rational.

You are learning.

Hand rework may be the fastest way to test the next question.

But record it.

In LVP, rescue should become visible in production metrics.

What is failing?

What is being reworked?

What still needs engineer help?

During ramp, repeated rescue becomes production debt.

It consumes capacity.

Costs money.

Creates schedule risk.

And can hide process instability behind a good final-output number.

The goal is not zero rework at all costs.

The goal is knowing what rework means about the maturity of the system.

---

## 11. Six traps to avoid

Trap one:

Final yield is the only yield that matters.

Trap two:

A final PASS makes the first failure irrelevant.

Trap three:

Rework is free because the part is eventually good.

Trap four:

All products and configurations belong in one yield number.

Trap five:

Scrap reduction automatically proves the process improved.

Maybe scrap fell because rework increased.

Trap six:

The learning curve happens automatically with volume.

Learning requires change and evidence.

---

## 12. The action after this episode

Take last week's production report.

Add three columns if they are missing:

First-pass result.

Rework minutes.

Failure mechanism.

Then ask:

How much of the output was produced by the intended process?

And how much was produced by rescue?

That answer tells you where the next production-learning effort belongs.

---

## Closing

Episode 28 exposed the hidden work behind good output.

Now we can ask the capacity question honestly.

If a test station runs every failed unit twice...

If downtime removes an hour from the shift...

If WIP keeps growing before calibration...

If the fastest station is not the system constraint...

How many accepted units can the system actually deliver?

That is Episode 29:

**Capacity, Bottlenecks, Takt Time and Line Balance.**

Because machine speed is not system capacity.

# End spoken script

## Draft source anchors — not spoken

- W3-S07 — NIST inventory/flow-time manufacturing context.
- W3-S08 — NIST flow-time/productivity context.
- Wave 01/02 — failure/rework history and quality-effectiveness logic.
- Sentinel examples are illustrative; no universal FPY/yield threshold.
