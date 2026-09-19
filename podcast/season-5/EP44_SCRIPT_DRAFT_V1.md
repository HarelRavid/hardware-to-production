# EP44 Full Script Draft V1 — Automated Inspection and End-of-Line Test

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 5 — Automation, Data and the Connected Factory
source_outline: EP44_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-04/
measurement_dependency: Wave 02
spoken_normative_standard_claims: NONE

## Production note — not spoken

EP44 applies Wave 02 measurement-system discipline to automated inspection/test. No universal GR&R, guard-band, uncertainty-ratio, false-accept/fail or calibration-interval threshold is introduced.

# SPOKEN SCRIPT

## Opening

A factory tests every unit automatically.

One hundred percent coverage.

The dashboard shows 99.8 percent pass.

It looks like strong control.

Then a fixture contact begins to degrade.

Good units start failing intermittently.

Operators retest them.

Most pass on the second attempt.

A few weeks later, someone changes a software threshold to reduce false rejects.

Now marginal units start passing.

The factory still has 100 percent automated test coverage.

What it no longer has is trustworthy decision integrity.

That is the central lesson.

Automation does not turn a test into truth.

An automated test is still a measurement and decision system.

And it has its own failure modes.

---

## 1. Start from the product claim

Do not start with:

“What can the tester measure?”

Start with:

What product claim are we trying to protect?

Which failure mechanism?

What is the consequence of a false accept?

What is the consequence of a false reject?

If the defect cannot be stimulated or observed by the test architecture, 100 percent coverage of the wrong signal does not help.

So map:

Requirement.

Failure mode.

Stimulus.

Response.

Measurement.

Decision.

Reaction.

That keeps the test tied to product evidence.

---

## 2. The Automated Test Evidence Chain

Here is the core chain:

Requirement or CTQ.

Stimulus.

Sensor or measurement.

Fixture/interface.

Reference/calibration.

Algorithm.

Limit version.

Unit result.

Reaction.

Genealogy.

Every link can fail.

A fixture pin wears.

A sensor drifts.

A software filter changes.

A limit file is edited.

A cable adds resistance.

The wrong product recipe loads.

The unit serial is mismatched.

The result can be numerically precise and still belong to the wrong measurement state.

---

## 3. Test systems drift too

We often monitor the production process and forget to monitor the test process.

But test systems have:

Wear.

Calibration drift.

Sensor aging.

Connector damage.

Software updates.

Reference-unit aging.

Environmental effects.

Network/configuration changes.

If test yield changes, ask whether the product changed or the measurement system changed.

This is the same discipline from EP24.

Automation increases repeatability of the test action.

It does not remove the need to understand the test system itself.

---

## 4. Golden units are check artifacts, not magic truth

A golden unit can be useful.

Run it every shift.

See whether the station response changes.

Great.

But the golden unit itself needs identity.

Configuration.

Storage.

Expected response.

History.

It is not automatically a calibration standard.

And one golden unit may not exercise all failure mechanisms or measurement ranges.

So use it for the purpose it can support.

Do not let a familiar artifact silently become the authority for every test claim.

---

## 5. False accepts and false rejects are different risks

An automated test can make two broad classes of wrong decision.

False accept:

A bad or marginal unit passes.

False reject:

A good unit fails.

The costs are different.

False accept can create field/customer risk.

False reject creates rework, scrap, retest, capacity loss and confusion.

The balance depends on the product and the consequence.

This episode will not give one universal guard band or acceptance-statistics rule.

The point is to make the two decision errors visible in the architecture.

---

## 6. Software and limits have effectivity

Imagine the test threshold changes Monday morning.

What happens to:

Units tested Sunday?

Units tested Monday before the change?

Retests?

Historical trend?

Comparison across stations?

If the software or limits can change PASS/FAIL, then version identity matters.

A threshold change is not “just software.”

It changes the evidence process.

So control:

Test software version.

Recipe.

Limit set.

Calibration/reference file.

Fixture revision.

Effectivity.

That is configuration management applied to test.

---

## 7. Retest must not become “test until pass”

Unit fails.

Operator reseats cable.

Passes.

What happened?

Maybe the first fail was a test-fixture problem.

Maybe the product had an intermittent fault.

Maybe the operator changed the product state.

If the system stores only the final PASS, the evidence is lost.

Define retest logic.

When is retest allowed?

What changes before retest?

Which failure history remains?

When does repeated retest trigger containment?

Again, exact rules are application-specific.

The principle is not.

A final result must not rewrite the evidence history.

---

## 8. Test yield is not always process yield

Suppose test pass rate drops.

Could be product quality.

Could be fixture faults.

Could be false rejects.

Could be network failures.

Could be recipe mismatch.

Could be operator loading.

If you call every test failure a product failure, your process yield is contaminated by the test system.

So separate categories where it matters.

Product/process defect.

Test-system fault.

Setup/operator issue.

Retest.

No-fault-found.

That classification improves both quality learning and capacity modeling.

---

## 9. Automated Test Architecture Map

The listener tool captures:

Product claim.

Failure mechanism.

Stimulus.

Measurement.

Fixture/sensor.

Reference/calibration.

Software/limit version.

Decision rule.

False-accept/fail consequence.

Reaction.

Retest rule.

Genealogy.

Change trigger.

If any consequential field has no owner, the automated test is not yet a controlled release system.

---

## 10. Test-System Drift Review

Periodically ask:

Did reference behavior move?

Fixture wear?

Calibration status?

Software or thresholds?

Environment?

Station-to-station correlation?

Retest patterns?

No-fault-found rate?

That review treats the tester as production equipment with its own health state.

---

## 11. DEV, LVP and SVP

DEV test can be flexible and diagnostic.

LVP needs repeatable fixtures, controlled procedures and captured results.

SVP requires test configuration, maintenance, measurement adequacy, change control and genealogy to support release decisions at rate.

The more automated the decision, the more important it is that the evidence chain remains visible.

---

## 12. Six traps

100 percent test equals zero escapes.

Automated equals objective.

Golden unit equals calibration standard.

Threshold edit is software-only.

Retest PASS erases original FAIL.

Test pass rate equals process FPY.

All false or incomplete.

---

## 13. The action after this episode

Take one automated test station.

List every thing that can change PASS/FAIL without changing the product:

Fixture.

Sensor.

Software.

Limits.

Calibration.

Reference artifact.

Environment.

Operator setup.

If those changes are not controlled or visible, your test system has hidden configuration risk.

---

## Closing

EP44 made automated test trustworthy.

Now the question gets bigger.

The machine worked at the integrator.

It passed FAT.

It runs at site.

But can it sustain real production?

What happens during jams?

Sensor faults?

Maintenance?

Recipe errors?

Restart?

And what does the OEE number actually tell us?

That is EP45:

**Automation Qualification, OEE and Maintenance.**

# End spoken script

## Draft source anchors — not spoken

- Wave 02 measurement-system source lock.
- Wave 01 configuration/effectivity.
- W4-S18 robot/equipment accuracy-maintenance context where relevant.
- No universal automated-test statistical threshold used.
