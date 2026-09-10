# A7 Full Script Draft V1 — Verification Planning Before DVT/PVT Thinking

status: FULL SCRIPT DRAFT V1 — EDITORIAL/TECHNICAL SCRIPT REVIEW NEXT
season: Season 1 — Build the Right Hardware Before Production Finds Your Mistakes
source_outline: `A7_SCRIPT_OUTLINE.md`
source_lock: `evidence/source-lock/wave-01/`
spoken_standard_claims: NONE PLANNED
real_case_claims: NONE — opening and Sentinel examples are illustrative

# SPOKEN SCRIPT

## Opening

Imagine your team has just finished three weeks of environmental testing.

The reports look good.
The graphs look good.
Most of the boxes say PASS.

A few months later, somebody preparing for production asks a very simple question:

Which exact product did we test?

Was the enclosure the final revision?
Was the firmware the same build we are releasing now?
Was the gasket production intent?
Which connector was installed?
What environmental profile did we actually run?
What was the acceptance criterion before the test started?
And what decision was this test supposed to support?

Now the room gets quiet.

The team remembers doing the work.
It remembers the chamber.
It remembers the long nights.
It remembers that the unit passed.

But it cannot reconstruct the evidence cleanly enough to know how far that PASS can actually be trusted.

This is a very important distinction in hardware development:

**Testing is activity. Verification is evidence.**

A lot of test activity can still produce weak evidence if the claim, configuration, conditions, method and decision are not connected.

By the end of this episode, I want you to be able to take the next consequential test your team is planning and write one page before the test begins: a Verification Intent Sheet.

Not a fifty-page qualification plan.
One page that answers one question:

**If this test passes, what exactly will we be justified in saying afterward?**

---

## 1. Exploration, verification and validation are not the same question

Hardware teams use the word “test” for almost everything.

That is fine in conversation, but it hides several different jobs.

Sometimes you test because you are exploring.

You change a resistor.
You move a sensor.
You increase the load until something strange happens.
You run a thermal camera and look for hotspots.

The purpose is learning.
You may not even know what the final acceptance criterion should be yet.

Sometimes you test because you are verifying a requirement.

Now the question is more specific:
Did this defined product, under these defined conditions, satisfy this defined requirement using this defined method?

And sometimes you are asking a validation question:
Does the product actually satisfy the intended use and stakeholder need in the environment where it matters?

Those questions overlap, but they are not interchangeable.

Validation is not just “the really serious test at the end.”
Verification is not simply “anything measured in a lab.”

For this episode, we are going to focus on verification evidence — and on how early teams can begin building good verification habits without turning DEV into a certification program.

---

## 2. Start with the claim, not the test machine

A common planning pattern sounds like this:

“We have access to the vibration table next Thursday. What tests should we run?”

That is backwards.

The machine is not the question.

Start with the claim.

What are you trying to prove, learn or decide?

Maybe the requirement is that an enclosure remains functional after a defined vibration exposure.

Maybe the claim is that a mounting interface does not shift enough to corrupt sensor data.

Maybe the question is whether a connector remains seated under a representative load profile.

Those are different claims.
They may use the same test machine, but they do not automatically need the same article, instrumentation, conditions or acceptance logic.

So the first line on the Verification Intent Sheet is:

**Claim or requirement.**

The second line is:

**Decision.**

What will change depending on the result?

Will we release a design?
Choose a material?
Approve a supplier?
Proceed to the next prototype?
Change an interface?
Or are we simply learning enough to design the next experiment?

If there is no decision connected to the result, you should at least ask why you are spending the time and money to generate it.

---

## 3. The verification chain

For a consequential test, I want you to walk through a simple chain.

Claim.
Decision.
Article.
Configuration.
Conditions.
Method.
Measurement.
Criterion.
Result.
Applicability.
Retest trigger.

Let's slow that down.

**Claim:** what are we trying to know?

**Decision:** what will the evidence be used for?

**Article:** which physical unit, sample or assembly are we testing?

**Configuration:** which hardware revision, firmware, material, supplier state, calibration state or process version matters to this claim?

**Conditions:** load, environment, duty cycle, operating state, preconditioning — whatever changes the meaning of the result.

**Method:** what exactly are we doing?

**Measurement:** is the measurement method good enough to support the conclusion?

**Criterion:** if this is a true pass/fail verification, what counts as success or failure?

**Result:** what actually happened, including anomalies and deviations?

**Applicability:** what exact claim and configuration does the result support?

And finally:

**Retest trigger:** what future change would make us question whether this evidence still applies?

That last field is one of the most valuable habits you can develop.

Because the problem is rarely that an engineering team has no test data.

The problem is that six months later, nobody knows whether old data still applies to the product that now exists.

---

## 4. Verification planning starts before DVT

Many hardware teams first become serious about verification when somebody says, “We are approaching DVT.”

But if you wait until then to ask how important requirements will be demonstrated, you can discover problems that are expensive to fix.

Maybe the requirement cannot actually be measured in the final geometry.

Maybe the interface you need to instrument is no longer accessible.

Maybe the acceptance statement is so vague that two engineers interpret it differently.

Maybe the final use condition cannot be reproduced by the test setup you assumed.

Maybe the prototype technology you selected is not representative of the failure mechanism you now need to verify.

You do not need a final formal test procedure while the architecture is still moving.

But for important requirements, you should be able to answer:

**What kind of evidence could eventually convince us this is true?**

That question belongs surprisingly early in development.

It improves the requirement.
It can improve the architecture.
And it prevents “we will figure out how to test it later” from becoming a late redesign.

---

## 5. Representative for what?

We discussed prototype representativeness earlier in this season, and it becomes critical here.

A prototype is not simply representative or non-representative.

It is representative **for a claim**.

Suppose you have a 3D-printed enclosure.

It may be perfectly useful for checking:
- connector access;
- installation clearance;
- cable routing;
- user interaction;
- rough packaging geometry.

But the same enclosure may be weak evidence for:
- molded-part warpage;
- production sealing behavior;
- long-term material aging;
- final surface durability;
- production tolerance distribution.

So before reusing a test result, ask:

What characteristic made the test article representative for the claim?

And what characteristic was still only a prototype shortcut?

This is why saying “we already tested that” is not enough.

The right question is:

**What exactly did we test, and for which claim was that configuration representative?**

---

## 6. Measurement can be precise and still be inadequate

Here is another trap.

A display shows 12.347.

It looks scientific.
It looks precise.

But does the measurement system actually support the decision you are making?

If the tolerance band is tiny and the instrument cannot resolve the relevant difference, extra decimal places do not create confidence.

If you are measuring temperature at one point while the failure mechanism depends on a thermal gradient somewhere else, the number may be accurate and still answer the wrong question.

If production-test noise is similar to the distance between good and bad product behavior, a clean pass/fail threshold can hide a weak measurement system.

We are not going to teach full Measurement System Analysis here. That deserves its own treatment later.

For now, keep one rule:

**Before trusting a strong conclusion, ask whether the measurement method is adequate for that conclusion.**

A precise-looking number is not evidence by itself.

---

## 7. Decide the criterion before the result — when it is a pass/fail test

There is an uncomfortable temptation in development.

You run the test.
You see the result.
And then you decide what “good enough” means.

Sometimes that is legitimate — because the test was exploratory.
You were characterizing behavior and learning what the design can do.

But if the test is intended to make a true verification or release decision, the acceptance logic should be defined before you interpret the result.

Otherwise the criterion can quietly move to fit the data.

So label the purpose honestly.

If it is an experiment, call it an experiment.

If it is characterization, let the output inform the model or target.

If it is a pass/fail verification, define what pass and fail mean before the result arrives.

The paperwork is not the point.

The point is protecting the decision from hindsight.

---

## 8. What can one passing unit prove?

You will often hear two extreme statements.

“One unit passed, so the design is proven.”

Or the opposite:

“One unit means nothing.”

Both are too simple.

One unit can sometimes provide valid evidence for a specific deterministic requirement on that configuration.

If you need to verify that a connector physically clears a defined envelope, one correctly configured article may answer that question.

If you need to verify a specific logical function under a defined state, one article may be enough for that claim depending on the method and risk.

But one passing unit does **not** automatically tell you about population variation.

It does not prove process capability.

It does not prove supplier consistency.

It does not prove long-term reliability.

It does not prove that hundreds of production units will behave the same way.

So the useful question is not:

“How many units is enough?”

The useful question is:

**What claim are we trying to support, and what evidence does that claim actually require?**

That distinction will become much more important when we reach production quality and statistics.

---

## 9. Change does not automatically mean retest everything

Now suppose the product changes.

A connector changes supplier.
A gasket material changes.
Firmware changes the calibration algorithm.
The PCB layout changes.
The enclosure moves from CNC machining to molding.

What happens to the old evidence?

There are two lazy answers.

The first is:
“Retest everything.”

The second is:
“It is a small change. No need to retest.”

Neither answer starts from engineering.

Start with the dependency.

What previous claim are we relying on?

What characteristics or assumptions made the old evidence valid?

Which of those did the change touch?

If the change affects the mechanism, interface, material, condition, software behavior or measurement on which the evidence depends, you may need new evidence.

If it genuinely does not affect a claim, repeating every historical test may add cost without adding knowledge.

This impact-based approach is something we will use repeatedly throughout the series.

But be careful with the wording.

It is not a magic formula that tells you the answer automatically.

It is a disciplined way to ask what old evidence still applies and what no longer does.

---

## 10. Sentinel Node: from useful learning to defensible verification

Let's use the Sentinel Node again.

The claim is:

The enclosure and connector system must maintain the required function after the intended wet environmental exposure.

Early in development, the team runs a quick exposure test.

The enclosure is 3D printed.
The connector is a prototype choice.
The gasket is hand cut.
Assembly is done by the engineer.

The test finds two likely ingress paths.

That is valuable evidence.

It teaches the team where the design is weak.

Now fast-forward.

The product has a production-intent enclosure material.
A defined gasket.
A selected connector.
A controlled fastener strategy.
A more representative assembly process.

Can we simply reuse the early PASS or FAIL as final release evidence?

No — not for every claim.

The early test may still tell us something about geometry or a known weak interface.

But the final sealing claim depends on the production-intent configuration.

So now fill out the Verification Intent Sheet.

Claim:
Maintain required function after the defined environmental exposure.

Decision:
Can this configuration proceed toward release for that environmental claim?

Article:
A production-intent assembly.

Configuration:
Record enclosure revision, gasket specification, connector source/revision, fasteners and assembly process that matter.

Conditions:
Define the relevant exposure and operating state.

Method:
Use the planned environmental procedure.

Measurement:
Define how ingress or functional degradation is detected and whether the method is adequate.

Criterion:
Set before the run if this is a pass/fail verification.

Result:
Capture pass, fail, anomalies and any rework.

Applicability:
This result supports this sealing/function claim for this demonstrated configuration and conditions.

Retest trigger:
Changes to gasket, enclosure process/geometry, connector, assembly compression or other relevant interfaces require an impact assessment.

That one page changes the nature of the test.

The chamber did not become more sophisticated.

The evidence did.

---

## 11. DEV, LVP and serial production

In DEV, rapid exploratory tests are good engineering.

You are trying to learn quickly.
You may change the setup between runs.
You may not have final acceptance criteria.

The discipline is simply to label what the result actually teaches and preserve enough context to avoid overusing it later.

As you move into low-volume production, more tests start supporting release, supplier, calibration, quality and production decisions.

Now controlled articles, procedures, measurement methods, criteria and traceable results become more important.

By serial production, evidence has to survive changes, lots, suppliers, software revisions and a much larger population.

The question is no longer only:

“Did this unit pass?”

It becomes:

“What population and configuration does this evidence support, and what change would force us to look again?”

That is a much stronger way to think about verification maturity than simply collecting more test reports.

---

## 12. The Verification Intent Sheet

Before the next consequential test, write one page.

Claim or requirement.

Decision.

Article.

Configuration.

Representativeness.

Conditions.

Method.

Measurement.

Criterion — or learning objective if the test is exploratory.

Result location.

Applicability.

Retest trigger.

And before you begin, ask one final question:

**If this test passes, what exactly will we be justified in saying afterward?**

If the answer is vague, the test plan probably still is too.

---

## Closing

Good verification is not about making development slower.

It is about making expensive evidence reusable.

It keeps a learning experiment from being mistaken for release evidence.

It keeps one passing article from being mistaken for process capability.

It keeps a test on an old configuration from silently proving a new one.

And it keeps “we tested that already” from ending the engineering conversation before anybody remembers what “that” actually was.

But verification creates one more obligation.

If evidence belongs to a specific product state, you have to preserve that state well enough to reconstruct it later.

Which hardware revision?
Which BOM?
Which firmware?
Which calibration?
Which supplier or material where relevant?
Which rework?

That is A8:

**Configuration Management from Prototype #1.**

Because evidence without configuration identity has a surprisingly short half-life.

# End spoken script

## Draft source anchors — not spoken
- S-W1-03 — NASA Systems Engineering Handbook §5.3 Product Verification.
- S-W1-01/S-W1-02/S-W1-05 — requirements/verification linkage.
- ISO/IEC/IEEE 29148:2018 — show-notes/current-standard context only if retained.

## Draft production flags
- No real case is implied.
- No clause-level ISO claim is spoken.
- Verification/validation distinction must remain technically exact.
- No universal sample-size or MSA threshold appears.
- Sentinel Node is fictional.
