# 9.11 System-of-Record Boundaries

status: Researching
provenance: [GNR]

## Purpose
Define which system is authoritative for which class of manufacturing truth and how the Atlas references rather than duplicates source-of-record data.

## Typical system responsibilities
### PLM
- product definition/revision
- drawings/specifications
- engineering BOM
- engineering change/effectivity
- approved technical documents

### ERP
- item/master records
- procurement/commercial supplier records
- inventory/location/accounting state
- purchase/work-order planning boundary
- costing boundary

### MES
- manufacturing order execution
- routing/operation execution
- WIP status
- operator/equipment execution context
- genealogy/traceability
- production test/inspection results boundary

### QMS
- NCR/MRB/CAPA
- audits
- controlled quality records
- supplier quality events
- deviations/concessions boundary

### SCADA / machine control
- real-time process control
- setpoints/commands
- alarms/interlocks
- machine state

### Historian / time-series platform
- high-frequency process observations
- equipment/process time series
- event trends

### Data Hub / Atlas
- semantic identity/mapping
- cross-system relationships
- knowledge/claim/evidence links
- derived context/views
- decision-support interfaces
- lineage to authoritative records

## Authority principle
One fact may appear in multiple systems for workflow/performance reasons, but an authoritative owner/source must be defined for each semantic field or record class.

## Example authority matrix
Product revision -> PLM
Inventory quantity -> ERP
Actual operation execution -> MES
Raw high-frequency process signal -> historian/SCADA boundary
NCR disposition -> QMS
Engineering claim evidence maturity -> Knowledge OS
Cross-system semantic relationship -> Data Hub/Atlas

## Synchronization objects
- source-system key
- Atlas stable ID
- mapping/version
- sync timestamp
- source revision
- ingestion status
- lineage
- conflict state

## Conflict handling
If systems disagree:
1. preserve both observed values and provenance;
2. identify the defined authority;
3. flag conflict rather than silently overwrite;
4. correct the authoritative source through its governed workflow;
5. propagate corrected state while preserving historical truth.

## Decision objects
### D-DH-SOR-001 — Which system owns this fact/record?
### D-DH-DUP-001 — Is duplication justified, and how is lineage preserved?
### D-DH-CONFLICT-001 — How is cross-system disagreement resolved?

## Anti-patterns
- Data Hub becoming an ungoverned shadow PLM/ERP/MES/QMS;
- two systems both treated as authoritative for the same field;
- manual spreadsheet bridges without version/provenance;
- analytics-derived values written back as raw observations;
- deleting historical source data after normalization.

## Integrity rule
The Atlas integrates truth; it should not manufacture competing truths.