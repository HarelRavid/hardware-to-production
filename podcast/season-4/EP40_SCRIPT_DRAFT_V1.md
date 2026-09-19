# EP40 Full Script Draft V1 — Supplier Quality, Dual Sourcing and Resilience

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 4 — Quality, Suppliers and the Reality of Scale
source_outline: EP40_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-02/
spoken_normative_standard_claims: NONE
protected_manual_detail: EXCLUDED

## Production note — not spoken

The script uses NIST MEP for public supplier-management context and the Wave 01/02 canonical evidence model for change, qualification and resilience. Exact supplier-change-notification and requalification obligations remain customer/contract/sector specific.

# SPOKEN SCRIPT

## Opening

Your company says it has two suppliers for a critical component.

That sounds resilient.

Then the primary supplier has a serious disruption.

Purchasing calls the backup supplier.

And discovers three things.

The backup supplier has never built the current revision.

Its tooling was never updated after the last design change.

And the material it qualified two years ago is no longer the material in the current product.

On the supplier list, you had two sources.

In production reality, you had one.

That is the core idea of this episode.

A supplier is not just a company name.

It is a production capability inside a defined evidence envelope.

Product revision.

Process.

Site.

Tooling.

Material.

Sub-tier.

Measurement system.

Test.

Rate.

Change history.

When those things move, the meaning of “approved supplier” can move with them.

So this episode asks:

**How do we manage supplier quality and resilience after the original approval is complete?**

---

## 1. Approval is an evidence envelope, not a permanent badge

Think back to Episode 39.

We approved first production based on evidence.

That evidence came from some specific state.

A specific drawing revision.

A specific source.

A specific process.

A specific site.

Specific tooling.

Specific inspection and test.

Maybe a specific sub-tier heat-treatment provider.

Maybe a defined production rate.

Now imagine one of those changes.

Does the original approval automatically remain valid?

Sometimes yes.

Sometimes no.

The right question is not:

“Was this supplier approved before?”

The right question is:

**Which claim did the old evidence support, and did the change touch the assumptions that made the evidence valid?**

That is the same change-control logic we used inside our own factory.

A supplier is part of the production system.

The same evidence discipline applies across the company boundary.

---

## 2. Supplier performance is multidimensional

NIST Manufacturing Extension Partnership material describes supplier management in terms that include supplier evaluation, segmentation, total cost of ownership, supplier metrics and supplier development.

That is useful because supplier performance is not one number.

Quality matters.

Delivery matters.

Response to problems matters.

Change discipline matters.

Capacity matters.

Technical capability matters.

Continuity risk matters.

Commercial stability can matter.

Sub-tier dependence can matter.

This is why supplier scorecards exist.

They create visibility across several dimensions.

But be careful.

The scorecard is a management tool.

It is not permission to average away a hard stop.

---

## 3. A weighted score must not hide a critical failure

Imagine a supplier scorecard.

Delivery: excellent.

Cost: excellent.

Responsiveness: excellent.

Quality: good.

Change control: poor.

Then the supplier makes an unreviewed change that can affect a safety-critical characteristic.

What is the overall score?

I do not care.

The issue is a hard stop until the evidence is understood.

Weighted scores are useful for prioritization and trend.

They are dangerous if they create the illusion that excellent performance in one dimension compensates for unresolved evidence in another.

A supplier can be 95 out of 100 and still have one issue that makes release unacceptable.

So keep scorecards and release decisions connected—but not identical.

---

## 4. Incoming inspection is one control, not the whole supplier-quality system

A common response to supplier problems is:

“We'll inspect more when the parts arrive.”

Sometimes that is exactly the right containment action.

Incoming inspection can be valuable.

Especially during a new source, process change, recovery or known-risk period.

But it has limits.

Suppose the failure mechanism is internal material state.

Or a heat-treatment condition.

Or contamination.

Or a latent weld defect.

Or a software/calibration configuration.

Or a process characteristic that final inspection cannot see economically.

More receiving inspection does not automatically control the source mechanism.

So ask:

What claim are we trying to protect?

Can incoming inspection actually detect the failure mode?

If not, the evidence needs to move upstream into supplier process control, qualification, certification, audit, test, or another mechanism appropriate to the risk.

Do not turn “inspect more” into a substitute for understanding the supplier process.

---

## 5. Supplier change is a configuration event

Now the supplier sends a message.

They want to change something.

New raw material source.

New sub-tier.

New machine.

New tooling.

New factory location.

New inspection method.

New process sequence.

New software version in test equipment.

Do all supplier changes require full requalification?

No.

That would be wasteful.

Do supplier changes never matter if the drawing number stays the same?

Also no.

The correct sequence is familiar.

What changed?

Which product/process claims depend on it?

Which prior evidence assumptions did the old state support?

Does the change touch those assumptions?

What new evidence is proportionate?

Which units or lots receive the change?

How do we record effectivity?

What post-change monitoring is needed?

The exact notification rules depend on the applicable customer contract, standard and sector.

But the engineering principle is general:

**a consequential supplier change must not silently cross the boundary of the approval evidence.**

---

## 6. Dual sourcing is an evidence problem

Companies love the phrase “dual source.”

It sounds safe.

But two suppliers are not automatically two interchangeable production systems.

Supplier A may machine the part.

Supplier B may forge and finish-machine it.

One may use one material route.

The other another approved route.

One may inspect with CMM.

The other with dedicated gauges.

That can be completely acceptable.

The goal is not identical manufacturing architecture.

The goal is independent evidence that each source satisfies the required product/process claims inside its own controlled route.

So a dual-source readiness review should ask:

Current product revision?

Current approved material?

Current process route?

Tooling available?

Measurement method?

Test?

Open deviations?

Capacity?

Lead time?

Sub-tier dependencies?

Genealogy?

Any customer approval needed?

What change would invalidate the source?

If those answers are stale, the source may exist commercially without existing technically.

---

## 7. Common-mode risk: two suppliers, one dependency

Now suppose Supplier A and Supplier B are both fully qualified.

Great.

But both buy the same custom connector from one sub-tier.

Or both use the same heat-treatment house.

Or both depend on the same mold tool.

Or both use the same software library.

Or both source the same constrained resin from one manufacturer.

A company can have two supplier logos and one failure mode.

This is common-mode risk.

Resilience requires mapping dependencies below the supplier name.

Not every sub-tier needs equal visibility.

Focus on dependencies where loss or change can threaten product claims, capacity, recovery time or requalification lead time.

That is where the map creates value.

---

## 8. Total cost matters because recovery is expensive

Purchase price is visible.

Recovery cost often is not.

Expedite.

Premium freight.

Engineering time.

Supplier-quality travel.

New tooling.

Qualification.

Scrap.

Line downtime.

Customer containment.

Inventory.

Working capital.

NIST MEP supplier-management guidance includes total cost of ownership because the cheapest quotation is not necessarily the lowest-cost production system.

The same logic applies to resilience.

A backup source that saves five percent on piece price but requires six months to reactivate may have a very different business value from a source that can safely cut in within weeks.

That does not mean every part needs expensive dual sourcing.

It means the sourcing strategy should reflect consequence and recovery time.

---

## 9. The Supplier Resilience Map

Here is the listener tool.

Pick a critical part.

Write:

Part or capability.

Current source.

Current process.

Important sub-tier dependencies.

Quality and capability evidence.

Change controls.

Capacity and logistics risk.

Alternate source.

Evidence gaps at the alternate.

Tooling and data required to transfer.

Lead time to qualify or restart.

Recovery trigger.

Let's use the Sentinel Node connector.

Primary source is qualified.

Alternate source exists commercially.

But the alternate has a different internal contact geometry and different environmental performance data.

That is not automatically bad.

But it means the equivalence claim has not yet been demonstrated for every relevant requirement.

Maybe the alternate is good enough.

Maybe it needs environmental regression testing.

Maybe firmware or calibration is unaffected.

Maybe enclosure sealing is affected.

The map makes the evidence gap visible before the shortage.

That is resilience engineering.

---

## 10. When a supplier escape happens

Supplier quality becomes real when something escapes.

A bad lot arrives.

Production uses it.

The issue is found after assembly.

Or in the field.

The immediate questions are:

What population is affected?

Can we identify the supplier lot, date, line or process state?

What WIP is exposed?

What finished product contains it?

What containment is needed?

What evidence distinguishes good from suspect?

Then move upstream.

What changed?

What control failed?

What detection missed it?

Does the supplier corrective action address the mechanism?

How will we know it worked?

This is where supplier-quality management connects directly to CAPA, genealogy and effectiveness evidence.

The supplier boundary does not break the engineering chain.

---

## 11. DEV to LVP to serial production

In DEV, you may work with prototype suppliers.

That is fine.

The supplier's job may simply be to create learning hardware.

Do not confuse prototype capability with production qualification.

In LVP, supplier evidence becomes much more important.

Repeatable process.

Representative material.

Traceability.

Inspection.

Change ownership.

Capacity.

As you scale, the supplier system becomes dynamic.

Multiple sites.

Sub-tiers.

Tool maintenance.

Alternate materials.

Rate increases.

Dual sources.

Commercial pressure.

You need a process that can absorb change without losing the connection between approval and actual production state.

That is supplier maturity.

Not the number of supplier forms.

---

## 12. Six traps to avoid

Trap one:

**Approved vendor equals approved forever.**

No.

Approval is bounded by evidence.

Trap two:

**Two supplier names equals resilience.**

Not if the second source cannot build the current product.

Trap three:

**Incoming inspection fixes a weak supplier process.**

Sometimes it contains risk.

It does not automatically control the source mechanism.

Trap four:

**One weighted supplier score captures everything.**

It can hide hard stops.

Trap five:

**The second source must use the same process.**

Not necessarily.

Different routes can be valid if the required claims are independently demonstrated.

Trap six:

**Resilience means different geography.**

Geography is one factor.

Tooling, material, sub-tier, software, capacity and qualification lead time can be just as important.

---

## 13. The action after this episode

Pick one purchased part that would hurt badly if the current source stopped tomorrow.

Ask:

What exactly would have to move or be recreated?

Drawing?

Tooling?

Process know-how?

Material?

Sub-tier?

Test method?

Inspection program?

Qualification evidence?

Customer approval?

Software?

Then ask:

How long would it take before another source could ship product we would actually release?

That answer is your real source redundancy.

Not the approved-vendor count.

---

## Closing

At the end of Season 4, we have taken quality beyond our own factory.

We have connected risk to process controls.

Measurement to trustworthy decisions.

SPC to process behavior.

First-production approval to representative supplier evidence.

And supplier quality to sustained performance, change and resilience.

Now we are ready for the next temptation.

Automation.

More equipment.

More data.

More integration.

Faster lines.

The dangerous assumption is that automation makes a weak production system mature.

It does not.

It can make a weak system faster.

Season 5 begins by asking the question that should come before every robot, vision system and automated station:

**Should we automate this process at all?**

# End spoken script

## Draft source anchors — not spoken

- W2-S11 — NIST MEP Supply Chain Management: supplier evaluation/selection, TCO, segmentation, metrics/scorecards and supplier development.
- W2-S05/W2-S12 — scoped PPAP/FAI method context.
- Wave 01 configuration/change lock — effectivity and evidence impact.
- Exact supplier-change notification, customer flow-down and requalification obligations remain customer/sector specific.
