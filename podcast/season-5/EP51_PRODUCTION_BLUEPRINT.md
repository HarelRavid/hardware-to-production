# Episode 51 Production Blueprint — OPC UA, ISA-95 and Semantic Integration Without the Buzzwords

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
lifecycle: LVP → SVP
maps_to: MASTER_WBS 9.2, 9.12

## Listener transformation
Before: connects machines and systems by moving tags/fields between APIs, brokers and databases.
After: defines manufacturing identities, hierarchy, context and semantics so exchanged data preserves engineering meaning across equipment, operations and enterprise systems.

## Narrative hook
A data platform receives `Temp_07 = 83.4`. Is it a furnace zone, adhesive dispense temperature, ambient sensor or bearing temperature? Which unit? Which product and operation? Which recipe revision? Connectivity succeeded; information transfer failed.

## Teaching flow
1. Connectivity, syntax and semantics are different problems.
2. Stable identities for site/area/line/cell/equipment and product/operation.
3. ISA-95 as a useful enterprise-control/manufacturing context model where applicable, not a mandatory software architecture.
4. OPC UA as an information/communication technology that can carry structured context, not automatic semantic correctness.
5. Naming, units, engineering ranges and state definitions.
6. Event versus state versus time-series measurement.
7. Product/lot/unit/operation/recipe context joined to machine signals.
8. Version/effectivity of semantic models and mappings.
9. Interface failure, latency and offline modes based on production consequence.
10. Security boundary and least necessary connectivity as part of architecture.

## Core framework — Context-to-Data Integration Map
`Engineering object → stable identifier → hierarchy/context → attribute/signal → unit/state semantics → source owner → interface/protocol → product/operation/recipe link → consumer/decision → version/security/recovery`.

## Listener tools
- Context-to-Data Integration Map.
- Meaning-Preservation Test: can a consumer interpret the datum correctly without tribal knowledge about the source tag/database column?

## DEV / LVP / SVP
DEV: simple naming/interfaces are acceptable if identity and units are explicit. LVP: stable equipment/product/operation identifiers and mappings become necessary. SVP: governed semantic models, versioning, availability, cybersecurity and recovery support dependable integration.

## Common mistakes
- OPC UA endpoint = semantic architecture;
- ISA-95 treated as a mandatory product stack rather than scoped reference model;
- tag names used as global identifiers;
- units/context assumed from tribal knowledge;
- interface changes without effectivity/version control;
- adding broad network connectivity because the protocol supports it.

## Standards/applicability gate
Any normative or definitional claim about ISA-95/IEC 62264, OPC UA/IEC 62541 or related standards requires exact current edition/part/scope verification before script authority. The episode teaches architecture concepts without inventing universal implementation rules.

## Closing handoff
Episode 52 asks what subset of this connected data is actually trustworthy and usable for engineering decisions — and how to obtain it without creating unsafe IT/OT pathways.
