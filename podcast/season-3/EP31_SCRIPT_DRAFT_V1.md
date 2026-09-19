# EP31 Full Script Draft V1 — Engineering Changes During Ramp-Up

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 3 — Build the Factory Before You Need the Factory
source_outline: EP31_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-03/
dependencies: Wave 01 configuration/change + Wave 02 quality/supplier
spoken_normative_standard_claims: NONE

## Production note — not spoken

This episode applies the already source-locked configuration/effectivity/change principles to live ramp conditions. ECO/ECN are used as common practitioner labels only, not as one universal standardized workflow.

# SPOKEN SCRIPT

## Opening

Engineering changes the connector.

The new connector solves a field problem and supply risk.

The BOM is updated.

Drawing is updated.

The change is approved.

So production should now be building the new configuration.

Right?

Not necessarily.

Old connectors are still in stock.

Two work orders are already open.

WIP is sitting between assembly stations.

The fixture was designed around the old connector.

The production test limits assume the old electrical behavior.

One supplier purchase order still references the previous source.

A service kit contains old spares.

Three weeks later, a failure appears.

And nobody can say with confidence whether the unit contains the old connector or the new one.

The engineering change was released.

The production transition was not controlled.

That distinction is the whole episode.

A change during ramp is not a document update.

It is a controlled population transition.

---

## 1. Start with why the change exists

Before changing the BOM, state the reason.

Defect correction?

Supplier shortage?

Cost reduction?

Reliability improvement?

Regulatory issue?

Capacity constraint?

Design improvement?

Why does this matter?

Because the reason tells us which claims are affected.

If the change addresses connector sealing, the evidence burden is different from a color change.

If the change addresses a safety function, the consequence is different from a packaging improvement.

If it is supplier shortage, interchangeability evidence matters.

A change record without a clear reason makes impact assessment much harder.

---

## 2. Product definition is only one layer of change

Engineering often begins with the product definition.

CAD.

Drawing.

BOM.

Firmware.

That is necessary.

But during ramp, the product is already connected to a production system.

So ask what else changes.

Fixture geometry.

Tooling.

Work instruction.

Assembly sequence.

Test software.

Calibration.

Inspection.

Packaging.

Supplier.

Sub-tier.

Material handling.

Service spares.

Training.

ERP or MES definition.

The change can propagate through the factory even when the new component looks physically similar.

That is why a purchasing substitution can become an engineering change.

And why a BOM release is only one part of implementation.

---

## 3. Effectivity answers: which population gets the change?

A revision tells you what definition exists.

Effectivity tells you where it applies.

Maybe the new connector starts at serial number 2501.

Maybe manufacturing order 184.

Maybe after depletion of a specific old lot.

Maybe two sources remain approved in parallel with different firmware/calibration combinations.

The boundary needs to make the population reconstructable.

A date may be enough in some systems.

If every unit after midnight unambiguously gets the new configuration, fine.

But when WIP spans several days, date alone may be too weak.

The point is not “never use date.”

The point is:

**Can we identify the first definitely new unit and the last definitely old unit?**

If not, the effectivity system is incomplete.

---

## 4. Inventory and WIP are engineering objects during change

When the change is released, what happens to:

Old raw material?

Purchased parts in transit?

Open WIP?

Finished goods?

Reworked units?

Service spares?

Do we use them as-is?

Rework them?

Scrap them?

Return them?

Use them under a temporary deviation?

Each choice has technical and economic consequences.

This is why WIP disposition belongs in change control.

If mixed populations remain invisible, later quality and field analysis become much weaker.

A design change can be correct and still create chaos if inventory disposition is unclear.

---

## 5. Re-verification should follow affected evidence

Now the classic question.

Do we need to retest everything?

Maybe not.

Do we need to retest nothing because the change seems minor?

Also maybe not.

The rule we locked earlier is impact-based.

What evidence did the old configuration support?

Which assumptions made that evidence valid?

Which assumptions changed?

If the connector changes, maybe:

Mechanical fit.

Sealing.

Electrical behavior.

EMC.

Reliability.

Assembly force.

Test limits.

Supplier qualification.

Service interchangeability.

Some existing evidence may remain valid.

Some may need analysis.

Some may need targeted regression.

The goal is not the smallest test plan.

The goal is proportionate evidence.

---

## 6. Emergency changes can still be controlled

Ramp creates emergencies.

A supplier stops shipping.

A safety problem appears.

A fixture breaks.

A critical component goes obsolete.

Sometimes you have to change quickly.

Fast does not have to mean uncontrolled.

An emergency deviation or temporary change can still define:

Scope.

Affected quantity.

Expiration date or condition.

Approval.

Effectivity.

Required evidence.

Containment.

Closure path.

The dangerous emergency change is not the fast one.

It is the temporary exception that quietly becomes permanent without being integrated into the baseline.

---

## 7. Supplier and contract-manufacturer cut-in

When suppliers or CMs are involved, release communication is not enough.

Did they receive the new definition?

Did they acknowledge it?

Is the new material available?

Is tooling ready?

Is inspection updated?

Is the test method updated?

What happens to old purchase orders?

What happens to old WIP at the supplier?

What is the first lot under the new configuration?

If the customer changes quickly and the supplier implements later, there is a hidden gap.

Effectivity must cross the organization boundary.

---

## 8. Post-cut-in effectiveness closes the change

A change is not finished because the ECO is closed.

Did the intended configuration actually cut in?

Did yield change?

Did the original failure disappear?

Did a new failure appear?

Did capacity change?

Did rework increase?

Did the supplier process remain stable?

Did field signals differ between old and new populations?

This is the effectiveness step.

Especially during ramp, technically plausible changes can move the constraint or create new quality mechanisms.

So monitor the changed population deliberately.

Change approval is not effectiveness evidence.

---

## 9. The Change Effectivity Map

Here is the listener tool.

Start with:

Change reason.

Affected requirements and interfaces.

Product-definition changes.

Process/tooling/test/work-instruction impacts.

Supplier impacts.

Inventory and WIP disposition.

Effectivity boundary.

Verification evidence.

Release communication.

Population monitoring.

Effectiveness result.

This turns a change from a document event into a controlled transition.

---

## 10. DEV to LVP to ramp

In DEV, changes are frequent.

Lightweight records may be enough if every important build remains reconstructable.

In LVP, multiple units and suppliers coexist.

Effectivity becomes much more important.

During ramp, the cost of ambiguity explodes.

Hundreds or thousands of units.

Open WIP.

Multiple lots.

Shifts.

Suppliers.

Field population.

The change-control system has to scale without becoming so heavy that engineering cannot move.

The goal is not bureaucracy.

It is preservation of truth while the product changes.

---

## 11. Five traps to avoid

ECO means document update only.

No.

Release date always proves effectivity.

Not necessarily.

Minor-looking supplier substitution needs no impact review.

Not automatically.

Emergency means uncontrolled.

No.

Change is closed when engineering releases it.

Not until implementation and effectiveness are understood for the required scope.

---

## 12. The action after this episode

Take the last meaningful engineering change.

Try to identify:

The first unit definitely new.

The last unit definitely old.

The WIP disposition.

The supplier cut-in.

The test or tooling change.

The evidence used to re-release.

If any of those are unknown, the change is not fully reconstructable.

---

## Season closing

Season 3 started with a product definition and asked:

How do we build the factory before we need the factory?

We built the MBOM and process flow.

Tooling and fixtures.

Work instructions.

Quality controls.

Measurement.

Layout.

Pilot planning.

Production validation.

Yield learning.

Capacity.

Supplier readiness.

And now controlled change during ramp.

The result is not a perfect factory.

It is something more useful.

A production system that can learn without losing its evidence.

Season 4 now asks what happens when that system has to remain trustworthy across time, suppliers, nonconformance, reliability, standards and scale.

# End spoken script

## Draft source anchors — not spoken

- Wave 01 configuration/change/effectivity source lock.
- Wave 02 supplier/quality source lock.
- W3-S02 — production-readiness context.
- Wave 03 ramp/evidence-envelope principles.
