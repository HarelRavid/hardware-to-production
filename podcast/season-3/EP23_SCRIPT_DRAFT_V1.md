# EP23 Full Script Draft V1 — DFMEA, PFMEA, Control Plans and Quality Gates

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 3 — Build the Factory Before You Need the Factory
source_outline: EP23_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-02/
spoken_normative_standard_claims: NONE
protected_manual_detail: EXCLUDED

## Production note — not spoken

The script uses AIAG only as scoped automotive-method context. It does not teach the current proprietary FMEA or Control Plan forms, steps, scoring logic, Action Priority rules or exact required fields.

# SPOKEN SCRIPT

## Opening

Imagine a production line with a recurring defect.

A connector sometimes fails final communication test.

The team reacts quickly.

They add another visual inspection.

Then they add a second electrical check.

For a few weeks, the defect rate looks better.

Then the same failure comes back.

Why?

Because the team improved detection.

They did not change the mechanism that was damaging the connector.

That distinction is one of the most important ideas in production quality.

A quality system is not a pile of inspections.

It is a chain that starts with a failure you care about and ends with a process that knows how to prevent it, detect it when necessary, react when something changes, and learn when the evidence says the control is not enough.

That is what this episode is about.

Not memorizing FMEA forms.

Not filling a Control Plan because an audit expects a file.

The question is:

**How do we turn what can go wrong into controls that actually change the way the product is built?**

By the end of this episode, I want you to be able to take one real production risk and build a complete Risk-to-Control Chain around it.

---

## 1. Product risk and process risk are related—but they are not the same question

Start with the product.

Suppose our Sentinel Node has an industrial connector.

At the product level, one important failure might be:

The node loses communication in service.

That is a product effect.

Now move into manufacturing.

How could the production system create that condition?

Maybe a connector pin is bent.

Maybe the connector is not fully seated.

Maybe a seal or enclosure feature pushes the connector sideways during closure.

Maybe the supplier dimension is near one edge of tolerance and the assembly fixture adds another small misalignment.

Maybe the electrical connection passes once and becomes intermittent after vibration.

Now we are asking a different question.

Not only:

“How can the product fail?”

But:

“How can the manufacturing process create, fail to prevent, or fail to detect the condition that leads to the failure?”

This is why design-focused and process-focused risk analysis are related without being identical.

The product function gives us the consequence.

The production flow gives us the mechanisms and opportunities where that consequence can be created.

The exact forms and methods vary by industry.

In automotive, FMEA and Control Plan methods are formalized as part of the Core Tools ecosystem.

But the engineering logic is broader than one sector:

**risk must eventually change execution.**

If a risk analysis lives in a spreadsheet and nothing in the design, process, tooling, measurement or reaction changes, then the analysis may be documented—but it is not yet doing much engineering work.

---

## 2. A score is not a control

Risk methods often use some form of prioritization.

That can be useful.

Teams need a way to focus attention.

But this is where quality systems can become dangerously comfortable with numbers.

A team sees a high score.

They debate whether it should be one point higher or lower.

They update the worksheet.

And the actual process remains unchanged.

So I want to give you a rule for this series:

**A score is not a control.**

A score may help you decide where to look.

The engineering question is what the risk changes.

Does it change the design?

Does it change the fixture?

Does it change the process sequence?

Does it create a prevention feature?

Does it add or improve detection?

Does it change a supplier requirement?

Does it create a reaction plan?

Does it change what has to be verified before release?

Those are the decisions that matter.

So instead of starting with a score, start with a chain.

Requirement or function.

Failure effect.

Process step.

Failure mode or mechanism.

Cause.

Prevention.

Detection.

Reaction.

Evidence that the control actually works.

That is the Risk-to-Control Chain we will use in this episode.

It is our listener framework.

It is not a replacement for the method your customer or industry may require.

Its purpose is to stop the paperwork from becoming disconnected from the physics and the process.

---

## 3. Prevention and detection are different jobs

Return to the connector.

Suppose the assembly operation allows the connector to enter at an angle.

The operator can still force the enclosure closed.

The pin bends.

Final test catches many of the damaged units.

One response is to add another final test.

That may reduce escapes.

But it does not reduce the number of connectors being damaged.

A prevention response might be different.

Change the geometry so the connector cannot enter at the wrong angle.

Add a positive datum.

Use a fixture that removes lateral freedom.

Change the assembly sequence.

Improve access so the operator is not pushing blind.

Those actions attack the mechanism.

Detection still matters.

Some failure modes cannot be completely prevented.

Some risks justify layered controls.

But the point is to know which job each control is doing.

A detection control answers:

“Can we find the bad state before it escapes?”

A prevention control answers:

“Can we make the bad state less likely to happen?”

They are not interchangeable.

And neither one should be added automatically.

There are cases where downstream test is the practical control.

There are cases where physical error-proofing is far stronger.

There are cases where the right answer is redesign.

There are cases where the risk is low enough that simple inspection is completely reasonable.

The control has to fit the mechanism, consequence and maturity of the process.

---

## 4. The Control Plan is where the risk meets production

Once the important risks are understood, the next question is operational.

What does production actually do?

This is where a Control Plan becomes useful.

In automotive quality practice, Control Plans are formal tools connected to product-quality and process planning.

But for this episode, I want to stay at the engineering level and avoid turning it into a form-filling lesson.

Think of the Control Plan as the execution layer.

For an important process characteristic or control objective, production needs to know things like:

What are we controlling?

Where in the process?

How?

With what method or equipment?

How often?

Who owns the action?

And what happens if the control says something is wrong?

That last question matters more than many teams realize.

A check without a reaction is not a complete control.

If the gauge says the process is abnormal, what happens to the machine?

What happens to the parts already produced?

Where is the last-known-good boundary?

Who has authority to restart?

What evidence is needed before release?

A good quality gate does not merely say “inspect here.”

It defines a decision.

---

## 5. The measurement method is part of the control

Now the connector process gets more interesting.

Suppose we decide connector seating depth is important.

We add a depth measurement.

We define a target and limits.

We collect data.

It looks very professional.

But there is a hidden question.

Can we trust the measurement system enough for the decision we are making?

Maybe the gauge is calibrated.

That is good.

But perhaps the contact point is inconsistent.

Maybe the operator can tilt the gauge.

Maybe one fixture supports the enclosure differently from another.

Maybe temperature matters.

Maybe the measurement software rounds the value.

Maybe different operators produce different results.

This is why measurement adequacy sits inside the quality chain.

The control is not stronger than the evidence it uses.

We will go deep into that in Episode 24.

For now, remember the dependency:

Risk says what matters.

The control defines what the process will do.

Measurement tells you what state the process or product appears to be in.

If the measurement is weak, the reaction can be wrong.

You can reject good parts.

Accept bad parts.

Adjust a stable process unnecessarily.

Or calculate capability from variation that partly belongs to the measurement system.

So measurement is not an afterthought.

It is part of control architecture.

---

## 6. Build a real reaction plan

Let's complete the connector example.

Suppose we add a controlled assembly fixture and a seating measurement.

During production, the seating result crosses the reaction threshold.

What now?

A useful reaction might include:

First, stop or contain the affected process as appropriate.

Second, identify the affected work-in-process and the last-known-good boundary.

Third, verify the measurement method. We do not want to tear apart the process because the gauge shifted.

Fourth, inspect the fixture, setup, material and process state.

Fifth, correct the cause.

Sixth, verify the process is restored.

Seventh, disposition the affected product based on evidence and risk.

Eighth, ask whether the PFMEA-style risk analysis, control plan, maintenance plan or work instruction needs to change.

Notice what happened.

The reaction is not just:

“Operator finds defect. Quality decides disposition.”

The reaction closes the loop back into the system that created the defect.

That is the difference between containment and learning.

Containment protects the customer now.

Learning changes the probability that the same mechanism returns later.

You need both.

---

## 7. Not every characteristic deserves the same control burden

Another common mistake is taking a quality method and applying the same control intensity everywhere.

Every dimension becomes critical.

Every operation gets a large inspection plan.

Every line on the drawing becomes a data-collection project.

That can make the system slower without making it safer.

The control burden should follow the product claim, failure consequence, process dependence and evidence need.

If a characteristic has little effect on function, safety, fit, reliability, downstream process behavior or customer requirement, it may not deserve the same control architecture as a seal compression dimension or safety-critical weld.

This does not mean “ignore noncritical requirements.”

It means use engineering judgment.

The real quality system is selective.

It focuses attention where variation can change the outcome.

---

## 8. A note on RPN, Action Priority and quality-method terminology

If you work in automotive or another environment with a formal FMEA method, you may use defined prioritization logic.

That method matters when it is contractually or organizationally required.

But I want to keep one boundary very clear.

In this podcast, I am not going to teach a proprietary scoring method from memory.

And I do not want you to leave this episode thinking that one prioritization number is the engineering conclusion.

Whatever method your sector uses, come back to the same practical question:

**Did the important risk change the process?**

If the answer is no, the analysis is not finished.

---

## 9. Sentinel Node — the complete Risk-to-Control Chain

Let's run the full chain once.

Product function:

Sentinel Node must maintain reliable communication in the installed environment.

Failure effect:

Intermittent or lost communication.

Production step:

Connector installation during enclosure assembly.

Potential mechanism:

Angular misalignment and side loading during insertion.

Potential causes:

Fixture freedom.

Poor visibility.

Operator technique.

Connector variation.

Sequence interaction with the enclosure.

Prevention:

Positive alignment feature in the fixture.

Assembly geometry that constrains orientation.

Improved access.

Possibly a design change if the interface itself is too fragile.

Detection:

Defined seating confirmation.

Potentially a controlled seating-depth measurement.

Final communication test.

Reaction:

Contain the affected population.

Verify measurement and fixture state.

Correct the process.

Recheck affected parts.

Verify restored process behavior.

Update controls if needed.

Effectiveness evidence:

Does the failure rate stay down?

Does the process remain stable?

Does the same mechanism disappear from NCR/rework/field data?

Now the quality system is not a document.

It is a chain from product function to process behavior and back to evidence.

---

## 10. What changes from DEV to LVP to serial production?

In early development, you do not need a mature production FMEA and control-plan bureaucracy for every bench experiment.

You do need to notice important failure mechanisms.

A lightweight risk register may be enough.

You can ask:

What can fail?

What would matter?

What should the next prototype teach us?

As you enter low-volume production, the situation changes.

Multiple people build the product.

The process repeats.

Suppliers become involved.

The same failure can recur.

Now control needs to become explicit.

What are the critical steps?

What is prevented?

What is detected?

What is measured?

What is the reaction?

As you move toward serial production, the burden grows again.

The system must survive more operators, more shifts, more supplier lots, more maintenance, more changes and more time.

Controls need to remain connected to real risks.

Measurements need to remain adequate.

Reaction plans need to work at scale.

And the quality system has to learn from actual production evidence rather than preserve the version of the risk analysis that existed before production started.

---

## 11. Six traps to avoid

Trap one:

**FMEA equals spreadsheet.**

No. The value is in the engineering decisions the risk analysis changes.

Trap two:

**High score means one automatic action.**

No. Prioritization helps focus. The engineering response still depends on mechanism and consequence.

Trap three:

**Final test equals prevention.**

It does not. Final test may be excellent detection. Know which job it is doing.

Trap four:

**Control Plan duplicates the FMEA.**

It should operationalize selected controls in production. If the two drift apart, the process is telling a different story from the risk analysis.

Trap five:

**Every characteristic needs equal control.**

It does not. Control intensity should follow consequence and dependence.

Trap six:

**The audit passed, therefore the risk is controlled.**

An audit can show that a system or document exists.

The process evidence has to show that the control actually works.

---

## 12. The action after this episode

Do one thing.

Take the most painful recurring defect from your last build.

Not the most complicated one.

The one everyone recognizes.

Write the full Risk-to-Control Chain.

What function or requirement is affected?

What is the failure effect?

At which process step is the condition created?

What is the real mechanism or cause?

What prevents it?

What detects it?

What measurement or evidence supports the decision?

What is the reaction if the control fails?

How will you know the corrective action was effective?

If any link is blank, that is where the engineering conversation starts.

---

## Closing

Episode 23 answered:

What needs to be controlled?

But the next question can break the entire chain.

What if the measurement itself is noisy?

What if two operators measure the same part differently?

What if a calibrated instrument is mounted in a fixture that introduces more variation than the process?

What if the test gives us a crisp PASS/FAIL and we have no idea how trustworthy the decision is?

That is Episode 24.

**Production Testing and Measurement-System Capability.**

Because before we calculate process capability, we need to know whether the measurement system is telling us the truth we think it is telling us.

# End spoken script

## Draft source anchors — not spoken

- W2-S01 — AIAG Quality Core Tools public overview.
- W2-S03 — AIAG Control Plan public identity/high-level relationship to APQP.
- W2-S07 — NIST/SEMATECH Measurement Process Characterization.
- W2-S09 — NIST measuring-system characterization/traceability.
- Exact AIAG/VDA FMEA and Control Plan method detail intentionally excluded pending licensed review.
