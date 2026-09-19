# EP27 Full Script Draft V1 — What a Production Validation Build Must Prove

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 3 — Build the Factory Before You Need the Factory
source_outline: EP27_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-03/
spoken_normative_standard_claims: NONE
universal_PVT_definition: NOT USED

## Production note — not spoken

The episode uses NASA PRR as evidence for production-system readiness categories but does not define one universal PVT phase. Production Validation Evidence Matrix is Hardware-to-Production synthesis.

# SPOKEN SCRIPT

## Opening

The product passes.

Every functional requirement tested in the build passes.

And yet the production-validation build is not successful.

How can both things be true?

Because during the build:

Engineering manually adjusts a fixture every few units.

A supplier shortage forces a substitution.

The production test freezes twice and a developer restarts it.

One operator skips a work-instruction step because the normal tool is unavailable.

Quality accepts several units after extra manual inspection.

The product works.

The production system still depends on rescue.

That distinction is the entire episode.

A production-validation build is not just another product test.

It is an evidence event for the integrated production system.

So the question is not:

“Did the units pass?”

The question is:

**What can the intended production system repeatedly do under the conditions we actually exercised?**

---

## 1. Product verification and production-system evidence are different

Product verification asks whether the product satisfies defined requirements.

Production readiness asks a wider question.

Can the system produce the required product?

With the intended process?

The intended equipment?

The intended people?

The intended suppliers?

The intended inspection and test?

The intended documentation and controls?

Formal production-readiness frameworks make this breadth visible.

NASA's current Production Readiness Review, for example, includes production documentation, production plans, critical process controls, resources, tooling and test equipment, personnel and suppliers.

Again, we are not turning a commercial pilot into a NASA review.

We are using the engineering lesson:

**Production is a system.**

A passing product can come from a weak system.

Validation has to tell us which one we have.

---

## 2. Bound the configuration being evaluated

People often say:

“Freeze the configuration for PVT.”

That can be useful language, but it is too absolute for many real ramp situations.

You may still need controlled changes.

The better rule is:

**Bound and control the configuration being evaluated.**

Which product revision?

Which firmware?

Which process route?

Which tooling?

Which test-software version?

Which supplier sources?

Which approved deviations?

If a change occurs, define its effectivity and separate the evidence.

The objective is not zero change.

The objective is knowing which production state generated each result.

---

## 3. Validate the route, not only the part

A real validation build should exercise the intended route as much as the claim requires.

Production-intent tooling.

Representative fixtures.

Normal work instructions.

Normal material presentation.

Normal inspection and test.

Normal operator roles.

Normal routing.

If a temporary difference remains, state it.

Maybe the final packaging line is not installed.

Maybe one station is still manual.

Maybe a soft tool represents a future hard tool.

That does not automatically make the build useless.

It defines an evidence limit.

The important question is:

Which claims still transfer?

Which claims remain open?

This is the same evidence-envelope logic we have used throughout the series.

---

## 4. Supplier readiness is part of the build

If production depends on purchased parts, supplier readiness is part of production readiness.

Did the parts come from the intended production source?

Same site?

Same process?

Same tooling?

Same sub-tier?

Representative inspection?

Representative lot conditions?

A beautiful supplier sample is not enough if ramp will use a different production route.

This is why supplier approval and production validation cannot be completely separated.

The integrated system includes the external production system too.

---

## 5. Measurement and traceability need to work at the same time

The product may be good while the evidence system is weak.

Can the test station identify the unit and configuration?

Can failed units retain their failure history?

Can we reconstruct which supplier lot was used?

Can the measurement method support the decision?

Does rework remain visible?

Can the genealogy survive the build without engineers manually stitching spreadsheets afterward?

Production validation should test the evidence infrastructure at the same time as the physical process.

Because that infrastructure has to survive ramp too.

---

## 6. Engineering intervention is part of the result

This is where teams can fool themselves.

An engineer helps.

A unit passes.

The result gets reported as PASS.

But the intervention disappears.

Do not do that.

Intervention is not automatically bad.

It can be valuable learning.

Maybe the fixture needs a small improvement.

Maybe the operator instruction is unclear.

Maybe the test station needs a recovery function.

The important thing is to record:

What intervention happened?

Why?

How often?

Who was required?

Would normal production have succeeded without it?

A validation build with high engineering intervention can still be successful as a learning event.

It may simply not support the claim:

“normal production is ready.”

---

## 7. Rate evidence must match the claim

Suppose the team runs at target rate for thirty minutes.

Everything looks good.

Can we declare capacity proven?

Not necessarily.

Was material pre-staged?

Were changeovers excluded?

Was rework deferred?

Were engineers staffing the station?

Did the run end before maintenance or replenishment mattered?

Did WIP accumulate downstream?

A short best-case run can be useful.

But the claim must remain narrow.

“We achieved the target pace for thirty minutes under pre-staged conditions.”

That is honest evidence.

“We demonstrated sustainable production capacity.”

That is a much stronger claim.

Episode 29 will show how to analyze that quantitatively.

For now, the rule is:

**Do not let a stronger conclusion outrun the run that generated it.**

---

## 8. The Production Validation Evidence Matrix

Here is the listener tool.

For every consequential production claim, write:

The claim.

The configuration and process envelope.

The evidence generated.

Any deviation or intervention.

The result.

The open gap.

The consequence of that gap.

The owner.

The release decision.

Example:

Claim:

Normal operators can assemble the connector without damage.

Evidence:

Thirty representative builds using production-intent fixture and work instruction.

Intervention:

Engineer assisted on six units.

Result:

Twenty-four normal builds succeeded; six required help.

Gap:

Fixture access still causes occasional misalignment.

Decision:

Not ready to call normal assembly stable. Correct fixture and repeat focused evidence.

This is a far better outcome than reporting:

“30 units completed.”

---

## 9. Proceed, constrain, or repeat

A validation build does not need one universal PASS/FAIL gate.

Depending on risk and open gaps, the rational decision may be:

Proceed to ramp.

Proceed with a constrained envelope.

Repeat validation after a targeted correction.

Hold production.

The important thing is that the decision is tied to evidence.

If one gap affects only a low-risk packaging operation, it may not block all production.

If the gap affects a critical safety function, measurement validity or configuration control, the consequence is different.

Do not turn every gap into a full stop.

Do not turn every completed batch into a release.

---

## 10. “PVT” is a label, not evidence

Different industries and companies use EVT, DVT, PVT and similar labels differently.

The label can help organize a program.

It is not proof.

Calling a build PVT does not make the process representative.

Calling something a production validation does not make the supplier ready.

Evidence makes the claim.

So whenever somebody says:

“We passed PVT.”

Ask:

What production-system claims were demonstrated?

Under what configuration and conditions?

That question is more useful than debating the label.

---

## 11. DEV to validation to ramp

In DEV, evidence can be narrow.

One prototype.

One claim.

One experiment.

In LVP, more elements begin to operate together.

Operators.

Suppliers.

Tooling.

Test.

Work instructions.

When you reach production validation, the integrated system is the object of evidence.

And during ramp, the question becomes:

Can that system sustain more output without quality, flow, cost or control degrading?

That is the next transition.

---

## 12. Five traps to avoid

Trap one:

Product passes, therefore factory passes.

Trap two:

We called the build PVT, therefore production is ready.

Trap three:

Any engineer intervention invalidates the run.

No. It limits what the run proves.

Trap four:

Supplier samples equal supplier readiness.

Trap five:

Short best-case rate equals sustainable capacity.

---

## 13. The action after this episode

Before your next production-validation build, make one list:

**Expected abnormal support.**

Engineer help.

Extra inspection.

Manual data patching.

Temporary tools.

Pre-staged material.

Supplier expediting.

Anything that will not exist in normal production.

For each one, ask:

What claim becomes weaker if we need this support?

That list tells you where validation evidence is still immature.

---

## Closing

Episode 27 asks whether the production system works as an integrated system.

But the next thing that happens in real factories is more subtle.

Units fail.

They get adjusted.

Opened.

Reworked.

Retested.

Eventually they pass.

And a dashboard reports excellent final yield.

So Episode 28 asks:

**How much output passed the first time—and how much of the factory is actually rescue?**

Yield, Rework, Scrap and the Learning Curve.

# End spoken script

## Draft source anchors — not spoken

- W3-S02 — NASA NPR 7123.1D Appendix G PRR.
- W3-S03 — NASA Systems Engineering Handbook PRR definition.
- Wave 02 — supplier / measurement / quality evidence.
- Wave 01 — configuration / effectivity / intervention history.
