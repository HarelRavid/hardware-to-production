# Episode 48 Production Blueprint — Product Genealogy, Recipes, Parameters and Measurements

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
lifecycle: LVP → SVP → FIELD
maps_to: MASTER_WBS 9.3–9.7

## Listener transformation
Before: stores machine data and serial numbers but cannot reliably reconstruct the as-built/as-processed history of a unit.
After: designs genealogy linking product configuration, materials, routing, recipes, equipment, parameters, measurements, quality events and rework into a reconstructable evidence chain.

## Narrative hook
A field failure is traced to serial 1847. The team has a test record and a timestamp, but the material lot, recipe revision and rework event cannot be linked confidently. Terabytes of process data exist; the evidence chain does not.

## Teaching flow
1. Definition versus execution/as-built state versus evidence.
2. Unit/lot/batch/carrier identity and parent-child assembly genealogy.
3. Material/component lot linkage and substitutions.
4. Operation/routing and equipment identity.
5. Recipe/configuration version and effectivity.
6. Critical process parameters: context, units, limits and timestamps.
7. Measurements/test results and measurement-system identity.
8. Deviations, rework and repair add history rather than overwrite it.
9. Time synchronization and event ordering where causality/reconstruction depends on it.
10. Retain enough evidence to reconstruct affected populations and release decisions.

## Core framework — Unit Evidence Thread
`Product config → material/component genealogy → routing/operation → equipment/fixture → recipe/software config → parameter record → measurement/test → deviation/rework → final disposition/release → field linkage`.

## Listener tools
- Unit Evidence Thread Design Card.
- RECONSTRUCT 8 Investigation Query: what was built, from what, where, how, under which recipe/configuration, what was measured, what failed/changed and what population shares the dependency?

## DEV / LVP / SVP
DEV: build IDs and revision/test linkage may be lightweight. LVP: lot/unit genealogy and rework visibility become essential for learning. SVP: scalable identifiers, effectivity, system interfaces, retention, access and recovery support population-level decisions.

## Common mistakes
- serial number = genealogy;
- parameter values stored without recipe/product/operation context;
- overwrite of recipe or rework history;
- timestamps assumed comparable across unsynchronized systems;
- collecting all tags while omitting the identifiers needed to join them;
- final PASS used to erase prior failure.

## Source/evidence backlog
Record-retention and regulated traceability obligations remain industry/jurisdiction specific. Data models may use ISA-95/OPC UA or sector standards where applicable, but the evidence chain is product/process specific.

## Closing handoff
Episode 49 shifts from unit evidence to engineering knowledge: how requirements, standards, claims and evidence can form a manufacturing knowledge graph rather than a document archive.
