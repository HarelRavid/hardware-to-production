# EP42 Full Script Draft V1 — Building the Business Case for Automation

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 5 — Automation, Data and the Connected Factory
source_outline: EP42_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-04/
economics_dependency: evidence/source-lock/wave-03/
spoken_normative_standard_claims: NONE

## Production note — not spoken

This script reuses the Wave 03 NIST investment-analysis lock. It does not introduce a universal hurdle rate, payback target, demand threshold or automation ROI benchmark.

# SPOKEN SCRIPT

## Opening

A vendor proposes an automated cell.

The business case looks excellent.

The cell costs 180,000 dollars.

It removes two operators.

The spreadsheet says payback is less than two years.

Everyone wants to proceed.

Then reality arrives.

Demand is 25 percent lower than forecast.

The product changes.

New tooling and programming are required.

Availability is lower than the quote assumption.

Maintenance needs a specialist.

The operators were reassigned, not eliminated, so the labor saving never became the cash saving in the model.

The original calculation may have been arithmetically correct.

The model was economically incomplete.

That is what this episode is about.

Automation economics is not:

Machine cost divided by labor saving.

It is a lifecycle decision under uncertainty.

---

## 1. Always compare alternatives

Do not evaluate one automation proposal in isolation.

Define the alternatives.

Continue manual.

Improve the fixture.

Add assisted tooling.

Semi-automate.

Fully automate.

Outsource.

Add a parallel station.

Change shift pattern.

Sometimes “do nothing for six months and learn” is a real option.

The business case is not:

“Does this robot have positive ROI?”

The decision is:

“Which feasible production architecture creates the best value for the actual business envelope?”

That prevents a common bias: comparing automation to a deliberately weak manual baseline.

---

## 2. Labor saving is not automatically cash saving

Suppose the automation removes one operator from the station.

What happens to that operator?

Position eliminated?

Reassigned to another constraint?

Needed for loading, inspection or recovery?

Still required during changeovers?

If the headcount does not change, the accounting benefit may be capacity or redeployment rather than direct payroll reduction.

That can still be valuable.

But model the benefit honestly.

A labor-hours saving and a cash saving are not always the same thing.

---

## 3. Build the full cost boundary

The equipment price is one line.

The project may also need:

Integration.

NRE.

Fixtures.

End effectors.

Vision.

Safety equipment.

Installation.

Utilities.

Programming.

FAT/SAT.

Production qualification.

Training.

Spare parts.

Maintenance.

Software licenses.

Vendor support.

Floor space.

Changeover tooling.

Calibration.

Future retooling.

Recovery support.

Cyber/OT integration.

The total economic boundary should match the decision.

Do not compare a full manual operating cost to only the purchase price of an automated machine.

Use the same boundary on every alternative.

---

## 4. Quality benefits must be proven

Automation often promises improved consistency and quality.

That is plausible.

NIST lists consistency, quality and yield among potential benefits of automation depending on application.

But in a business case, potential benefit is not measured benefit.

If the current process has 8 percent rework, do not simply assume automation reduces it to 1 percent.

Show the mechanism.

What variation is removed?

What CTQ becomes more controlled?

What detection improves?

What data support the new yield assumption?

Automation can improve quality.

It can also create new defects through tooling, sensors, recipes, fixturing or software.

The economic model must use evidence, not optimism.

---

## 5. Capacity assumptions come from the production system

A machine quote says 20 seconds per cycle.

Does that mean the line gains 180 units per hour?

No.

EP29 already gave us the rule.

Capacity includes availability, rework, changeover, material supply and the system constraint.

If the automated station is not the bottleneck, improving it may not increase accepted output.

If it is the bottleneck, the gain still depends on sustainable operation.

So the business case should consume the capacity model.

It should not overwrite it with nameplate speed.

---

## 6. Maintenance and downtime are economic inputs

Automation changes the maintenance burden.

Preventive maintenance.

Corrective maintenance.

Spare parts.

Vendor support.

Technician skills.

Calibration.

Software backup.

Downtime.

NIST manufacturing-maintenance research shows that maintenance costs and losses are economically material.

So do not put maintenance in a footnote.

If the cell is economical only when it never fails, the model is not realistic.

---

## 7. Reuse NPV, payback and sensitivity correctly

Wave 03 introduced the investment tools.

Payback asks how long until the initial investment is recovered.

NPV discounts future cash flows into present value.

IRR gives the discount rate at which NPV is zero.

They answer different questions.

No one universal payback or hurdle rate is correct for every company.

What matters here is discipline.

Cash flow over time.

When investment happens.

When savings start.

What additional costs occur.

What happens under downside assumptions.

---

## 8. Staged CapEx preserves option value

Suppose full automation becomes attractive only if volume reaches 40,000 units per year.

Current demand is 8,000.

Forecast says 40,000 in three years.

One option is to buy the full cell now.

Another is to use semi-automation now.

Gain quality and rate improvement.

Learn the product/process.

Preserve cash.

Then invest in dedicated automation when demand and process evidence strengthen.

This is staged CapEx.

It is not universally better.

If a safety requirement or immediate bottleneck demands the large investment now, waiting can be irrational.

But where uncertainty is high, staging buys information before commitment.

That information has value.

---

## 9. Run the downside case

Every hard-to-reverse automation investment should have a downside case.

Demand lower.

Ramp delayed.

Yield below plan.

Availability below plan.

Maintenance above plan.

Product change earlier.

Integration overrun.

Supplier input variation larger.

What happens?

Does the decision remain attractive?

If not, identify which assumption flips it.

That assumption is not a finance detail.

It is engineering or business evidence that deserves work.

---

## 10. The Automation Business Case Sheet

The tool is simple.

Problem/constraint.

Alternatives.

Demand scenarios.

CapEx and NRE.

Operating cost.

Labor model.

Yield/rework.

Accepted throughput.

Maintenance and downtime.

Changeover.

Product-change flexibility.

Support skills.

Residual/redeployability if credible.

Cash-flow timing.

Sensitivity.

Decision.

Full automation.

Semi-automation.

Stage.

Defer.

Reject.

Now the spreadsheet becomes a decision model instead of a sales aid.

---

## 11. DEV, LVP and SVP

In DEV, economics are directional.

Preserve flexibility.

In LVP, use real cycle, yield and intervention data to compare modest automation.

In SVP, larger capital becomes more defensible when demand, uptime, process stability, maintenance and product mix are measured.

Do not automate the forecast.

Automate the demonstrated need when the evidence earns the investment.

---

## 12. Five traps

Operator-hours saved equal cash saved.

Not always.

Machine price equals project cost.

No.

Lowest unit cost equals best investment.

No.

Forecast demand is evidence.

No.

Short payback makes NPV and risk irrelevant.

No.

---

## 13. The action after this episode

Take one automation business case.

Change three assumptions:

Demand minus 25 percent.

Maintenance plus 50 percent.

One major product revision requiring retooling.

Does the decision change?

If yes, those inputs are not spreadsheet details.

They are the evidence priorities before approval.

---

## Closing

EP42 answered whether the automation investment makes economic sense.

Now we still have to design the automation boundary.

Which tasks stay human?

Which get fixtures?

Which get powered assistance?

Which need a robot?

Which need vision?

Which need judgment?

That is EP43:

**Semi-Automation, Robotics and Machine Vision.**

# End spoken script

## Draft source anchors — not spoken

- Wave 03 NIST investment-analysis/economics register.
- W4-S12 — NIST maintenance economics.
- W4-S14 — NIST MEP automation opportunities/business case.
- P2.05 staged-CapEx synthesis.
