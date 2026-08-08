# 9.4–9.7 Genealogy, Execution, Versioning & Temporal Effectivity Model

status: Researching
provenance: [GNR]

## Purpose
Allow reconstruction of exactly what configuration, process, resource, parameter and evidence applied to a unit/lot at a historical point in time.

## Four distinct time concepts
- valid/effective time: when a definition/revision is intended to apply
- transaction/record time: when the system learned/recorded it
- execution time: when the manufacturing event actually occurred
- observation time: when a measurement/condition was observed

These times may differ and should not be silently collapsed.

## Definition/revision/instance pattern
Definition -> Revision -> Effectivity -> Instance/Execution -> Observation/Result.

Examples:
Process Definition -> Process Revision -> effective date/serial range -> Operation Execution -> parameter observations.
Tool -> Tool Revision -> qualification/effectivity -> tool usage event.
Test Definition -> Test Recipe Revision -> effectivity -> Test Execution -> raw results.

## Genealogy event model
A genealogy event may:
- consume material/part lots
- merge components into an assembly
- split bulk material/batch
- transform product state
- apply a process/load
- record equipment/tool/operator
- create measurements/test evidence
- create defect/NCR/rework path
- release/hold/scrap product

## Intermediate Product State
State dimensions may include:
- configuration/revision
- dimensions/geometry condition
- material/metallurgical condition
- surface/coating condition
- cleanliness/moisture condition
- assembly completeness
- calibration/configuration/software state
- quality/release status

The state is not necessarily duplicated as a giant snapshot; it can be reconstructed from typed events where architecture/performance permits.

## Effectivity objects
- date/time range
- serial range
- lot/batch range
- product variant
- site/line/equipment
- supplier/site
- temporary deviation window

## Engineering change cut-in
EngineeringChange -> affected definitions/revisions -> approved effectivity -> WIP disposition -> inventory disposition -> revalidation requirement -> actual execution genealogy.

## Historical truth principle
Correcting master data must not rewrite what actually happened to historical units. The Atlas needs current truth and historical execution truth simultaneously.

## Decision objects
### D-DH-TIME-001 — Which time semantics are required for this object/event?
### D-DH-EFF-001 — How is revision/effectivity expressed?
### D-DH-GEN-001 — What minimum event graph is required to reconstruct genealogy and containment?

## Integrity rule
Never infer historical configuration from today's current master data when execution-specific revision/effectivity evidence exists or should exist.