# EP32 Full Script Draft V1 — Process Capability, SPC and Knowing Whether Production Is Stable

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 4 — Quality, Suppliers and the Reality of Scale
source_outline: EP32_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-02/
spoken_normative_standard_claims: NONE
protected_manual_detail: EXCLUDED

## Production note — not spoken

NIST is the primary open technical source for capability concepts and Cp/Cpk formulas. The 2026 AIAG/VDA SPC manual is current automotive method context only. This script intentionally avoids customer-specific capability thresholds and proprietary chart rules.

# SPOKEN SCRIPT

## Opening

A production dashboard shows one number.

Cpk: 1.67.

The number is green.

The team is happy.

Quality says the process looks capable.

Operations says the line is healthy.

Management sees no reason to worry.

Then somebody plots the same measurements in the order they were produced.

Halfway through the run, the process clearly shifts.

Nothing in the capability number told the story.

That is the danger of compressing process behavior into one statistic before asking whether the process behavior is stable enough to summarize.

So this episode is about three questions that teams often collapse into one.

First:

Can we trust the measurement?

Second:

Is the process behaving consistently over time?

Third:

If the process is stable enough to characterize, is its spread and centering acceptable relative to the specification?

Those are different questions.

And the order matters.

---

## 1. Start with time, not the spreadsheet summary

Production processes create sequences.

Part 1.
Part 2.
Part 3.
Shift one.
Shift two.
New material lot.
Tool wear.
Maintenance.
Operator change.
Temperature change.
Fixture adjustment.

The order contains information.

If you take all the measurements and collapse them into a mean and standard deviation, you can hide the fact that the process changed during the run.

That is why statistical process control is fundamentally interested in process behavior over time.

We are not just asking:

“How many parts passed?”

We are asking:

“Is this process behaving like the same process?”

That distinction is powerful.

A process can produce all conforming parts today and still be showing a change that should trigger investigation.

And a process can be perfectly stable and consistently produce bad parts because its natural variation or centering is not good enough for the specification.

So conformance, stability and capability are not synonyms.

---

## 2. Specification limits and control limits are not the same thing

This is one of the most important distinctions in quality engineering.

Specification limits come from the product or engineering requirement.

They answer:

What is acceptable for the product?

Maybe a diameter must be between two limits.

Maybe connector seating depth must remain within a functional range.

Maybe a voltage, force, thickness or temperature has an engineering acceptance range.

Those are specification limits.

Process-control limits answer a different question.

They describe the expected behavior of the process under the statistical model being used.

They are based on process data and the charting approach.

They do not become product requirements.

And product specifications do not become control limits.

Why does this matter?

Because a point can be inside specification and still be statistically unusual for the process.

That can be an early warning.

And a process can remain completely inside its own expected behavior while that expected behavior is too wide or badly centered relative to the specification.

That is why we need both views.

---

## 3. Stable does not mean capable

Imagine a machining process that has run for weeks.

No unusual shifts.

No special-cause signals.

Very consistent.

The problem is that the average is too close to the upper specification limit.

Or the variation is simply too wide.

The process is stable.

It is just stably producing too much risk of nonconformance.

That is not a contradiction.

Statistical stability asks whether the process behavior is consistent.

Capability asks whether that behavior fits the engineering specification.

So stability is not the final goal.

It is the condition that makes a capability statement interpretable.

---

## 4. In specification does not mean stable

Now flip the example.

Suppose every unit is still inside specification.

Production reports 100% pass.

But the measurements move upward over time.

5.01.
5.02.
5.04.
5.06.
5.07.
5.08.
5.10.
5.11.
5.12.
5.13.

For our illustrative Sentinel connector-depth example, the specification is 4.80 to 5.20 millimeters.

Every one of those measurements is still in spec.

A simple pass/fail report says:

Everything is good.

But if the process had previously behaved around 5.00 with much less variation, that sequence is telling us the process changed.

Maybe a fixture stop is moving.

Maybe the tool is wearing.

Maybe setup changed.

Maybe the measurement system shifted.

The important thing is that the process is giving us information before the specification is necessarily violated.

That is one of the main reasons SPC exists.

Not to decorate dashboards.

To see process changes while there is still time to understand and react.

---

## 5. Measurement adequacy comes first

Before we trust any of this, remember Episode 24.

If the gauge, fixture, method or operator variation is large enough to distort the process signal, then the chart is partly monitoring the measurement system.

That can create fake signals.

Or hide real ones.

So the chain begins with:

Is the measurement system adequate for this decision?

Only then do we ask whether the process is stable.

Only then do we make strong capability interpretations.

That order is one of the global rules in this series:

**measurement adequacy before capability confidence.**

---

## 6. Cp — spread relative to specification width

Let's introduce the first capability index.

Cp compares the width of the specification with the observed process spread.

Using sample standard deviation, the common formula is:

Cp equals:

USL minus LSL

divided by

six times s.

For the Sentinel example:

USL = 5.20 millimeters.

LSL = 4.80 millimeters.

Observed standard deviation = 0.04 millimeters.

So the specification width is:

0.40 millimeters.

Six times the standard deviation is:

0.24 millimeters.

0.40 divided by 0.24 gives approximately 1.67.

What does that tell us?

It tells us about the relationship between spread and specification width.

It does **not** tell us whether the process is centered.

That is the limitation.

---

## 7. Cpk — include centering

Now suppose the process mean is exactly 5.00.

The process is centered between the two specification limits.

With the same 0.04 standard deviation, Cpk is also approximately 1.67.

Now move the mean to 5.10.

Keep the same standard deviation.

Keep the same specification limits.

What happens?

Cp stays approximately 1.67.

The spread did not change.

But Cpk drops to approximately 0.83 because the process moved closer to the upper specification limit.

That is why Cp and Cpk are related but not identical.

Cp sees spread relative to specification width.

Cpk also responds to off-centering.

These numbers are useful.

But only if the assumptions underneath them are reasonable.

---

## 8. A capability number is conditional evidence

This is where dashboards can become dangerous.

The formula always gives you a number.

Excel does not ask whether the data came from one stable process.

It does not ask whether the measurement system is adequate.

It does not ask whether you mixed multiple tools, cavities, shifts or product variants.

It does not ask whether the distribution model is appropriate.

It does not ask whether your sample is enough for the confidence you need.

The number appears anyway.

So a capability result is not evidence simply because the formula ran successfully.

It is evidence only inside an explicit context.

NIST discusses capability indices with assumptions including stable process behavior and distribution/data considerations.

For the podcast, we will keep the decision rule simple:

Before you trust a capability number, ask:

Can I trust the measurement?

Do I understand the sampling and time order?

Is the process behavior stable enough for this analysis?

Are the distribution/model assumptions reasonable for the data and question?

Is the dataset adequate for the conclusion?

If the answer to those questions is weak, adding more decimals to Cpk does not improve the engineering.

---

## 9. No universal Cpk magic number

You have probably heard thresholds.

1.00.

1.33.

1.67.

2.00.

Different companies, sectors, characteristics, launch phases and customer requirements can use different criteria.

So this episode will not tell you:

“Cpk above X means the process is good.”

That would be too simple.

The correct threshold depends on the applicable customer, risk, characteristic, contract, method and decision context.

The transferable lesson is not the threshold.

The transferable lesson is the sequence:

Measurement.

Stability.

Assumptions.

Capability.

Reaction.

---

## 10. The reaction plan matters more than the dashboard color

Return to the drifting connector-depth process.

The chart gives us a signal.

Now what?

First, contain affected production according to the risk and reaction plan.

Second, verify the measurement system or check artifact.

Third, inspect the fixture and setup.

Fourth, identify the last-known-good boundary.

Fifth, correct the likely special cause.

Sixth, verify that normal process behavior is restored.

Seventh, disposition affected product based on evidence.

Eighth, update the risk/control/maintenance system if the mechanism was not adequately controlled.

That is the important part.

SPC is not a collection of statistical warning lights.

It is a decision-and-reaction system.

A signal with no reaction path is only information.

---

## 11. The Stability vs Capability Review

Here is the listener tool for this episode.

For any CTQ or key characteristic, ask:

One:

Is the measurement adequate?

Two:

Do I have the data in time order?

Three:

Do I understand the sampling or subgroup logic?

Four:

Is the process behaving consistently enough for the intended analysis?

Five:

What are the engineering specification limits?

Six:

How is the process centered?

Seven:

How large is the process variation?

Eight:

Is a capability index appropriate here?

Nine:

What reaction occurs if the process behavior changes?

That is the Stability vs Capability Review.

Use it before showing Cpk on a management slide.

---

## 12. DEV to LVP to serial production

In development, statistical capability may be premature.

You may have too few units.

Too many design changes.

Too much intentional experimentation.

The objective is learning.

As you enter low-volume production, time-order starts becoming useful.

Repeated operators.

Repeated setups.

Supplier lots.

Fixture wear.

Now you can begin seeing the process as a process.

By serial production, selected CTQs may justify sustained statistical monitoring and capability evidence.

But do not turn that into a rule that every variable gets a control chart.

Use statistical control where the characteristic, process and decision justify it.

The purpose is not to maximize statistics.

It is to make production behavior visible.

---

## 13. Six traps to avoid

Trap one:

**High Cpk proves future quality.**

It does not.

It summarizes evidence under assumptions.

Trap two:

**All parts are in spec, so the process is in control.**

Not necessarily.

Trap three:

**Stable means capable.**

No.

A process can be stably wrong.

Trap four:

**Control limits are tolerances.**

They answer different questions.

Trap five:

**One capability threshold works for every customer and characteristic.**

It does not.

Trap six:

**More decimal places mean more confidence.**

Precision in the display does not create validity in the analysis.

---

## 14. The action after this episode

Find one process dashboard that shows yield, Cp, Cpk or another summary statistic.

Then ask:

Can I see the raw measurements in time order?

If not, pull them.

Look for shifts.

Runs.

Tool changes.

Material changes.

Operator changes.

Maintenance.

Anything that says:

“This may not be one stable population.”

Do that before you make the next process decision from the summary number.

---

## Closing

Episode 32 gives us a way to separate measurement trust, process stability and capability.

But sooner or later, the signal is real.

A part is out of specification.

A process changes.

A field return appears.

A supplier escape is found.

Then the question is no longer:

“Is the process stable?”

The question becomes:

“What do we do with the affected product, what do we do with the process, and how do we prove the corrective action actually worked?”

That is Episode 33.

Because closing one defect is not the same as correcting the system that produced it.

# End spoken script

## Draft source anchors — not spoken

- W2-S07/W2-S09 — measurement adequacy prerequisites.
- W2-S10 — NIST/SEMATECH process capability, Cp/Cpk definitions and stable-process framing.
- W2-S04 — AIAG & VDA SPC Manual, 1st Edition, Jul 2026, current automotive method context only.
- Sentinel numerical example is illustrative and arithmetic-verified; it is not field data.
