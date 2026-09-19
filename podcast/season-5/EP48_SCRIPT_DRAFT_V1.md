# EP48 Full Script Draft V1 — Product Genealogy, Recipes, Parameters and Measurements

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 5 — Automation, Data and the Connected Factory
source_outline: EP48_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-05/
spoken_normative_standard_claims: NONE
regulated_retention_claims: NONE

## Production note — not spoken

NIST IR 8536 final (2026-09-09), NIST Digital Thread and UUID research support linked provenance/identity concepts. The Unit Evidence Thread and RECONSTRUCT 8 are internal synthesis.

# SPOKEN SCRIPT

## Opening

Serial number 1847 fails in the field.

Good.

At least we know which unit.

Engineering opens the database.

There is a final test record.

A production timestamp.

A machine historian has millions of data points around that time.

But then the questions begin.

Which material lot went into the unit?

Which recipe revision ran?

Was the connector changed during ramp?

Was the unit reworked?

Which fixture was used?

Which test-software version made the final decision?

Did the temperature signal belong to this unit or the one before it?

The serial number exists.

The genealogy does not.

That is the distinction for this episode.

**Identity tells you which object. Genealogy tells you how it became what it is.**

---

## 1. Serial number is the beginning, not the whole chain

A serial number is extremely valuable.

It gives the finished unit an identity.

But production truth is relational.

Unit 1847 may contain:

PCB lot A.

Connector lot B.

Enclosure batch C.

Firmware build D.

Calibration file E.

It moved through:

Operation 10.

Operation 20.

Test 30.

It was processed on:

Fixture F.

Machine G.

Recipe H.

And after failing once, it was reworked under deviation J.

That linked history is genealogy.

Without those relationships, the serial is a label attached to incomplete context.

---

## 2. NIST's new traceability framework reinforces the same idea

NIST finalized IR 8536 in September 2026.

The report presents a technology-neutral manufacturing traceability meta-framework for organizing, linking and querying traceability records across different ecosystems.

It emphasizes provenance, pedigree and a temporally ordered chain of events.

That is important for us because it reinforces a principle we already built into the Manufacturing Atlas:

Historical manufacturing truth is about linked events and relationships.

Not just current master data.

And importantly, NIST does not say every organization needs one centralized database.

That gives us architectural freedom.

We need linked trustworthy records.

Not one giant software product.

---

## 3. Build the Unit Evidence Thread

For this podcast, the genealogy chain is:

Product configuration.

Material and component genealogy.

Routing and operation.

Equipment and fixture.

Recipe or software configuration.

Critical parameter record.

Measurement and test.

Deviation and rework.

Final disposition and release.

Field linkage.

Not every product needs every field at the same detail.

Capture the dependencies that matter to quality, safety, reliability, investigation, service and release.

The principle is risk based.

---

## 4. Current master data cannot always reconstruct old production

This is a common failure.

You look at today's BOM.

Today's recipe.

Today's work instruction.

Then assume that is what built a unit six months ago.

But the definition changed.

Supplier changed.

Recipe changed.

Test limits changed.

A temporary deviation existed.

If history was overwritten, the current system may be correct for today and useless for reconstructing yesterday.

So historical truth needs revision and effectivity.

What definition existed?

Where did it apply?

What was actually executed?

That is why genealogy is tightly connected to configuration management.

---

## 5. Durable identity across systems

NIST's digital-thread work identifies persistent and globally unique identifiers as an important capability gap and research need.

Why?

Because different systems consume and transform engineering information across the lifecycle.

A durable identifier can help preserve the relationship.

But do not overread that.

A UUID does not prove the data are correct.

It does not prove who has authority.

It does not create provenance.

It is an identity mechanism.

Provenance needs the event relationships and evidence around it.

So use durable IDs where valuable.

Do not confuse identity technology with trust.

---

## 6. Source identifiers are not automatically enterprise identities

A PLC tag may be stable for years.

An OPC UA NodeId may be well governed inside a namespace.

A database primary key may be perfectly appropriate inside its system.

The mistake is assuming that because an identifier works locally, it is automatically the permanent cross-system semantic ID for the organization.

Maybe it is.

Maybe it should be mapped.

The architecture decision needs to be deliberate.

This matters during migration, replacement, line replication and supplier integration.

---

## 7. Recipe and parameter values need context

Suppose the historian says:

Pressure = 4.2.

What does that mean?

Which unit?

Which operation?

Which recipe?

Which units?

Which phase of the cycle?

Which sensor?

Which calibration state?

Was the value a setpoint or measured process value?

Without context, data are numbers.

With context, data can become evidence.

So for critical parameters, keep the product/operation/recipe/equipment/time relationship needed by the engineering decision.

---

## 8. Measurement context belongs in genealogy too

Wave 02 taught that measurement systems have identity and limitations.

Now connect that to genealogy.

A unit passes at 5.02 millimeters.

Which gauge?

Which fixture?

Which procedure?

Which calibration/reference state?

Which software version?

If the measurement method changes, historical comparability can change.

So the genealogy is not just what material went into the product.

It includes the evidence system that said the product was acceptable.

---

## 9. Rework adds history

Unit 1847 fails.

It is opened.

Connector replaced.

Retested.

Passes.

Do not overwrite the first state.

The final product has a new as-built history.

For field investigation, that distinction may be the entire answer.

Genealogy should make rework visible as an event:

old state,

action,

new state,

evidence,

decision.

That is much more useful than changing a status field from FAIL to PASS.

---

## 10. Time matters—but precision depends on the question

Manufacturing systems love timestamps.

But two systems can have clocks that are not perfectly aligned.

If you are reconstructing which batch was in a furnace over six hours, seconds may be irrelevant.

If you are correlating a millisecond machine event with a test failure, time synchronization may matter much more.

So do not prescribe one universal synchronization requirement.

Ask:

What event order or temporal precision is required to reconstruct the decision or causal sequence?

Then engineer the time architecture accordingly.

---

## 11. RECONSTRUCT 8

Here is the listener tool.

For a suspect unit or population, ask:

What was built?

From what?

Where?

How?

Under which recipe or configuration?

What was measured?

What failed or changed?

What population shares the same dependency?

If your systems cannot answer those questions for an important failure, the missing relationship is genealogy debt.

---

## 12. DEV to LVP to SVP

In DEV, genealogy may be a prototype ID, build note and linked test file.

In LVP, lot and serial linkage, rework and supplier identity become much more valuable.

In SVP, automated event capture, stable identifiers, retention, access and recovery become necessary to scale.

Do not start by buying enterprise genealogy software.

Start by deciding what history must survive.

---

## 13. Six traps to avoid

Serial number equals genealogy.

Latest BOM reconstructs old production.

Collect every machine tag and genealogy appears automatically.

UUID equals provenance.

Final PASS erases rework.

Timestamp means event order is always trustworthy.

---

## 14. The action after this episode

Pick one shipped serial.

Try to reconstruct:

definition,

materials,

route,

equipment,

recipe,

measurements,

failures/rework,

release.

Do it without asking the engineer or operator who remembers.

Every missing link is an information obligation for your next digital-thread iteration.

---

## Closing

EP48 reconstructs what physically happened to the product.

But another question remains.

An engineer finds a test report.

What engineering claim does it actually support?

Which requirement?

Which revision?

Which source?

What happens if the process changes?

That is Episode 49:

**Standards, Claims and Evidence as a Manufacturing Knowledge Graph.**

# End spoken script

## Draft source anchors — not spoken

- W5-S04 — NIST Digital Thread for Manufacturing.
- W5-S05 — NIST AMS 300-12 persistent/UUID research.
- W5-S06 — NIST IR 8536 final traceability meta-framework, 2026-09-09.
- Waves 01/02 — effectivity, rework and measurement evidence.
