# EP51 Full Script Draft V1 — OPC UA, ISA-95 and Semantic Integration Without the Buzzwords

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 5 — Automation, Data and the Connected Factory
source_outline: EP51_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-05/
spoken_normative_standard_claims: NONE
cybersecurity_ownership: EP52

## Production note — not spoken

ISA-95 current public Part 1 (2025) is used as scoped enterprise/manufacturing integration context. OPC Foundation public material supports OPC UA infrastructure and Companion-Spec information-model layering. No IEC 62541 clause detail is required.

# SPOKEN SCRIPT

## Opening

A data platform receives one value:

Temp_07 = 83.4.

The connection works perfectly.

The broker delivered it.
The database stored it.
The dashboard plotted it.

Now ask:

Temperature of what?

Celsius?
Fahrenheit?
Furnace zone?
Adhesive dispense?
Bearing?
Ambient air?

Which machine?
Which product?
Which operation?
Which recipe?

Was 83.4 normal, high or meaningless?

Connectivity succeeded.

Information transfer failed.

That is the problem for this episode.

Industrial integration has at least three different layers:

Can systems connect?

Can they exchange a valid data structure?

Do both sides understand the engineering meaning?

Those are not the same problem.

## 1. Connectivity is not semantics

At the lowest level, systems need a path.

Network.
Protocol.
API.
Broker.
File transfer.
OPC UA.
Something.

Then syntax matters.

Can the receiving system parse the message?

Field names.
Types.
Structure.
Timestamp.

But even valid syntax can carry ambiguous meaning.

state = 3.

What does 3 mean?

pressure = 4.2.

Which units?

recipe = R17.

For which product?

Semantic integration means the consumer can interpret the engineering object correctly without tribal knowledge about the source system.

That is the step many integration projects skip.

## 2. ISA-95 gives useful manufacturing context

ISA-95 is one of the most useful reference families for discussing enterprise/manufacturing-control integration.

ISA updated Part 1 in 2025.

At public scope, it helps define the manufacturing operations/control domain, physical-asset organization and enterprise/control information interfaces.

That gives us a language for talking about manufacturing hierarchy and responsibility.

Enterprise.
Site.
Area.
Production resources.
Activities and information exchange.

But do not turn that into:

ISA-95 requires my architecture to have exactly these five software layers.

It does not.

And do not use ISA-95 levels as if they were automatically cybersecurity network zones.

That is a different problem.

Use ISA-95 for functional and information context.

## 3. What OPC UA gives you

OPC UA is useful because it is more than raw tag transport.

The OPC Foundation describes infrastructure for:

Discovery.
Transport.
Information access.
Security.
Object-based information models.

That means data can be exposed as structured objects and relationships rather than only isolated registers.

This is powerful.

But it still does not mean the organization suddenly has a complete business ontology.

OPC UA provides infrastructure and information-modelling capability.

The manufacturing organization still has to define:

Which product?
Which operation?
Which unit?
Which authoritative definition?
Which genealogy?
Which effectivity?
Which decision?

## 4. Companion Specifications add domain models

The OPC Foundation uses Companion Specifications to define domain-, device- or use-case-specific information models and profiles.

This is exactly why you should look before inventing everything yourself.

Maybe your equipment or industry already has a useful model.

Use or map to it where it fits.

But that is an engineering recommendation, not a universal rule.

A Companion Specification can improve semantic interoperability.

It does not decide your ERP ownership, genealogy policy or product-release logic.

## 5. Identity has to survive system boundaries

Suppose the PLC calls the station CELL_04.

MES calls it WC-119.

Historian calls it AREA2_LINE1_INSERTION.

All can be legitimate.

The integration problem is knowing they refer to the same engineering object.

NIST digital-thread research highlights persistent and universally unique identifiers as a way to improve lifecycle traceability.

That does not mean every organization must replace readable IDs with UUIDs.

It means durable identity matters.

Map local identifiers to a governed engineering identity where cross-system continuity matters.

## 6. NodeId, tag name and database key are local identities until governance says otherwise

This point needs nuance.

An OPC UA NodeId can be stable and well designed.

A PLC tag can be carefully governed.

A database key can remain unchanged for decades.

The problem is not that these identifiers are bad.

The problem is assuming automatically that a source-system identifier should become the organization's permanent cross-system semantic identity.

Maybe it should.

Maybe it should map to another identifier.

The decision depends on lifecycle, migration, replication and interoperability needs.

Make the decision explicit.

## 7. Preserve engineering context with the data

For a critical signal, capture enough context that another system can use it correctly.

Engineering object.
Stable identifier.
Hierarchy or location.
Attribute or signal.
Unit.
State meaning.
Source owner.
Product or lot.
Operation.
Recipe.
Consumer.
Version.
Security and recovery consequence.

Not every high-rate tag needs every field copied into every message.

The architecture can join context through identifiers.

The requirement is that the decision can recover the meaning.

## 8. Event, state and time series are different

A temperature sampled every second is time series.

A machine mode may be state.

Recipe changed from R16 to R17 is an event.

Those distinctions affect storage and reconstruction.

If you record only current state, history disappears.

If you record only samples, important events may be hard to infer.

Design data representation around the engineering question.

## 9. Semantic models have configuration too

Information models change.

Tag mapping changes.
Equipment gets renamed.
Recipe structure changes.
A new product variant appears.

If the semantic layer changes silently, historical data can become ambiguous.

So version the mapping.

Define effectivity.

Preserve enough history that old data remain interpretable.

Semantic integration is still configuration management.

## 10. Security is part of the interface—but depth comes next

OPC UA includes security capabilities.

That is valuable.

But protocol security is not the complete OT security program.

A secure connection can still grant too much authority.

A valid certificate can still connect a badly designed architecture.

EP52 owns that problem.

For this episode, the rule is:

Connectivity should be no broader than the manufacturing decision requires, and the production consequence of failure or loss should shape the interface.

## 11. The Context-to-Data Integration Map

Here is the listener tool.

Write:

Engineering object.
Stable identity.
Hierarchy/context.
Signal or attribute.
Unit/state meaning.
Source owner.
Interface/protocol.
Product/operation/recipe relationship.
Consumer or decision.
Version.
Security/recovery consequence.

If a downstream engineer cannot interpret the datum from that map, the integration is not semantically complete.

## 12. The Meaning-Preservation Test

Pick one machine tag.

Give it to an engineer who did not program the PLC.

Can they answer:

What physical thing is this?
Units?
State?
Which operation?
Which product context?
Who owns the definition?
How do I know when the meaning changed?

If the answer depends on calling one veteran engineer, the factory still has semantic tribal knowledge.

## 13. Five traps to avoid

OPC UA endpoint equals semantic architecture.

ISA-95 equals mandatory software stack.

ISA-95 levels equal cybersecurity zones.

Tag name equals global identity.

Protocol security equals OT security.

## 14. The action after this episode

Take ten signals that feed a dashboard or analytics model.

For each one, try to define:

identity,
units,
operation,
product/recipe context,
source authority,
and version.

The missing fields are not documentation problems.

They are semantic integration problems.

## Closing

EP51 gives connected data meaning.

Now we have to ask whether the connected data are fit for real engineering decisions—and whether the connection itself creates a production risk.

A data lake can contain millions of samples and still be useless for root cause.

A read-only connector can still create availability or credential risk.

A write-back integration can alter the physical process.

Episode 52 closes Season 5 with:

Manufacturing Data Engineers Can Actually Use.

# End spoken script

## Draft source anchors — not spoken

- W5-S01/S02 — current ISA-95 public scope/status.
- W5-S03 — OPC UA infrastructure/Companion Specifications.
- W5-S04/S05 — NIST digital thread and durable identity.
- OT security depth deferred to EP52.