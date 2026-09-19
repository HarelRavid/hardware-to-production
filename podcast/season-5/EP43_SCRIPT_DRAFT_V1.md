# EP43 Full Script Draft V1 — Semi-Automation, Robotics and Machine Vision

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 5 — Automation, Data and the Connected Factory
source_outline: EP43_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-04/
spoken_normative_standard_claims: NONE
clause_level_robot_safety: EXCLUDED

## Production note — not spoken

ISO 10218-1/-2 current public scope and NIST task-based HRC/robotics research support the safety and integration boundaries. No clause-level robot-safety design instructions are narrated.

# SPOKEN SCRIPT

## Opening

A team wants to automate an assembly operation.

The proposal is a full robotic cell.

Robot.

Vision.

Feeder.

Safety system.

Automatic unloading.

The presentation is impressive.

Then we decompose the work.

The operator does five things.

Picks the part.

Locates it.

Dispenses a controlled amount of material.

Makes one judgment about alignment.

Checks the result.

Only one of those functions is truly repetitive and painful.

A simple fixture plus controlled dispenser may remove most of the problem.

The right automation boundary may be much smaller than the proposed machine.

That is the lesson of this episode.

Automation is not one switch between manual and automatic.

It is a function-allocation problem.

---

## 1. Break the operation into functions

Before choosing technology, break the operation into pieces.

Handling.

Locating.

Transformation.

Verification.

Decision.

For another process:

Feed.

Orient.

Clamp.

Join.

Measure.

Accept/reject.

Recover.

Now ask which functions create the real burden.

High repetition?

Ergonomic risk?

Hazard?

Precision?

Quality variation?

Rate?

Data capture?

Operator judgment?

Once the operation is decomposed, the design space becomes much larger.

You may automate one function and leave four manual.

That can be the best architecture.

---

## 2. Allocate work by the task—not by ideology

People sometimes say:

“Humans are flexible; robots are precise.”

There is truth in that, but it is too simplistic.

Humans can be variable.

Robots can be flexible.

Humans can make consistent skilled judgments.

Robots can fail badly when inputs move outside their model.

So allocate work based on demonstrated task characteristics.

Variability.

Required judgment.

Precision.

Force control.

Hazard.

Ergonomics.

Change frequency.

Sensing difficulty.

Recovery complexity.

Training.

Economics.

The objective is not to maximize machine work.

The objective is a robust production system.

---

## 3. Feeding and fixturing often matter more than the robot

Robotic demos usually show the motion.

The production problem is often part presentation.

Where is the part?

What orientation?

How much variation?

Can it be gripped reliably?

Does the fixture locate it?

What happens when two parts stick together?

What happens when the incoming geometry shifts?

NIST robotic-integration work highlights how custom integration, sensing and constrained environments remain major barriers.

That is why buying the robot is often the easiest part.

The cell is the system.

Feeder.

Fixture.

End effector.

Sensors.

Robot.

Software.

Safety.

Recovery.

All of them determine performance.

---

## 4. Repeatability, accuracy and capability are different

A robot can return to the same programmed position very consistently.

That is repeatability.

NIST explicitly distinguishes repeatability from accuracy.

A robot can repeatedly go to the same wrong point.

And even good accuracy/repeatability does not prove the manufacturing process is capable.

The part varies.

The fixture varies.

The tool deflects.

The process transforms material.

The measurement system contributes variation.

So never take a repeatability specification from a robot brochure and convert it directly into a product tolerance guarantee.

The process has to be demonstrated.

---

## 5. “Cobot” is not a safety conclusion

This is a critical boundary.

ISO 10218 separates industrial robot requirements from industrial robot application/cell integration.

That separation is powerful.

A robot can have safety-rated features.

The application can still create hazards through:

End effector.

Workpiece.

Pinch points.

Stored energy.

Speed.

Task.

Layout.

Recovery.

Human access.

NIST human-robot collaboration research uses a task-based perspective that includes tooling, expected contact and force/pressure transfer.

So the engineering statement is not:

“This cobot is safe.”

It is:

“The integrated task/application has been risk assessed and the required protective measures have been designed and verified for the defined modes.”

The exact standards and legal obligations depend on the machine and jurisdiction.

This episode is not a safety-design tutorial.

It is a reminder that the application is the safety object.

---

## 6. Machine vision begins with optics and the part

A vision problem is not automatically an AI problem.

Before choosing the algorithm, ask:

What feature must be detected?

Is there contrast?

Is the lighting controlled?

Does part pose vary?

Is there occlusion?

What surface finish changes?

What reference truth exists?

What happens if the system falsely accepts a bad part?

What happens if it falsely rejects a good part?

How will calibration and change be controlled?

A brilliant algorithm cannot recover information that the optics never captured.

And an easy vision task can become unstable when lighting, lens position or surface condition drifts.

So vision belongs inside the same measurement-system discipline from Wave 02.

---

## 7. Abnormal states belong in the design

A demo shows the good cycle.

Production lives in the bad cycles too.

Missing part.

Wrong orientation.

Double feed.

Jam.

Ambiguous image.

Lost vacuum.

Sensor disagreement.

Tool wear.

Operator opens the station.

What happens?

Can the cell identify the state?

Can it make safe?

Can the operator recover?

Does the product remain identifiable?

Does restart repeat or skip an operation?

Does a suspect unit get released?

Recovery is a design function.

Not a maintenance afterthought.

---

## 8. The Function Automation Map

Here is the listener tool.

For each process step, list:

Function.

Input variation.

Consequence of error.

Human strengths.

Machine strengths.

Sensing/measurement requirement.

Fixturing/handling.

Candidate automation level.

Abnormal state.

Recovery method.

Evidence needed.

That map lets you automate the painful function without automatically automating the whole operation.

---

## 9. Vision Feasibility Card

For a visual check, record:

Feature.

Contrast.

Lighting.

Pose.

Occlusion.

Surface variation.

Tolerance.

Reference truth.

False-accept consequence.

False-reject consequence.

Calibration/change control.

If half of those fields are unknown, the project may need a sensing experiment before a vision system purchase.

---

## 10. DEV, LVP and SVP

In DEV, automate experiments if it speeds learning.

In LVP, modular assistance and semi-automation often preserve flexibility while improving control.

In SVP, robots and vision can be powerful when interfaces, variation, safety, maintenance and recovery are controlled.

Again:

The maturity is not how much is automated.

The maturity is how much of the production claim is understood and controlled.

---

## 11. Five traps

Robot selection before feeding/fixturing.

Cobot equals safe application.

Vision equals algorithm.

Robot repeatability equals process capability.

Removing operator judgment always improves production.

All false or incomplete.

---

## 12. The action after this episode

Take one operation proposed for automation.

Split it into:

Handling.

Locating.

Transformation.

Verification.

Decision.

Mark the one or two functions causing most of the burden.

Now ask whether those functions alone can be automated or assisted.

That is often where the best architecture appears.

---

## Closing

EP43 chose the automation boundary.

Now we move to one function with unusually high evidence burden.

Test.

Inspection.

Release.

A factory can test 100 percent of units and still make wrong decisions 100 percent automatically.

EP44 asks:

**How do we make automated inspection and end-of-line test trustworthy?**

# End spoken script

## Draft source anchors — not spoken

- W4-S05/S06 — ISO 10218-1/-2 current public scope.
- W4-S17 — NIST task-based human-robot collaboration safety.
- W4-S15/S16 — NIST robotic integration/benchmarking.
- W4-S18 — repeatability vs accuracy.
- Wave 02 measurement-system principles for vision/test.
