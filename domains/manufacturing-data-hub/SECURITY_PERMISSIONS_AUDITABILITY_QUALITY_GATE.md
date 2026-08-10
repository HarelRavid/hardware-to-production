# 9.15 Security, Permissions, Auditability & Section Quality Gate

status: Researching
provenance: [GNR]
architecture_maturity: DEFINED

## Architecture maturity model
Section 9 uses three distinct maturity states:
1. **DEFINED** — conceptual architecture, objects, boundaries and decision rules are documented coherently.
2. **EVIDENCE VALIDATED** — architecture has been checked against applicable standards, authoritative literature and industrial examples; important claims have evidence/applicability statements.
3. **IMPLEMENTATION VALIDATED** — architecture has been exercised against at least one concrete implementation/reference model with representative objects, data flows and failure/conflict cases.

V1.0 architecture closure means DEFINED unless a higher maturity state is explicitly recorded. It does not mean evidence or implementation validation.

## Security model
Access should be based on role, responsibility, object sensitivity and action type rather than a single broad application permission.

## Permission actions
- discover/search
- read
- export
- create
- edit
- approve/release
- execute/write-back
- administer ontology/master data
- view sensitive supplier/commercial data

## Critical separation-of-duty examples
- author versus approver
- process parameter editor versus production release authority
- NCR creator versus concession approval where required
- AI recommendation versus authoritative disposition
- system administrator versus engineering content approval boundary

## OT / ICS cybersecurity boundary
The Atlas may connect IT, engineering and operational/manufacturing systems. Generic RBAC/auditability is therefore insufficient as the complete security model.

Evidence population must explicitly evaluate, where applicable:
- IEC 62443 family and other relevant industrial cybersecurity requirements/guidance;
- zones and conduits / segmentation concepts;
- industrial asset and service identities;
- least privilege for machine/service accounts;
- remote/vendor access;
- secure integration between enterprise IT and OT;
- controlled write paths into PLC/SCADA/MES or other operational systems;
- patch/change/configuration management constraints in validated production environments;
- logging, monitoring and incident-response evidence;
- safety/security interaction and consequences of loss of availability/integrity.

This section currently defines the gap and conceptual boundary only. It is not yet evidence validated against IEC 62443.

## Audit-event objects
- actor/service
- action
- semantic object
- before state
- after state
- timestamp
- reason/change reference
- approval/e-signature boundary
- source system
- correlation/execution ID

## Auditability principle
The Atlas must allow reconstruction not only of what data currently says, but who/what changed controlled meaning or state, when, under which authority and with which effectivity.

## Security/integration questions
1. Can read-only analytics credentials alter production systems?
2. Are machine/service identities distinct from human identities?
3. Are write-back paths explicitly allow-listed and validated?
4. Are sensitive supplier, employee or export-controlled data segregated as required?
5. Can historical engineering decisions and evidence be reconstructed after revisions?
6. Are AI/tool actions auditable as actions rather than appearing as human edits?
7. Does an IT-to-OT integration cross a trust zone/conduit boundary?
8. What happens to safety, quality and production if integrity or availability is lost?

## Decision objects
### D-DH-PERM-001 — Role/object/action permission policy
### D-DH-WRITE-001 — Which integrations may write to authoritative systems?
### D-DH-AUDIT-001 — What audit evidence is required for this controlled action?
### D-DH-SEG-001 — What data requires additional segregation/restriction?
### D-DH-OTSEC-001 — What OT/ICS security boundary and controls apply to this integration?

## Section 9 architecture coverage
All 9.1–9.15 sub-sections are **DEFINED** at conceptual architecture level.
They are not automatically EVIDENCE VALIDATED or IMPLEMENTATION VALIDATED.

- 9.1 Manufacturing ontology — DEFINED
- 9.2 ISA-95 / IEC 62264 hierarchy alignment — DEFINED
- 9.3 Equipment/resource model — DEFINED
- 9.4 Material/product genealogy — DEFINED
- 9.5 Process/recipe/version model — DEFINED
- 9.6 Parameter/measurement model — DEFINED
- 9.7 Historical metadata/effective dates — DEFINED
- 9.8 Claims/evidence/standards graph — DEFINED
- 9.9 Manufacturing-process Atlas — DEFINED
- 9.10 Decision-engine interfaces — DEFINED
- 9.11 PLM/ERP/MES/QMS/SCADA/historian boundaries — DEFINED
- 9.12 OPC UA / semantic integration boundary — DEFINED
- 9.13 Data ownership/authoritative source — DEFINED
- 9.14 Dashboards/analytics/AI interfaces — DEFINED
- 9.15 Security/permissions/auditability/OT boundary — DEFINED

## Validation targets
Before promoting Section 9 beyond DEFINED:
- create at least one representative Manufacturing Atlas reference implementation/mock dataset spanning product/process/resource/execution/measurement/evidence objects;
- exercise temporal/effectivity reconstruction;
- exercise conflicting source-of-record values;
- exercise claim/evidence/applicability linkage;
- exercise read/write authority and audit events;
- validate relevant concepts against ISA-95/IEC 62264, OPC UA and IEC 62443 evidence where applicable.

A reference implementation validates the integrated architecture; it is not necessary to create fifteen unrelated mock systems.

## Open population/evidence work
- ISA-95/IEC 62264 clause-level mapping
- OPC UA information-model examples and companion-specification boundaries
- IEC 62443 / OT-ICS cybersecurity applicability mapping
- system-of-record patterns and industrial architectures
- PLM/MES/QMS/historian integration case studies
- genealogy and temporal-data implementation patterns
- semantic/knowledge-graph industrial case studies
- manufacturing AI governance and validation evidence
- cybersecurity/identity/access standards applicable to manufacturing systems
- data-retention and electronic-record requirements by industry
- GNR verification

## Integrity gates before Podcast Ready
1. Definition/revision and execution/observation are distinct.
2. Historical truth is not reconstructed from current master data alone.
3. Stable semantic IDs are independent of source-system keys/navigation paths.
4. Authoritative source is defined at appropriate semantic granularity.
5. Atlas does not duplicate competing master data.
6. Derived analytics retain lineage/version/units/time basis.
7. AI outputs distinguish evidence, inference, recommendation and approval.
8. Write-back permissions are explicit and auditable.
9. Controlled changes preserve actor/time/reason/effectivity.
10. OT/ICS trust boundaries are explicit where operational systems are connected.
11. GNR remains visible until verified.

## Status
Section 9 Architecture definition: DEFINED
Knowledge population: OPEN
Evidence validation: OPEN
Implementation validation: OPEN
Podcast readiness: NOT READY