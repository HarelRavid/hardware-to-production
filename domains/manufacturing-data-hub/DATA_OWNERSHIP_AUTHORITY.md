# 9.13 Data Ownership & Authoritative-Source Model

status: Researching
provenance: [GNR]

## Purpose
Define who owns the meaning, lifecycle, quality and authoritative value of manufacturing data while allowing the Atlas to integrate and reason across systems without creating competing truths.

## Distinct responsibilities
- Data owner: accountable for definition, policy, quality and lifecycle.
- Data steward: maintains semantics, metadata and quality rules.
- System of record: authoritative application for a defined datum/object state.
- Data producer: creates observations/events.
- Data consumer: uses data for execution, analytics or decisions.
- Semantic owner: governs ontology term/relationship meaning.

## Authority rule
Authority is assigned at object/attribute/event level, not merely by application name.

Examples:
- PLM may own released Part Revision.
- ERP may own inventory balance.
- MES may own Operation Execution and production genealogy.
- QMS may own NCR/CAPA disposition state.
- Historian may own high-frequency recorded process observations.
- Atlas/Knowledge OS may own semantic mappings, engineering claims/evidence relationships and decision models.

## Conflict model
When two systems disagree:
1. identify the semantic object/attribute;
2. identify applicable time/effectivity;
3. determine authoritative source;
4. preserve conflicting observations where historically relevant;
5. resolve master-data error through controlled correction rather than silent overwrite.

## Data-quality dimensions
- completeness
- validity
- consistency
- uniqueness
- timeliness
- traceability/lineage
- revision/effectivity correctness
- semantic conformity

## Decision objects
### D-DH-OWN-001 — Who owns this semantic object/attribute?
### D-DH-SOR-001 — Which system is authoritative for this value/state and time?
### D-DH-CONFLICT-001 — How should conflicting values be resolved while preserving historical truth?

## Integrity rule
The most recently synchronized value is not automatically the authoritative truth.