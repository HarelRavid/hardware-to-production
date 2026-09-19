# EP26 Full Script Draft V1 — How to Plan a Pilot Build

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 3 — Build the Factory Before You Need the Factory
source_outline: EP26_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-03/
spoken_normative_standard_claims: NONE
customer_specific_pilot_rules: EXCLUDED

## Production note — not spoken

NASA PRR is used only as authoritative production-readiness context. The Pilot Build Plan, quantity rationale, intervention logic and exit structure are Hardware-to-Production synthesis. No universal pilot quantity or stop threshold is asserted.

# SPOKEN SCRIPT

## Opening

A team plans its first pilot build.

They pick a number: 25 units.

The build goes reasonably well.

Some units need rework.
A few parts are substituted.
Engineering helps the operators through two difficult steps.
The test station is patched during the build.
Most of the units are eventually good.

The team ships almost all of them and calls the pilot successful.

Three weeks later, somebody asks a basic question:

What exactly did the pilot prove?

Did the operators build the intended process?
Did the supplier parts match the production source?
How much rework happened?
Did the test station work normally?
Which configuration produced which result?
Which problems required engineer rescue?
What should stop us from ramping?

Nobody can answer cleanly.

That is the pilot-build trap.

A pilot is not successful because a small batch eventually came out of the factory.

A useful pilot is an evidence-generating experiment.

It has a purpose.

It has a bounded configuration.

It has a data plan.

It has rules for intervention and change.

And it ends with a decision.

That is what this episode is about.

By the end, I want you to be able to plan a pilot around the decision it must support rather than around an arbitrary unit count.

---

## 1. Start with the decision after the pilot

Before asking how many units to build, ask:

What decision comes next?

Are we deciding whether the assembly method is workable?

Whether the supplier route is representative?

Whether operators can build without continuous design-engineer help?

Whether the production test finds the right failures?

Whether a fixture is mature enough for a more formal validation build?

Whether the product is ready for limited customer release?

Those are different decisions.

And they require different evidence.

This is one of the lessons we can borrow from formal production-readiness thinking.

NASA's Production Readiness Review, for example, looks at a broad production system: documentation, process controls, production resources, tooling and test equipment, personnel, suppliers and unresolved production issues.

We are not copying the NASA review into a startup.

We are using the same underlying idea:

Production readiness is a system claim.

So define the claim.

If the pilot has no explicit post-build decision, the team will collect whatever data happen to be convenient and call it learning afterward.

---

## 2. Define the configuration and the evidence envelope

The next question is:

What exactly are we building?

Which product revision?

Which PCB?

Which firmware?

Which material?

Which supplier?

Which fixture?

Which test procedure?

Which work instruction?

Which operator qualification state?

Which process route?

Which deviations are already approved?

A pilot can include variation deliberately.

Maybe you are comparing two fixtures.

Maybe two suppliers are being evaluated.

Maybe half the units use one process setting and half use another.

That is fine.

The problem is mixing them and later reporting one result.

If fifteen units used Rev B and ten used Rev C, that is not one population unless the changed attribute is irrelevant to the claim.

If one operator had engineering support and another did not, that may matter.

If the first ten units used one test-software build and the next fifteen used a patched build, that matters.

The rule is simple:

**Pilot learning requires identity.**

You need enough configuration and effectivity information to know which evidence belongs to which state.

---

## 3. There is no magic pilot quantity

This is where many teams want a number.

How many units should we build?

Ten?
Thirty?
One hundred?

There is no universal answer.

The quantity should follow the learning question.

If you are validating a fixture interaction, you may need enough repeated cycles to expose the relevant variation.

If you are evaluating multiple operators, you need enough work across operators to learn something.

If supplier-lot behavior matters, one lot may be weak evidence.

If you are testing a failure mechanism that is rare, a very small pilot may never expose it.

But do not reverse that logic and say:

“We built 100 units, therefore the pilot was statistically meaningful.”

Quantity by itself is not evidence quality.

One hundred mixed configurations with poor traceability may teach less than twenty controlled units with the right measurements and conditions.

So for every pilot quantity, write one sentence:

**Why is this quantity enough for the question we are asking?**

If you cannot answer, the number is probably a planning habit rather than an evidence decision.

---

## 4. Build the data plan before the build

The production floor is a terrible place to invent the data plan after problems begin.

Decide in advance what you will record.

At minimum, for a serious pilot, think about:

First result.

Defect mode.

Rework or repair.

Scrap.

Cycle time where relevant.

Operator or station identity.

Supplier or material lot where relevant.

Test/measurement result.

Engineer intervention.

Shortage or material substitution.

Process deviation.

Configuration change.

Downtime or recovery event.

Why capture intervention?

Because intervention is part of the evidence.

If an engineer holds the fixture by hand to make every unit pass, the build may still be valuable.

But the result is:

“we can build with engineer-assisted operation.”

Not:

“normal production can build this.”

The rescue is not embarrassment to hide.

It is the learning.

---

## 5. Decide what intervention is allowed

A pilot is often still a learning build.

So changes can be allowed.

Debugging can be allowed.

Engineer assistance can be allowed.

But define the rules.

For example:

Operators may stop and call engineering after repeated fit problems.

Engineering may propose a temporary fixture shim.

The shim receives an identifier.

Units before and after the change are separated.

The reason for change is recorded.

The affected result is not blended.

This is far better than pretending the build must remain frozen while everyone quietly improvises.

The objective is not zero intervention.

The objective is visible intervention.

Because invisible intervention creates false readiness.

---

## 6. Define stop and containment logic

Suppose a pilot begins producing a repeated critical defect.

Do you keep building because the plan says 25 units?

Maybe not.

A good pilot plan defines conditions that force reassessment.

A safety concern.

A repeated critical functional failure.

A measurement system that becomes unreliable.

A lost configuration boundary.

A process condition that means the remaining units would no longer answer the intended question.

The threshold is risk-dependent.

There is no universal “three failures means stop.”

The important thing is to decide before the pressure of schedule changes the logic.

Stop rules protect the evidence.

Containment protects the product.

---

## 7. Run a daily learning loop

For a multi-day or multi-shift pilot, do not wait until the end to discover that the data are unusable.

Review the build while it is happening.

What defects are recurring?

How much rework?

Which step is consuming engineering time?

Where is WIP building?

Which supplier or material issues appeared?

Did the test method change?

Did cycle time stabilize or degrade?

Were there configuration changes?

What did the operators learn?

Did yesterday's corrective action change today's population?

This is not permission to change the process constantly.

It is a disciplined learning loop.

When a change is made, define effectivity.

Then compare before and after honestly.

---

## 8. Exit the pilot with a decision, not a feeling

At the end, do not ask:

“Did the pilot go well?”

Ask:

What did we prove?

What did we learn?

What did we fail to exercise?

What required abnormal support?

What configuration generated the result?

What risks are still open?

Which ones are acceptable to carry?

Which ones block the next build?

The outcome might be:

Proceed to production validation.

Repeat a focused pilot on the test station.

Proceed with a constrained release while one low-risk gap closes.

Redesign the fixture before continuing.

Change the supplier route.

Those are useful decisions.

“Pilot complete” is not.

---

## 9. The Pilot Build Plan

Here is the listener tool.

Start with:

Decision after pilot.

Then list:

Objectives.

Configuration.

Population or quantity rationale.

Production route and suppliers.

CTQs and test.

Staffing and operator qualification.

Data to capture.

Allowed engineering intervention.

Stop and containment rules.

Change/effectivity rules.

Exit evidence.

Carryover gaps.

That is the Pilot Build Plan.

If the build plan contains only dates, quantities and names, it is not yet an evidence plan.

---

## 10. DEV to LVP to production validation

In early development, builds can change rapidly.

That is fine.

Label the evidence.

As you enter low-volume pilot production, the build still learns—but identity and intervention become much more important because repeated units and multiple people are now involved.

When you reach production validation, the standard changes again.

The question becomes less:

“Can we learn how to make this?”

And more:

“Does the intended production system work as a system under representative conditions?”

That is where we go next.

---

## 11. Five traps to avoid

Trap one:

Pilot quantity becomes the objective.

Trap two:

Mixed configurations are reported as one yield number.

Trap three:

Engineer rescue is hidden because the final units passed.

Trap four:

The process is changed mid-build with no effectivity boundary.

Trap five:

Units are shipped before learning, containment and configuration records are closed.

Shipping is not forbidden.

But the release state must be explicit and the learning must not disappear with the product.

---

## 12. The action after this episode

Take your next pilot-build plan.

At the top of the page write:

**Decision after pilot:**

Complete that line before adding quantity.

Then ask whether every section of the build plan produces evidence for that decision.

If not, redesign the pilot now.

It is much cheaper than discovering after the build that the batch produced product but not knowledge.

---

## Closing

Episode 26 plans the experiment.

The next episode raises the bar.

What happens when the goal is no longer to learn whether the production approach might work?

What evidence do we need before saying the integrated production system is ready for ramp?

That is Episode 27:

**What a Production Validation Build Must Prove.**

Because product verification and production-system readiness are not the same thing.

# End spoken script

## Draft source anchors — not spoken

- W3-S02 — NASA NPR 7123.1D Appendix G, G.9 PRR.
- W3-S03 — NASA Systems Engineering Handbook PRR definition.
- Wave 01 — configuration/effectivity/history.
- Wave 02 — measurement/rework/supplier evidence.
