# 9.15 Security, Permissions, Auditability & Section Quality Gate

status: Researching
provenance: [GNR]

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

## Decision objects
### D-DH-PERM-001 — Role/object/action permission policy
### D-DH-WRITE-001 — Which integrations may write to authoritative systems?
### D-DH-AUDIT-001 — What audit evidence is required for this controlled action?
### D-DH-SEG-001 — What data requires additional segregation/restriction?

## Section 9 architecture coverage
- 9.1 Manufacturing ontology: COMPLETE architecture
- 9.2 ISA-95 / IEC 62264 hierarchy alignment: COMPLETE architecture
- 9.3 Equipment/resource model: COMPLETE architecture
- 9.4 Material/product genealogy: COMPLETE architecture
- 9.5 Process/recipe/version model: COMPLETE architecture
- 9.6 Parameter/measurement model: COMPLETE architecture
- 9.7 Historical metadata/effective dates: COMPLETE architecture
- 9.8 Claims/evidence/standards graph: COMPLETE architecture
- 9.9 Manufacturing-process Atlas: COMPLETE architecture
- 9.10 Decision-engine interfaces: COMPLETE architecture
- 9.11 PLM/ERP/MES/QMS/SCADA/historian boundaries: COMPLETE architecture
- 9.12 OPC UA / semantic integration boundary: COMPLETE architecture
- 9.13 Data ownership/authoritative source: COMPLETE architecture
- 9.14 Dashboards/analytics/AI interfaces: COMPLETE architecture
- 9.15 Security/permissions/auditability: COMPLETE architecture

## Open population/evidence work
- ISA-95/IEC 62264 clause-level mapping
- OPC UA information-model examples and companion-specification boundaries
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
10. GNR remains visible until verified.

## Status
Section 9 Architecture: COMPLETE
Knowledge population: OPEN
Evidence verification: OPEN
Podcast readiness: NOT READY

## Next architecture work
Audit/reconcile Sections 0–2 against MASTER_WBS.md, then close Section 10 Case Studies & Podcast Synthesis architecture.