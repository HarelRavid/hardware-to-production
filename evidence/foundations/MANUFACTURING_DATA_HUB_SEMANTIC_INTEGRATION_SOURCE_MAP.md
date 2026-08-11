# Manufacturing Data Hub / Semantic Integration / OT-ICS — Evidence Source Map

status: IN PROGRESS — ISA-95/OPC-UA/OT-ICS BACKBONE CAPTURED
campaign: A8
maps_to: MASTER_WBS Section 9; PODCAST_MAP Episodes 47–52
provenance: primary-source-first

## Purpose
Validate the Manufacturing Data Hub / Manufacturing Atlas conceptual architecture against authoritative external standards and specifications, while preserving the distinction between architecture DEFINED, EVIDENCE VALIDATED and IMPLEMENTATION VALIDATED.

## Primary backbone captured

### ISA-95 / IEC 62264 — enterprise-control integration and manufacturing hierarchy
ISA describes ISA-95 / IEC 62264 as an international standards series for integrating logistics/business systems with manufacturing control systems. It organizes activities into levels and defines interfaces/information shared between enterprise and manufacturing-control functions.

Part 1 covers models/terminology, manufacturing operations/control scope, physical-asset organization, functions and information exchange. Part 2 specifies conceptual interface content between Level 3 manufacturing systems and Level 4 business systems.

Engineering implications for the Atlas:
- the Enterprise/Site/Area/production-resource hierarchy has a legitimate standards backbone;
- hierarchy and activity models should be used as semantic alignment/reference, not blindly copied as a database schema;
- Level 3/4 integration is an explicit information-boundary problem;
- the Atlas must preserve source-system authority rather than becoming an accidental replacement ERP/MES.

### OPC UA — infrastructure plus information modelling
The OPC Foundation defines OPC UA as a platform-independent, secure, extensible service-oriented architecture with information modelling, discovery, transport, information access and security capabilities.

OPC UA represents industrial information through an AddressSpace of typed Nodes and References. Information models can define Objects, Variables, Methods, DataTypes and relationships.

Engineering implications:
- OPC UA is not itself the complete business ontology of the Manufacturing Atlas;
- it is a strong semantic integration/information-exposure mechanism;
- a PLC tag or vendor BrowseName/NodeId must not automatically become the Atlas's durable business identity;
- stable semantic identity and source-system keys/navigation paths should remain distinct concepts.

### OPC UA Companion Specifications
The OPC Foundation states that Companion Specifications typically define domain-specific information models on top of OPC UA and can include both a written specification and machine-readable UANodeSet.

Engineering implications:
- use applicable Companion Specifications before inventing proprietary machine/domain semantics;
- Companion Specs improve semantic interoperability but do not eliminate the need for plant/product-specific mappings and governance;
- model version/effectivity must be retained because companion and vendor implementations evolve.

### ISA/IEC 62443 — OT/IACS cybersecurity boundary
ISA describes ISA/IEC 62443 as a standards series defining requirements and processes for implementing and maintaining secure industrial automation and control systems, explicitly bridging operations/IT and process safety/cybersecurity.

Engineering implications:
- Data Hub connectivity into operational systems creates an OT/IACS security boundary, not merely an application RBAC problem;
- read/write paths, identities, remote access, segmentation, change control and monitoring require explicit security treatment;
- analytics/AI access should default toward controlled/read-only patterns unless operational write authority is intentionally engineered and validated;
- detailed zones/conduits/security-level applicability requires clause-level Pass-2 work.

## Evidence-backed architecture checks
### Check 1 — ISA-95 hierarchy alignment
Result: SUPPORTED AT BREADTH LEVEL.
The Atlas resource hierarchy is directionally aligned with ISA-95/IEC 62264 concepts. Exact naming and implementation depth remain context-specific.

### Check 2 — OPC UA as semantic integration, not master ontology
Result: SUPPORTED.
OPC UA explicitly provides infrastructure and information-modelling mechanisms; domain-specific semantics are layered through information models/Companion Specifications.

### Check 3 — Stable semantic identity independent of source navigation key
Result: STRONG ARCHITECTURE SYNTHESIS.
OPC UA NodeId/BrowseName have defined roles inside UA information models, but Atlas-level durable identity across ERP/MES/PLM/QMS/SCADA/historian systems remains an architectural governance requirement rather than a direct OPC UA rule.

### Check 4 — System-of-record boundaries
Result: STRONG DIRECTION, NEEDS CROSS-SYSTEM CASE EVIDENCE.
ISA-95 supports explicit enterprise/manufacturing integration boundaries, but exact PLM/ERP/MES/QMS/SCADA/historian authority is implementation-specific.

### Check 5 — OT security cannot be reduced to RBAC
Result: SUPPORTED AT FAMILY LEVEL.
ISA/IEC 62443 explicitly addresses secure IACS across lifecycle and IT/OT/safety boundaries. Detailed controls/applicability remain Pass 2.

## Applicability Statement reference example — draft A8
Object: `AS-A8-ISA95-001`

Standard family: ISA-95 / IEC 62264
Claim: The Manufacturing Atlas may align enterprise/site/area/production-resource concepts and Level 3/4 information boundaries to ISA-95 models.
Applies when: modelling manufacturing operations/resources and enterprise-to-manufacturing information exchange.
Does not imply: that every company must deploy five physical software tiers; that ISA-95 defines the entire Atlas ontology; or that a specific ERP/MES/SCADA product owns a semantic object solely because of its nominal ISA-95 level.
Evidence maturity: BREADTH VERIFIED from ISA overview; clause-level mapping OPEN.
Decision linkage: D-DH-HIER-001 / system-of-record and hierarchy decisions.

Object: `AS-A8-OPCUA-001`

Specification family: OPC UA Core + applicable Companion Specifications
Claim: OPC UA can expose typed industrial information and domain models for semantic interoperability.
Applies when: systems/devices expose or consume OPC UA information models.
Does not imply: that OPC UA automatically resolves enterprise master-data ownership, temporal truth, genealogy or business decision semantics.
Evidence maturity: BREADTH VERIFIED from OPC Foundation.
Decision linkage: D-DH-SEM-001 / integration mapping decisions.

Object: `AS-A8-62443-001`

Standard family: ISA/IEC 62443
Claim: A Manufacturing Data Hub that interfaces with IACS/OT should evaluate industrial cybersecurity requirements beyond generic application permissions.
Applies when: data flows cross into/out of industrial automation/control environments, especially where write/control capability or remote access exists.
Does not imply: that every Atlas deployment has identical security requirements or security level; applicability depends on system role, risk, architecture and lifecycle responsibility.
Evidence maturity: FAMILY-LEVEL VERIFIED; clause-level applicability OPEN.
Decision linkage: D-DH-OTSEC-001.

## Claim register
### C-DH-001 — ISA-95/IEC 62264 is an appropriate alignment backbone for manufacturing hierarchy and enterprise-control information boundaries
status: STRONG / APPLICABILITY-SCOPED

### C-DH-002 — OPC UA provides semantic information-modelling and access infrastructure but is not by itself a complete Manufacturing Atlas business ontology
status: STRONG

### C-DH-003 — Applicable OPC UA Companion Specifications should be evaluated before inventing proprietary device/domain models
status: STRONG ENGINEERING DIRECTION

### C-DH-004 — Source-system keys, PLC tags and OPC UA navigation identifiers should not automatically be treated as permanent cross-system semantic identities
status: STRONG ARCHITECTURE SYNTHESIS
Need Pass-2 implementation/case corroboration.

### C-DH-005 — Current master data alone is insufficient to reconstruct historical production truth when definitions/revisions/effectivity change
status: HIGH PRIORITY ARCHITECTURE CLAIM
Need temporal/genealogy standards and implementation evidence in Pass 2.

### C-DH-006 — A connected Manufacturing Data Hub must treat OT/IACS cybersecurity as an architectural boundary, not only a user-permission feature
status: STRONG / FAMILY-LEVEL VERIFIED

### C-DH-007 — Read-only analytics/AI and authoritative operational write-back should be different permission/integration classes
status: STRONG ENGINEERING DIRECTION
Need IEC 62443 and industrial architecture depth in Pass 2.

### C-DH-008 — Semantic integration does not remove system-of-record ownership
status: STRONG SYNTHESIS

## Podcast editorial guardrails
Do not say:
- “ISA-95 says your factory must have exactly these software systems.”
- “OPC UA gives you a complete manufacturing ontology.”
- “If everything uses OPC UA, integration is solved.”
- “A PLC tag is the digital identity of the physical asset forever.”
- “Read access and write access are basically the same integration problem.”
- “IEC 62443 compliance” without identifying applicable role/part/scope/evidence.

Teach instead:
1. semantic meaning;
2. authoritative ownership;
3. identity and mapping;
4. revision/effectivity/time;
5. lineage/genealogy;
6. read/write authority;
7. OT trust/security boundary;
8. evidence and applicability.

## Breadth gaps remaining
1. temporal/effectivity/genealogy implementation evidence;
2. PLM/ERP/MES/QMS/historian system-of-record case patterns;
3. IEC 62443 zones/conduits and role/part applicability at useful depth;
4. OPC UA Companion Specification implementation/versioning cases;
5. one representative Atlas mock/reference dataset to support IMPLEMENTATION VALIDATED later;
6. AI/analytics provenance and write-back governance evidence;
7. episode-ready case studies for Episodes 47–52.

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
Source map: IN PROGRESS
Critical claims identified: YES
Primary-source backbone: ISA-95 + OPC UA + ISA/IEC 62443 CAPTURED
Applicability Statements: FIRST DRAFTS CAPTURED
Implementation validation: OPEN
Podcast Ready: NO