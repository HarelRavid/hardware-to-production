# 9.12 OPC UA & Semantic Integration Boundary

status: Researching
provenance: [GNR]

## Purpose
Define the boundary between machine-level/industrial interoperability standards and the broader Manufacturing Atlas semantic model.

## Integration layers
- machine/control protocol
- information model / semantic namespace
- gateway/edge mapping
- event/time-series transport
- enterprise integration/API
- Atlas stable semantic identity

## OPC UA role
OPC UA can provide structured industrial data access and information models for equipment, variables, events and methods. It is an integration mechanism and semantic source; it is not by itself the complete product/process/quality/knowledge ontology.

## Mapping objects
- source node/identifier
- source namespace/model revision
- equipment asset ID
- parameter/measurement definition ID
- engineering unit
- timestamp semantics
- quality/status code
- sampling/aggregation context
- Atlas semantic ID
- mapping revision/effectivity

## Semantic integration questions
1. Is the incoming signal a command/setpoint, actual state, calculated value or measurement?
2. Which physical/equipment/product context does it belong to?
3. Are units and scaling explicit?
4. Is event time preserved separately from ingestion time?
5. Does the mapping survive machine replacement/controller upgrade?
6. Is a vendor-specific tag name being mistaken for durable semantic identity?

## Information-model alignment boundary
Relevant industrial information models/companion specifications may be mapped where useful, but Atlas object identity should remain stable across vendor/protocol changes.

## Edge/gateway principle
Normalization near the source can reduce integration complexity, but transformations must preserve lineage, units, timestamps and raw-source reference.

## Decision objects
### D-DH-INT-001 — Direct system integration, OPC UA, gateway/edge or batch/API path?
### D-DH-MAP-001 — Mapping from source semantics to Atlas object model
### D-DH-RAW-001 — Which raw/source data must be retained versus normalized/aggregated?

## Anti-patterns
- treating PLC tag names as enterprise ontology;
- stripping status/quality codes from process data;
- losing source timestamp during ingestion;
- silently converting units without lineage;
- hard-coding equipment identity to network address;
- assuming a connectivity standard resolves data ownership/governance.

## Integrity rule
Connectivity is not semantic integration; semantic integration is not governance.