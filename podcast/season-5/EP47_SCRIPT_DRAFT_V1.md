# EP47 Full Script Draft V1 — What PLM, ERP, MES, QMS, SCADA and Historians Actually Do

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 5 — Automation, Data and the Connected Factory
source_outline: EP47_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-05/
spoken_normative_standard_claims: NONE

## Production note — not spoken

ISA-95 is used only as public current integration/model context. The system-category ownership map is practitioner synthesis; no claim is made that ISA-95 mandates specific vendor categories or system-of-record assignments.

# SPOKEN SCRIPT

## Opening

A factory has a BOM in PLM.

Another BOM in ERP.

Work instructions in a shared folder.

A recipe stored in the machine.

Quality dispositions in email.

Production status in a spreadsheet.

And machine history in a historian.

Every system is locally “correct.”

Then a field failure arrives.

Someone asks:

Which definition actually built this serial?

Which material lot?

Which work instruction?

Which recipe?

Was there a deviation?

Was the unit reworked?

Suddenly the factory has a lot of data and very little truth.

This is the problem we are solving in this episode.

Not which software brand is best.

Not whether you “need MES.”

The question is:

**For each important manufacturing object or decision, where is the authoritative truth—and how do the other systems consume it without becoming competing truth?**

---

## 1. Start with the information object

Before PLM, ERP or MES, name the thing you are trying to control.

Product definition.

BOM.

Purchase order.

Material lot.

Work order.

Routing.

Recipe.

Unit genealogy.

Inspection result.

Nonconformance.

Release status.

Machine state.

Maintenance event.

Those are engineering and business objects.

Software is the custodian.

If you start from software categories, you can easily make the architecture fit the tool instead of the production need.

So the first design question is:

What object exists?

What decision depends on it?

Who has authority to create or change it?

Who needs to consume it?

That is system-of-record architecture.

---

## 2. What ISA-95 helps us with

ISA-95 is useful because it gives a common language for enterprise-to-manufacturing-control integration.

The current ISA Part 1 was updated in 2025.

At the public level, it describes the manufacturing operations and control domain, the organization of physical assets, functions at the enterprise/control interface and the information exchanged across that boundary.

That is valuable.

It means the idea that manufacturing and enterprise systems need explicit information boundaries is not something we invented for this podcast.

But be careful.

ISA-95 does **not** mean:

“Level 4 equals ERP, Level 3 equals MES, therefore buy these exact systems.”

And it does not mean every company must implement five physical software layers.

Use ISA-95 as a reference model and shared language.

Not as a shopping list.

---

## 3. PLM or PDM: definition and configuration context

In many organizations, PLM or PDM systems hold product definition.

Drawings.

CAD.

BOM structures.

Specifications.

Revisions.

Engineering changes.

But the exact boundary varies.

Some companies keep manufacturing BOM data elsewhere.

Some keep work instructions in MES.

Some use lightweight controlled repositories.

The transferable role is:

**controlled product definition and configuration context.**

The brand and implementation can differ.

---

## 4. ERP or MRP: planning and transactions

ERP systems often own commercial/material/resource transactions.

Purchase orders.

Inventory.

Work orders.

Demand and planning.

Cost/accounting context.

Supplier transactions.

But ERP is not automatically the right place to store every physical process truth.

A purchase transaction can tell you a lot arrived.

It may not tell you which serial consumed which exact lot unless execution/genealogy systems provide the linkage.

So ERP can be authoritative for a transaction while another system is authoritative for execution evidence.

That is normal.

---

## 5. MES or MOM: execution context

Where MES or MOM exists, it often handles execution.

Dispatch.

Routing.

WIP.

Operation completion.

Operator/station context.

Production records.

Genealogy.

But again, do not convert a common role into a universal rule.

A small LVP factory may implement these functions with a custom database, barcode workflow or controlled digital traveler.

The question is not:

“Do we have MES?”

The question is:

**Can we reconstruct what execution actually happened?**

---

## 6. QMS: quality events and decisions

A QMS may own:

Nonconformance.

Deviation.

CAPA.

Audit.

Disposition.

Quality approvals.

But even here, quality truth often needs links to other systems.

The NCR references a unit.

The unit references a work order.

The work order references a configuration.

The failure references a measurement.

The disposition may change release status.

If the QMS is isolated, the quality record exists but the evidence chain is weak.

---

## 7. SCADA, HMI and controls: operational supervision and control

SCADA, HMI, PLC and control systems live close to the physical process.

They may contain:

machine state,

alarms,

setpoints,

recipes,

interlocks,

process values,

operator commands.

This is where software architecture can become dangerous.

A machine-local recipe may be the value actually used in production.

But does that make the PLC the enterprise master of the recipe definition?

Not necessarily.

Maybe the recipe is authored elsewhere and deployed to the machine.

Maybe the machine owns only the active instance.

The architecture needs to distinguish:

definition,

distribution,

active execution,

history.

---

## 8. Historian: time-series history, not all manufacturing truth

Historians are excellent at high-rate process and equipment history.

Temperature.

Pressure.

Speed.

Current.

Alarm state.

But a historian sample by itself may not know:

which product was present,

which operation,

which recipe revision,

which material lot,

which rework state.

So a historian is not automatically genealogy.

It is a powerful source of evidence that needs context.

---

## 9. Authoritative owner does not mean only one copy

This distinction matters.

A BOM may be authored in PLM and copied into ERP.

A recipe may be defined in one system and deployed into a controller.

A quality status may be replicated to MES for execution decisions.

Replication is not inherently bad.

Caching is not inherently bad.

The question is:

Which record is authoritative for which decision?

How is revision/effectivity preserved?

What happens when copies disagree?

When does synchronization occur?

Who may change the source?

If those questions are explicit, multiple copies can be operationally useful.

If they are not, you create competing truth.

---

## 10. The System-of-Record Map

Here is the listener tool.

Choose an information object.

Then record:

Authoritative owner.

Consuming systems.

Identifier.

Revision or effectivity.

Interface.

Latency or availability need.

Evidence that must be retained.

Fallback or recovery behavior.

Let's take product revision.

Authoritative owner might be the controlled engineering definition.

ERP consumes the revision for planning.

MES consumes it for execution.

Test software uses it to select limits.

QMS links NCRs to it.

The critical question is not that everybody has the same string.

The critical question is that they all refer to the same controlled meaning.

---

## 11. Run the Competing-Truth Audit

Pick seven objects:

Product revision.

Routing.

Recipe.

Quality status.

Unit genealogy.

Material lot.

Machine configuration.

For each one ask:

Where can it be changed?

Where can it be copied?

Which copy controls production?

Which copy controls release?

What happens if systems disagree?

What is the recovery source after outage?

Every “we're not sure” is an architecture debt item.

---

## 12. DEV to LVP to SVP

In DEV, a disciplined spreadsheet plus Git and structured test files can be enough.

The important thing is identity.

In LVP, system boundaries become harder to keep in people's heads.

Released definitions.

Work orders.

Lots.

Serials.

Rework.

Now explicit ownership and interfaces matter.

In SVP, multiple products, lines, sites and automated systems force the issue.

Authority, access, recovery, versioning and integration must scale.

Enterprise software becomes useful when the information obligation earns it.

Not because the company reached a certain employee count.

---

## 13. Five traps to avoid

ERP is master of everything.

MES is automatically required for mature manufacturing.

ISA-95 defines my vendor stack.

Duplicate data is always wrong.

Integration can fix unclear ownership.

It cannot.

Integration moves ambiguity faster.

---

## 14. The action after this episode

Take seven information objects your factory cannot afford to misunderstand.

For each one write:

Authoritative source.

Who can change it.

Who consumes it.

How version/effectivity is represented.

What happens if the authoritative system is unavailable.

If two teams give different answers, you have found the next data-architecture problem.

---

## Closing

Episode 47 defines where different forms of manufacturing truth live.

Now we have to follow the physical product through those systems.

If serial 1847 fails in the field, can we reconstruct what material, process, recipe, equipment, measurement and rework history created it?

That is Episode 48:

**Product Genealogy, Recipes, Parameters and Measurements.**

# End spoken script

## Draft source anchors — not spoken

- W5-S01/S02 — current ISA-95 public scope/status.
- W5-S04/S07 — NIST digital-thread context.
- system-category ownership descriptions are Hardware-to-Production practitioner synthesis.
