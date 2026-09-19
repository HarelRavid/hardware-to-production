# EP24 Full Script Draft V1 — Production Testing and Measurement-System Capability

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 3 — Build the Factory Before You Need the Factory
source_outline: EP24_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-02/
spoken_normative_standard_claims: NONE
protected_manual_detail: EXCLUDED

## Production note — not spoken

The script uses NIST as the primary open technical source for measurement-process concepts. AIAG MSA remains method context only; no proprietary study design or universal acceptance threshold is narrated.

# SPOKEN SCRIPT

## Opening

Picture this.

Two production stations test the same product.

Station A says PASS.

Station B says FAIL.

The team reacts exactly the way many teams react.

They start blaming the process.

Maybe assembly is unstable.
Maybe the supplier is drifting.
Maybe the product is too sensitive.
Maybe the operator is making mistakes.

So they start adjusting things.

Fixture settings change.
Process parameters move.
A supplier gets called.
A technician retunes the station.

But then somebody asks a more basic question:

What if the product is not changing as much as the measurement?

That question is uncomfortable because production data often arrive with an aura of certainty.

The display shows 5.02.

The software says PASS.

The gauge has a calibration sticker.

The database has a timestamp.

It looks objective.

But a measurement result is not just the product.

It is the product interacting with a measurement system.

And that system can include the instrument, fixture, operator, method, software, reference artifact, environment and time.

So this episode asks one question:

**Can we trust the measurement enough for the decision we are using it to make?**

Not “is the instrument calibrated?”

Not “does the test station work?”

The decision.

That is the level that matters.

---

## 1. The measurement system is bigger than the instrument

Suppose we are measuring connector seating depth on the Sentinel Node.

The instrument is a depth gauge.

Easy.

But how is the enclosure located?

Where does the gauge touch?

How much force is applied?

Can the operator tilt it?

Does the plastic surface deform?

Is the fixture worn?

Does temperature matter?

Does the software round the result?

Does a different operator use a slightly different contact point?

Is the reference zero checked the same way every shift?

All of those can influence the number.

This is why NIST talks about characterizing measurement processes in terms such as repeatability, reproducibility and stability.

The key idea is simple:

**Observed variation can come from the thing you are measuring and from the system doing the measuring.**

If we do not understand that split, we can react to measurement noise as if it were product variation.

Or worse, we can miss product variation because the measurement method is too weak to resolve it.

---

## 2. Repeatability and reproducibility are different questions

These two words are often used loosely.

Let's keep them practical.

Repeatability asks:

If we measure the same thing again under the same conditions, how consistent are the results?

Same method.
Same instrument.
Same operator.
Same location.
Short time interval.

Reproducibility asks:

What happens when relevant measurement conditions change?

Different operator.

Different instrument.

Different location.

Different setup.

Different time.

The changed condition needs to be named.

This matters because a method can look repeatable in one engineer's hands and become inconsistent when production operators use it across three shifts.

Or two stations can each be internally repeatable and still disagree with each other.

So when somebody says:

“Our gauge study looks good.”

Ask:

Good under which conditions?

That question is not bureaucracy.

It is the applicability statement for the measurement evidence.

---

## 3. Calibration is important—but it does not answer every question

This is another area where language matters.

Calibration is important.

In many contexts it is essential.

But calibration and production decision capability are not the same question.

A calibrated gauge can still be used badly.

Imagine the instrument itself is accurate against a reference.

But the part is located inconsistently.

The contact point changes.

The operator force changes.

The fixture flexes.

The measurement software applies the wrong offset.

The gauge can be calibrated and the measurement process can still produce poor decisions.

So instead of asking only:

“Is the gauge calibrated?”

Ask:

**Is the complete measurement method adequate for the decision?**

That includes calibration where relevant.

But it also includes the geometry, procedure, operator, fixture, data handling and environmental conditions that influence the result.

---

## 4. Adequate for what?

Measurement quality is not an abstract score.

It depends on what decision you are making.

Suppose a measurement method resolves to 0.1 millimeter.

For a rough screening decision with a tolerance several millimeters wide, that might be completely reasonable.

For a critical feature where the accept/reject boundary is only a few hundredths of a millimeter away, it may be useless.

Same instrument.

Different decision.

That is why I do not want this episode to give you one universal ratio or percentage and say:

“Below this number your measurement system is good.”

Real measurement decisions depend on consequence, tolerance, process variation, method, uncertainty and the type of conclusion being made.

The better question is:

**What wrong decision could this measurement cause?**

Could it reject a good unit?

Could it accept a bad unit?

Could it make a stable process look unstable?

Could it make an unstable process look stable?

Could it hide a supplier shift?

Could it make two production sites incomparable?

That is the engineering problem.

---

## 5. The golden unit trap

Many production teams use a golden unit or reference unit.

This can be useful.

A controlled reference product can help detect whether a station has drifted or changed.

But be careful with the language.

A golden unit is not automatically a calibration standard.

Those are different concepts.

If you use a reference unit, define what makes it useful.

What exact unit is it?

What configuration?

How is it stored?

What response is expected?

What tolerance around that response is meaningful?

How often is it checked?

What happens if the reference unit itself changes, ages or is damaged?

A reference unit can become another uncontrolled source of truth if nobody controls the reference.

So treat it as an engineering artifact with identity and history.

---

## 6. Test software and fixtures are part of configuration

Now connect this episode back to configuration management.

Suppose the physical product does not change.

But the test fixture changes.

Or the software algorithm changes.

Or the acceptance limit changes.

Or the calibration file changes.

Can the old results be compared directly to the new results?

Maybe.

Maybe not.

The point is that measurement evidence has configuration too.

A result should be interpretable relative to the method that generated it.

That means the relevant instrument, fixture, software, procedure and reference state may need identity.

You do not need to log every meaningless detail.

But if a change can alter the engineering conclusion, the change belongs in the evidence story.

---

## 7. Retest does not erase the first result

Here is a common production pattern.

Unit fails.

Operator adjusts something.

Unit passes.

Database stores PASS.

Production moves on.

The problem is not that retest is always wrong.

Retest can be perfectly legitimate.

The problem is erasing the path.

If the original failure matters to understanding the product, process or measurement system, it needs to remain visible.

Why did the unit fail?

Was the first result measurement error?

Was the fixture reseated?

Was the product reworked?

Was firmware restarted?

Was the acceptance method changed?

A final PASS is the final state.

It is not the whole history.

And that history can be where the useful engineering signal lives.

---

## 8. Sentinel Node — a simple measurement-system study

Let's make this concrete.

Our Sentinel Node has a connector seating-depth characteristic.

For the teaching example, imagine ten representative parts across the process range.

Three operators measure the same parts.

Each repeats the measurement.

The method is a manual depth gauge.

The pattern shows two things.

First, repeated measurements on the same part differ noticeably.

Second, one operator tends to read slightly higher than another.

Do we immediately calculate a universal acceptance percentage?

No.

The point is simpler.

The observed production number contains a meaningful measurement contribution.

So before we use those numbers for strong process-capability conclusions, we improve the measurement method.

We add a hard datum.

Control gauge orientation.

Use more consistent contact force.

Write the method clearly.

Train the operators.

Use a controlled check artifact.

Then repeat the study.

Notice the sequence.

We did not start by blaming the operators.

We improved the measurement architecture.

That is the same mindset we used in DFA and mistake-proofing.

When variation matters, look at system design before reaching for blame.

---

## 9. The Measurement Decision Chain

Here is the listener tool for this episode.

Start with the claim or CTQ.

What are we trying to decide?

Then:

What is the measurement method?

What instrument and fixture are involved?

What reference or calibration state matters?

What repeatability, reproducibility or stability behavior matters?

What is the acceptance rule?

What happens when the result is near the boundary?

What is the reaction?

How is the data tied to the unit, station, method and version?

What change would require us to reassess the method?

That is the Measurement Decision Chain.

It forces the test to answer an engineering question instead of merely produce a number.

---

## 10. DEV to LVP to serial production

In early development, a sophisticated measurement system is often unnecessary.

An engineering instrument may be completely adequate for learning.

The important thing is knowing its limitations.

As you move into low-volume production, the burden changes.

Multiple operators.

Repeated units.

Supplier lots.

Acceptance decisions.

Now you need repeatable fixtures, defined methods and enough evidence to trust the decisions.

By serial production, measurement becomes infrastructure.

Calibration.

Maintenance.

Software versions.

Station-to-station comparability.

Reference artifacts.

Automated data.

Change control.

Recovery after station failure.

The measurement system has to survive time, rate and change without silently changing the meaning of PASS.

---

## 11. Six traps to avoid

Trap one:

**Calibrated means capable.**

Calibration can be necessary and still not answer the whole production-decision question.

Trap two:

**Digital means objective.**

A digital display can report a very precise number from a weak method.

Trap three:

**Golden unit means calibration standard.**

Not automatically.

Trap four:

**One GR&R percentage tells us whether every measurement system is acceptable.**

Context matters.

Trap five:

**Tighter test limits always make quality better.**

If the measurement system cannot support the tighter discrimination, you may only create false rejects or confusing retest behavior.

Trap six:

**The final PASS is the only result that matters.**

Sometimes the first failure is the most useful piece of evidence in the record.

---

## 12. The action after this episode

Choose one production measurement that directly drives accept or reject.

Ask three people who use or depend on it to explain:

Where is the part located?

Where is the measurement taken?

What could move the result?

What is the reference?

What happens if the station changes?

What happens if the result is near the limit?

If the three answers are materially different, do not start by buying a better instrument.

Start by defining the measurement system.

---

## Closing

Episode 23 told us what the process needs to control.

Episode 24 tells us whether we can trust the measurement used to control it.

Now we are ready for a different question.

Suppose the measurement system is good.

We collect data.

Every part is still inside specification.

But the process is drifting.

Or the process is perfectly stable—but centered in the wrong place.

Or a dashboard gives us one impressive capability number from data that were never stable in the first place.

That is where we go in Episode 32.

**Process Capability, SPC and Knowing Whether Production Is Stable.**

Because a trustworthy measurement is only the beginning.

Next we have to understand the behavior of the process itself.

# End spoken script

## Draft source anchors — not spoken

- W2-S07 — NIST/SEMATECH Engineering Statistics Handbook, Measurement Process Characterization.
- W2-S08 — NIST repeatability/reproducibility terminology.
- W2-S09 — NIST measuring-system characterization and traceability considerations.
- AIAG MSA-4 — current method-context identity only; proprietary acceptance/study details intentionally excluded.
