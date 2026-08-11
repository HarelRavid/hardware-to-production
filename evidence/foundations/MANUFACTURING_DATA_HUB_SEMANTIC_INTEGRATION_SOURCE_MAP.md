# Manufacturing Data Hub / Semantic Integration / OT-ICS — Evidence Source Map

status: BREADTH COMPLETE
campaign: A8
maps_to: MASTER_WBS Section 9; PODCAST_MAP Episodes 47–52
provenance: primary-source-first

## Purpose
Validate the Manufacturing Data Hub / Manufacturing Atlas conceptual architecture against authoritative external standards and specifications, while preserving the distinction between architecture DEFINED, EVIDENCE VALIDATED and IMPLEMENTATION VALIDATED.

## Primary backbone captured

### ISA-95 / IEC 62264 — enterprise-control integration and manufacturing hierarchy
ISA describes ISA-95 / IEC 62264 as an international standards series for integrating logistics/business systems with manufacturing control systems. It organizes activities into levels and defines interfaces/information shared between enterprise and manufacturing-control functions.

Engineering implications for the Atlas:
- Enterprise/Site/Area/production-resource hierarchy has a legitimate standards backbone;
- hierarchy/activity models are semantic alignment references, not a mandatory database schema;
- Level 3/4 integration is explicitly an information-boundary problem;
- integration does not eliminate authoritative ownership in ERP/MES/PLM/QMS/SCADA/historian systems.

### OPC UA — infrastructure plus information modelling
The OPC Foundation defines OPC UA as a platform-independent architecture with information modelling, discovery, access and security capabilities. Industrial information is represented through typed Nodes and References, while Companion Specifications add domain-specific models.

Engineering implications:
- OPC UA is not the complete Manufacturing Atlas business ontology;
- it is a strong semantic integration/information-exposure mechanism;
- applicable Companion Specifications should be evaluated before proprietary semantics are invented;
- PLC tags, BrowseNames, NodeIds and source-system keys must not automatically become durable cross-system business identities;
- model/version/effectivity governance remains necessary even with semantic protocols.

### ISA/IEC 62443 — OT/IACS cybersecurity boundary
ISA describes ISA/IEC 62443 as a standards series defining requirements and processes for secure industrial automation and control systems across lifecycle responsibilities.

Engineering implications:
- Data Hub connectivity into operational systems creates an OT/IACS trust boundary, not merely an application RBAC problem;
- segmentation/zones/conduits, identity, remote access, monitoring, change control and write authority require explicit treatment;
- analytics/AI access and operational write-back are different integration classes;
- detailed role/part/security-level applicability remains clause-level Pass-2 work.

### NIST Digital Thread — traceability, semantics and durable identity
NIST's Digital Thread for Manufacturing work emphasizes communication of product definition through design, manufacturing and quality, and return of manufacturing/inspection information to engineering. NIST explicitly identifies globally unique identifiers, semantic product/manufacturing information, authorization/authentication and traceability of trustworthy product data as digital-thread needs.

Engineering implications:
- cross-lifecycle traceability requires more than copying current master data into one database;
- durable identifiers and semantic relationships are legitimate architecture requirements;
- data trust includes who may use/change data and who did what to it;
- the Atlas provenance/audit model is directionally supported by external digital-thread research.

### NIST manufacturing traceability — provenance, pedigree and linked traceability records
NIST manufacturing supply-chain traceability work defines product provenance around chronology of origin, development, ownership, location and changes, and emphasizes pedigree/validation and linked traceability records across manufacturing ecosystems.

Engineering implications:
- genealogy/provenance is fundamentally historical and event-linked;
- current-state master data cannot, by itself, reconstruct all historical production truth after revisions or changes;
- traceability chains should preserve the relationship between physical/product identity, transformations/events and evidence;
- exact internal bitemporal implementation remains an Atlas design choice rather than a direct NIST prescription.

## Evidence-backed architecture checks
### Check 1 — ISA-95 hierarchy alignment
Result: SUPPORTED AT BREADTH LEVEL.
The Atlas resource hierarchy is directionally aligned with ISA-95/IEC 62264 concepts. Exact naming and implementation depth remain context-specific.

### Check 2 — OPC UA as semantic integration, not master ontology
Result: SUPPORTED.
OPC UA explicitly provides infrastructure and information-modelling mechanisms; domain-specific semantics are layered through information models/Companion Specifications.

### Check 3 — Stable semantic identity independent of source navigation key
Result: SUPPORTED AS ARCHITECTURE SYNTHESIS.
NIST digital-thread work explicitly identifies GUID/traceability needs; OPC UA defines identifiers within its information model. The Atlas still needs a governed cross-system identity layer rather than assuming one source identifier is globally permanent.

### Check 4 — System-of-record boundaries
Result: SUPPORTED DIRECTION / IMPLEMENTATION-SPECIFIC.
ISA-95 supports explicit enterprise/manufacturing integration boundaries. NIST digital-thread work supports lifecycle information exchange and traceability. Exact PLM/ERP/MES/QMS/SCADA/historian authority must be defined by semantic object/attribute in each implementation.

### Check 5 — Historical truth requires temporal/provenance context
Result: SUPPORTED AT BREADTH LEVEL.
NIST traceability/provenance work treats origin, changes and chronology as essential. Therefore an Atlas must retain historical relationships/effectivity rather than reconstructing an old build solely from today's master data. Bitemporal schema mechanics remain an implementation choice.

### Check 6 — OT security cannot be reduced to RBAC
Result: SUPPORTED AT FAMILY LEVEL.
ISA/IEC 62443 explicitly addresses secure IACS across lifecycle and IT/OT boundaries. Detailed controls/applicability remain Pass 2.

### Check 7 — Read-only analytics and write-back are distinct authority classes
Result: STRONG ENGINEERING DIRECTION.
NIST digital-thread security work supports authorization/authentication/traceability of data use and change; IEC 62443 provides the OT security family context. Exact write-back patterns require architecture/risk-specific validation.

## Applicability Statement reference examples — A8 breadth
Object: `AS-A8-ISA95-001`
Standard family: ISA-95 / IEC 62264
Claim: The Manufacturing Atlas may align enterprise/site/area/production-resource concepts and Level 3/4 information boundaries to ISA-95 models.
Applies when: modelling manufacturing operations/resources and enterprise-to-manufacturing information exchange.
Does not imply: five mandatory physical software tiers, a complete Atlas ontology, or automatic ownership by a system merely because of nominal ISA-95 level.
Evidence maturity: BREADTH VERIFIED; clause-level mapping OPEN.
Decision linkage: D-DH-HIER-001 / system-of-record and hierarchy decisions.

Object: `AS-A8-OPCUA-001`
Specification family: OPC UA Core + applicable Companion Specifications
Claim: OPC UA can expose typed industrial information and domain models for semantic interoperability.
Applies when: systems/devices expose or consume OPC UA information models.
Does not imply: automatic resolution of enterprise master-data ownership, temporal truth, genealogy or business decision semantics.
Evidence maturity: BREADTH VERIFIED.
Decision linkage: D-DH-SEM-001 / integration mapping decisions.

Object: `AS-A8-62443-001`
Standard family: ISA/IEC 62443
Claim: A Manufacturing Data Hub interfacing with IACS/OT should evaluate industrial cybersecurity requirements beyond generic application permissions.
Applies when: data flows cross into/out of industrial automation/control environments, especially where write/control capability or remote access exists.
Does not imply: identical security requirements/security level for every Atlas deployment.
Evidence maturity: FAMILY-LEVEL VERIFIED; clause-level applicability OPEN.
Decision linkage: D-DH-OTSEC-001.

Object: `AS-A8-NIST-PROV-001`
Source family: NIST Digital Thread + Manufacturing Supply Chain Traceability
Claim: Manufacturing traceability architecture should preserve provenance/chronology and trustworthy links between product/data changes and lifecycle events.
Applies when: reconstructing genealogy, configuration, source/evidence lineage or historical production state.
Does not imply: blockchain is required, or that NIST prescribes the Atlas's database technology/bitemporal schema.
Evidence maturity: BREADTH VERIFIED.
Decision linkage: temporal/effectivity, genealogy, audit/provenance and semantic-ID decisions.

## Claim register
### C-DH-001 — ISA-95/IEC 62264 is an appropriate alignment backbone for manufacturing hierarchy and enterprise-control information boundaries
status: STRONG / APPLICABILITY-SCOPED

### C-DH-002 — OPC UA provides semantic information-modelling and access infrastructure but is not by itself a complete Manufacturing Atlas business ontology
status: STRONG

### C-DH-003 — Applicable OPC UA Companion Specifications should be evaluated before inventing proprietary device/domain models
status: STRONG ENGINEERING DIRECTION

### C-DH-004 — Source-system keys, PLC tags and OPC UA navigation identifiers should not automatically be treated as permanent cross-system semantic identities
status: STRONG ARCHITECTURE SYNTHESIS / NIST GUID NEED CORROBORATION

### C-DH-005 — Current master data alone is insufficient to reconstruct historical production truth when definitions/revisions/effectivity change
status: STRONG BREADTH SYNTHESIS / PROVENANCE SUPPORTED

### C-DH-006 — A connected Manufacturing Data Hub must treat OT/IACS cybersecurity as an architectural boundary, not only a user-permission feature
status: STRONG / FAMILY-LEVEL VERIFIED

### C-DH-007 — Read-only analytics/AI and authoritative operational write-back should be different permission/integration classes
status: STRONG ENGINEERING DIRECTION

### C-DH-008 — Semantic integration does not remove system-of-record ownership
status: STRONG SYNTHESIS

### C-DH-009 — Genealogy should be event/relationship based and preserve provenance through transformations and configuration changes
status: STRONG BREADTH SYNTHESIS / NIST TRACEABILITY SUPPORTED

## Podcast editorial guardrails
Do not say:
- “ISA-95 says your factory must have exactly these software systems.”
- “OPC UA gives you a complete manufacturing ontology.”
- “If everything uses OPC UA, integration is solved.”
- “A PLC tag is the digital identity of the physical asset forever.”
- “A historian is automatically the source of truth for every historical question.”
- “Read access and write access are basically the same integration problem.”
- “IEC 62443 compliant” without identifying applicable role/part/scope/evidence.
- “Blockchain is required for manufacturing traceability.”

Teach instead:
1. semantic meaning;
2. authoritative ownership;
3. durable identity and mapping;
4. revision/effectivity/time;
5. lineage/genealogy/provenance;
6. read/write authority;
7. OT trust/security boundary;
8. evidence and applicability.

## Breadth gaps explicitly bounded for Pass 2
1. ISA-95/IEC 62264 clause/object-level mapping;
2. concrete PLM/ERP/MES/QMS/historian authority case patterns;
3. IEC 62443 zones/conduits, role/part and security-level applicability;
4. OPC UA Companion Specification implementation/versioning cases;
5. exact bitemporal/effectivity implementation pattern;
6. AI/analytics provenance and controlled write-back governance;
7. episode-ready industrial case studies;
8. representative integrated Atlas mock/reference dataset for IMPLEMENTATION VALIDATED status.

## Pass-2 targets
- ISA-95/IEC 62264 clause/object mapping;
- one ISA-95 Applicability Statement worked example with clause evidence;
- IEC 62443 role/part/applicability map and OT boundary example;
- OPC UA NodeId/BrowseName/semantic-ID comparison;
- Companion Specification mapping example;
- bitemporal/effectivity worked example;
- genealogy reconstruction example after engineering change;
- conflicting system-of-record resolution case;
- read-only analytics versus controlled write-back architecture;
- integrated mock/reference Manufacturing Atlas dataset.

## Readiness
Source map: BREADTH COMPLETE
Critical claims identified: YES
Primary-source backbone: ISA-95 + OPC UA + ISA/IEC 62443 + NIST DIGITAL THREAD/TRACEABILITY CAPTURED
Applicability Statements: BREADTH REFERENCE SET CAPTURED
Implementation validation: OPEN
Podcast Ready: NO