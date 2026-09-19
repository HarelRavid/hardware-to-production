# EP41 Full Script Draft V1 — When Not to Automate

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 5 — Automation, Data and the Connected Factory
source_outline: EP41_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-04/
spoken_normative_standard_claims: NONE

## Production note — not spoken

This script treats automation readiness as Hardware-to-Production synthesis supported by NIST automation/robotics sources plus Waves 01–03. It does not make clause-level machinery-safety claims.

# SPOKEN SCRIPT

## Opening

A team has a painful assembly step.

Operators struggle to align a connector.

The step creates rework.

Cycle time varies.

Engineering keeps changing the product.

Someone says:

“We should automate it.”

A robot is proposed.

The demo looks excellent.

The robot repeats the motion perfectly.

The cell is installed.

And the same connector defect appears.

Now the process is harder to change.

Recovery takes a technician.

A new product revision needs new tooling and programming.

The machine repeats the unresolved problem with more consistency and less flexibility.

The problem was not insufficient automation.

The problem was automating before the process was understood.

That is the question for this episode:

**When is automation the wrong next step—even if the technology can technically perform the task?**

Automation is not a maturity badge.

It is one possible production architecture.

And like any architecture, it should earn its place by solving the right problem.

---

## 1. Start with the manufacturing problem, not the machine

Before discussing robots, PLCs, vision or automation vendors, write one sentence:

What are we trying to improve?

A safety exposure?

An ergonomic burden?

A quality failure mechanism?

A throughput constraint?

Labor availability?

Data capture?

Consistency?

Cost?

Those are very different problems.

NIST's manufacturing-automation guidance starts from business and operational need, not from technology for its own sake.

That matters because automation can be technically feasible and still be the wrong intervention.

If the real problem is bad part presentation, buy or redesign the fixture.

If the problem is unstable incoming material, fix the source/process.

If the problem is poor measurement, automate the wrong measurement and you get bad decisions faster.

If the process is not the system constraint, a faster machine may only build WIP.

So automation readiness begins with a problem statement.

Not a purchase order.

---

## 2. Understand the mechanism before you encode it

Return to the Sentinel connector.

Why does the connector fail?

Misalignment?

Excess insertion force?

Part variation?

Poor visibility?

Fixture freedom?

Operator technique?

If we do not know the mechanism, full automation is a dangerous way to learn.

A robot can repeat a motion.

It does not automatically know whether the motion is correct for every variation of the process.

Sometimes automation exposes the mechanism and helps stabilize it.

Sometimes it simply hides the human feedback that previously signaled something was wrong.

So the readiness question is:

Do we understand the input variation, the CTQ, the failure mechanism and the reaction enough to encode them?

Not perfectly.

But enough that the machine is automating a controlled process rather than replacing visible uncertainty with invisible software.

---

## 3. Operator judgment is data

Manual work often contains tacit compensation.

An experienced operator feels that one connector is tighter.

Rotates the part slightly.

Notices a seal is mispositioned.

Slows down on a difficult batch.

That can be a weakness because it creates operator dependence.

It can also be valuable information.

Before removing the human, ask what the human is compensating for.

Is it unnecessary habit?

Or real process variation nobody has modeled?

The goal is not to preserve craftsmanship forever.

The goal is to convert hidden judgment into explicit engineering where the process requires it.

Fixture.

Sensor.

Process limit.

Material requirement.

Error detection.

Reaction logic.

Only then decide what should stay human and what should become automatic.

---

## 4. Repeatability is not process capability

Robots are often sold on repeatability.

Repeatability is useful.

NIST makes an important distinction between repeatability and accuracy: a robot can return consistently to the same point and still not be at the correct point.

And even a robot that is both accurate and repeatable does not prove the manufacturing process is capable.

Part geometry can vary.

Fixtures can wear.

The end effector can drift.

Material can change.

The measurement system can be weak.

The process window can be too narrow.

Process capability is a system result.

Robot repeatability is one input.

Do not confuse the specification of one component with evidence about the output of the full process.

---

## 5. The intervention ladder

Now ask the most useful automation question:

What is the simplest intervention that removes the dominant loss?

For Sentinel, start at manual.

Then consider a keyed fixture or poka-yoke.

Maybe the defect disappears because the fixture removes angular freedom.

Next level:

Assisted tooling.

Operator loads the part, but controlled insertion force/displacement removes variation and records data.

Next:

Semi-automatic.

Operator loads and unloads; machine executes insertion and verification.

Then:

Fully automatic handling, insertion, verification and routing.

Each step adds capability.

It also adds integration, maintenance, safety, recovery and change burden.

So the correct level is not the highest level.

It is the lowest-complexity architecture that robustly satisfies the required safety, quality, rate, flexibility and economics envelope.

---

## 6. Do not automate the wrong constraint

Suppose connector assembly is unpleasant.

But downstream calibration is still the system bottleneck.

Automating connector insertion may improve local labor and quality.

That can still be valuable.

But do not justify it with a throughput claim that belongs to another station.

Wave 03 gave us the capacity rule:

System accepted throughput is what matters.

If automation is being sold as a capacity project, prove that the operation is actually limiting the system or that it must improve to support the next constraint state.

Otherwise, call the benefit what it really is:

ergonomics.

quality.

labor.

data.

safety.

Do not invent a rate benefit because rate is easy to put in a spreadsheet.

---

## 7. Product change frequency matters

Automation likes stable interfaces.

Dedicated tooling, feeders, nests, recipes and vision models become more valuable when the product architecture is stable enough to reuse them.

If geometry changes every two months, the automation may spend more time being re-engineered than producing value.

That does not mean low-volume/high-mix automation is impossible.

NIST robotics research is explicitly aimed at greater flexibility and reconfigurability.

But flexibility is not free.

It must be designed, measured and paid for.

So include product life, expected variants and changeover burden in readiness.

---

## 8. Safety, recovery and maintenance are not afterthoughts

The automatic cycle is the easy demo.

The hard engineering questions are:

What happens when the part is missing?

The sensor disagrees?

The air supply drops?

The tool jams?

Power fails?

Someone opens the guard?

The wrong recipe is selected?

Who recovers the cell?

Operator?

Technician?

Vendor?

How long?

What product state is left inside?

Can the system restart without losing unit identity or bypassing a quality check?

And can it be maintained by the actual organization?

If those questions have no owner, the automation is not ready even if the nominal motion works.

---

## 9. The Automation Readiness Gate

Here is the listener tool.

Ask:

Is the product/configuration stable enough for the investment?

Do we understand the process mechanism?

Can we trust the measurement?

Do we know the real constraint and losses?

Is the manual or semi-manual method repeatable enough to understand?

Have simpler interventions been tested?

What safety architecture is needed?

What happens during faults and recovery?

Who maintains it?

What changes invalidate the solution?

Does the lifecycle economics justify it?

Then make the decision:

Automate.

Semi-automate.

Fix the process first.

Defer.

The gate is not anti-automation.

It is anti-automation theater.

---

## 10. DEV, LVP and SVP

In development, automation can be useful when it is itself the experiment.

Automated data collection.

Repeatable test.

Safe handling of a hazardous task.

But avoid freezing an unstable architecture into expensive dedicated tooling.

In LVP, selective automation often has the best learning value.

Fixtures.

Assisted tools.

Semi-automatic test.

Simple error-proofing.

In SVP, larger automation investments become more defensible when demand, process stability, measurement, rate, maintenance and product life are demonstrated.

The maturity is not the automation percentage.

The maturity is the evidence.

---

## 11. Five traps

Trap one:

If a robot can do it, we should automate it.

No.

Trap two:

Robot repeatability equals process capability.

No.

Trap three:

Operator judgment is just waste.

Sometimes it is. Sometimes it is unmodeled process knowledge.

Trap four:

Full automation is more mature than semi-automation.

Not necessarily.

Trap five:

We will fix recovery and maintenance after launch.

That is how a fast machine becomes an expensive source of downtime.

---

## 12. The action after this episode

Take the automation proposal currently closest to approval.

Remove the words robot, cobot, vision, PLC and vendor name.

Write the problem in one sentence.

Then list three alternatives:

Simpler process/fixture change.

Assisted or semi-automatic option.

Full automation.

If you cannot compare those three against the same problem and evidence, the automation decision is not ready.

---

## Closing

EP41 answered:

Should we automate now?

Suppose the answer is yes.

The next danger is a spreadsheet that says:

“Two-year payback.”

Labor savings.

Machine cost.

Done.

That is not enough.

EP42 asks whether the automation investment survives the real lifecycle:

integration, maintenance, yield, utilization, change, downtime and uncertainty.

**Building the Business Case for Automation.**

# End spoken script

## Draft source anchors — not spoken

- W4-S14 — NIST MEP Robotics and Manufacturing Automation.
- W4-S15/S16 — NIST robotic integration and benchmarking.
- W4-S18 — robot accuracy/repeatability distinction.
- Wave 02 — quality/measurement.
- Wave 03 — capacity/economics.
