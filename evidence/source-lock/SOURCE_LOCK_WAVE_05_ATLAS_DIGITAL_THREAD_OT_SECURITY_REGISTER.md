# Source-Lock Wave 05 — Manufacturing Atlas / Digital Thread / OT Security Shared Source Register

status: SHARED SOURCE REGISTER LOCKED
checked: 2026-09-19
scope: EP47 / EP48 / EP49 / EP50 / EP51 / EP52 + P2.08 / P2.09
backbone: Manufacturing Atlas / Digital Thread / Semantic Integration / OT-ICS Cybersecurity / Recovery

## 1. Purpose

Lock the authoritative/public source layer shared by the connected-manufacturing episodes while preserving strict separation among:

1. information ownership and manufacturing semantics;
2. product/unit genealogy, provenance and traceability;
3. OPC UA connectivity/information modelling;
4. Manufacturing Atlas decision-support synthesis;
5. OT/IACS cybersecurity responsibilities and controls;
6. production/evidence recovery after cyber/configuration incidents.

No episode may treat one software category, protocol or security standard as a complete architecture by itself.

## 2. Manufacturing integration / semantics source register

### W5-S01 — ANSI/ISA-95.00.01-2025 / IEC 62264-1 Modified
Owner: ISA
Title: Enterprise-Control System Integration — Part 1: Models and Terminology
Current ISA publication checked: ANSI/ISA-95.00.01-2025 (IEC 62264-1 Mod)
Public announcement:
https://www.isa.org/news-press-releases/2025/april/update-to-isa-95-standard-addresses-integration-of
Public series page:
https://www.isa.org/standards-and-publications/isa-standards/isa-95-standard

Current-status finding:
The 2025 Part 1 replaces the 2010 ISA Part 1 edition.

Publicly supportable scope:
- manufacturing operations/control domain scope;
- organization of physical assets;
- functions at enterprise/control interfaces;
- information shared between enterprise and manufacturing/control functions.

Episode use:
EP47/EP51.

Guardrail:
ISA-95 is a reference model/terminology/information-integration standard. It is not a mandatory software stack, database schema or network-security architecture.

### W5-S02 — ISA-95 other current public series context
Public ISA series page lists, among others:
- Part 2: ANSI/ISA-95.00.02-2018;
- Part 3: ANSI/ISA-95.00.03-2013;
- later Parts 4–8 in the ISA-95 family.

Use:
show-notes/current-series context only unless a specific claim requires exact part verification.

Guardrail:
Do not overstate one Part 1 public summary as the entire IEC 62264/ISA-95 series.

### W5-S03 — OPC UA infrastructure + Companion Specifications
Owner: OPC Foundation
Source:
https://opcfoundation.org/about/opc-technologies/opc-ua/ua-companion-specifications/

Public support:
- OPC UA provides infrastructure for discovery, transport, information access, security and object-based information models;
- information models are layered on top of the infrastructure;
- Companion Specifications define domain/device/use-case information models and profiles.

Episode use:
EP51.

Strong boundary:
OPC UA can transport/expose structured semantics but does not automatically define the organization's business ontology, master-data ownership, genealogy, effectivity or decision logic.

### W5-S04 — NIST Digital Thread for Manufacturing
Owner: NIST
Source:
https://www.nist.gov/programs-projects/digital-thread-manufacturing
Updated: 2026-08-12.

Public support:
- digital thread connects product design information with manufacturing and quality and returns manufacturing/inspection information back to engineering;
- gaps/needs include globally unique identifiers, semantic product/manufacturing information and trust/security of data assets.

Episode use:
EP48/EP49/EP50/EP51.

### W5-S05 — NIST AMS 300-12 UUID research
Owner: NIST
Title: Research Results and Recommendations for Universally Unique Identifiers in Product Data Standards
Published: 2024-07-16
Source:
https://www.nist.gov/publications/research-results-and-recommendations-universally-unique-identifiers-product-data

Public support:
- digital thread is an authoritative integrated information flow across lifecycle phases;
- persistent/universally unique identifiers linked with human-readable IDs help track engineering information across lifecycle and systems.

Episode use:
EP48/EP51.

Guardrail:
A UUID alone does not create provenance, semantic correctness or authoritative ownership.

### W5-S06 — NIST IR 8536 final traceability meta-framework
Owner: NIST / NCCoE
Title: Supply Chain Traceability Principles: A Manufacturing Meta-Framework
Final publication: 2026-09-09
Sources:
https://www.nist.gov/publications/supply-chain-traceability-principles-manufacturing-meta-framework
https://csrc.nist.gov/pubs/ir/8536/final

Public support:
- practical conceptual framework to organize, link and query traceability data across diverse manufacturing ecosystems;
- continuous temporally ordered provenance chain;
- pedigree/provenance, interoperable interfaces and selective disclosure;
- does not require one centralized repository.

Episode use:
EP48 and supporting EP49/EP52.

Current-status finding:
the 2024 and 2025 public drafts are obsolete; the final September 2026 report is authoritative current NIST record.

### W5-S07 — NIST Digital Thread for Smart Manufacturing
Owner: NIST
Source:
https://www.nist.gov/programs-projects/digital-thread-smart-manufacturing

Public support:
information silos across lifecycle processes are connected into an integrated digital thread spanning design, manufacturing and product support.

Episode use:
supporting digital-thread context.

## 3. OT / IACS cybersecurity source register

### W5-S08 — NIST SP 800-82 Rev.3
Owner: NIST
Title: Guide to Operational Technology (OT) Security
Final publication: 2023-09
Source:
https://csrc.nist.gov/pubs/sp/800/82/r3/final

Current status checked 2026-09-19:
Rev.3 remains the current final publication; a 2024 planning note identifies potential future errata/updates but does not change the final publication.

Public support:
OT security must account for unique performance, reliability and safety requirements; the guide discusses OT topologies, threats, vulnerabilities and recommended countermeasures.

Episode use:
EP52 primary open OT-security guidance source.

Guardrail:
NIST SP 800-82 is guidance, not a universal law or one mandated network topology.

### W5-S09 — IEC 62443-2-1:2024
Owner: IEC
Title: Security for industrial automation and control systems — Part 2-1: Security program requirements for IACS asset owners
Edition: 2.0
Publication: 2024-08-07
Source:
https://webstore.iec.ch/en/publication/62883

Public support:
asset-owner security-program policy/procedure requirements.

Current watch:
IEC lists stability date 2026; re-check immediately before final publication/recording lock.

Episode use:
EP52 responsibility mapping.

### W5-S10 — IEC 62443-2-4:2023
Owner: IEC
Title: Security program requirements for IACS service providers
Edition: 2.0
Publication: 2023-12-15
Source:
https://webstore.iec.ch/en/publication/67631
Stability date: 2027.

Public support:
security-related processes that IACS service providers can offer during integration and maintenance; public summary explicitly distinguishes asset owner, service provider and product supplier relationships.

Episode use:
EP52 responsibility mapping.

### W5-S11 — IEC 62443-3-2:2020
Owner: IEC
Title: Security risk assessment for system design
Edition: 1.0
Publication: 2020-06-24
Source:
https://webstore.iec.ch/en/publication/30727
Stability date: 2027.

Public support:
- define system under consideration;
- partition into zones and conduits;
- assess risk by zone/conduit;
- establish target security levels;
- document security requirements.

Episode use:
EP52 system architecture context.

Guardrail:
Do not prescribe a universal zone/conduit layout or target security level.

### W5-S12 — IEC 62443-3-3:2013
Owner: IEC
Title: System security requirements and security levels
Edition: 1.0
Publication: 2013-08-07
Source:
https://webstore.iec.ch/en/publication/7033
Stability date: 2027.

Public support:
technical system requirements/security-level capability framework for IACS within stated scope.

Episode use:
show-notes/current family context and generic security-requirement layer.

### W5-S13 — IEC 62443-4-1:2018
Owner: IEC
Title: Secure product development lifecycle requirements
Edition: 1.0
Publication: 2018-01-15
Source:
https://webstore.iec.ch/en/publication/33615
Stability date: 2027.

Public support:
secure development lifecycle requirements for IACS product developers/maintainers; public IEC page explicitly states these apply to developer/maintainer rather than integrator or user.

Episode use:
EP52 product-supplier responsibility boundary.

### W5-S14 — IEC 62443-4-2:2019
Owner: IEC
Title: Technical security requirements for IACS components
Edition: 1.0
Publication: 2019-02-27
Source:
https://webstore.iec.ch/en/publication/34421
Corrigendum 2022 included; stability date 2027.

Public support:
technical security requirements for IACS components and component security-capability levels.

Episode use:
EP52 component/product context only.

## 4. Shared manufacturing-information claims

### W5-C01 — system categories do not define manufacturing truth by themselves
Status: VERIFIED PREMISE + V6 SYNTHESIS
Support: W5-S01/S04/S07.
Claim:
PLM/ERP/MES/QMS/SCADA/historian roles are useful implementation categories, but authoritative ownership must be defined by information object/attribute/decision in the actual organization.

Guardrail:
Do not claim ISA-95 normatively assigns every company-specific system-of-record role.

### W5-C02 — ISA-95 is a manufacturing/enterprise integration reference, not a mandatory software stack
Status: VERIFIED PUBLIC SCOPE
Support: W5-S01/S02.

### W5-C03 — connectivity, syntax and semantics are different problems
Status: VERIFIED + V6 SYNTHESIS
Support: W5-S03.
Claim:
an OPC UA endpoint/API/broker can move data while the consumer still lacks product/operation/recipe meaning.

### W5-C04 — OPC UA does not automatically create a complete enterprise/manufacturing ontology
Status: VERIFIED
Support: W5-S03.
Claim:
OPC UA infrastructure plus domain information models can support semantic interoperability; business ownership/context remains implementation/governance work.

### W5-C05 — applicable Companion Specifications should be evaluated before inventing proprietary domain models
Status: VERIFIED ENGINEERING DIRECTION
Support: W5-S03.

### W5-C06 — durable identity matters across lifecycle/system boundaries
Status: VERIFIED
Support: W5-S04/S05.
Claim:
persistent/global identifiers can support cross-system/lifecycle traceability.

Boundary:
source-system tag/BrowseName/NodeId/DB primary key is not automatically a durable enterprise identity.

### W5-C07 — serial number alone is not full genealogy
Status: VERIFIED + V6 SYNTHESIS
Support: W5-S06 plus Waves 01–03.
Claim:
reconstructable product history can require linked material/component, process, equipment, recipe, measurement, rework and disposition events.

### W5-C08 — current master data alone may be insufficient to reconstruct historical production truth
Status: VERIFIED + V6 SYNTHESIS
Support: W5-S06 provenance/chronology + Wave 01 effectivity/history.

### W5-C09 — documents are source containers, not complete engineering claims
Status: V6 LOCKED AS SYNTHESIS
Claim:
claim/evidence/applicability/configuration/provenance relationships must remain explicit if the document is to support a decision later.

### W5-C10 — Manufacturing Atlas / ATLAS 10 is internal synthesis
Status: V6 LOCKED AS SYNTHESIS
Boundary:
no claim that an external standard defines the Atlas or its exact object graph/decision path.

### W5-C11 — AI/analytics output does not replace evidence lineage
Status: V6 GLOBAL INVARIANT
Support: provenance/digital-thread source family.
Claim:
derived output needs source/input/model/version/context lineage appropriate to decision consequence.

## 5. Shared OT-security claims

### W5-C12 — OT security must account for safety, reliability and availability consequences
Status: VERIFIED OPEN SOURCE
Support: W5-S08.

### W5-C13 — read-only analytics and operational write-back are distinct risk/authority classes
Status: VERIFIED PREMISE + V6 SYNTHESIS
Support: W5-S08 + IEC 62443 responsibility/system-risk family.
Claim:
write/control authority can alter physical production/evidence and requires stronger architecture/change/authorization consideration than passive observation.

### W5-C14 — OT security is not merely application RBAC
Status: VERIFIED
Support: W5-S08/W5-S11/W5-S12.
Claim:
system boundaries, segmentation/zones/conduits, remote connectivity, asset/config awareness, monitoring and recovery are relevant beyond ordinary app permissions.

### W5-C15 — IEC 62443 responsibilities are distributed by role
Status: VERIFIED PUBLIC SCOPE
Support:
- asset owner: W5-S09;
- service provider: W5-S10;
- system risk/zones/conduits: W5-S11;
- system security requirements: W5-S12;
- product developer/maintainer: W5-S13;
- component requirements: W5-S14.

Guardrail:
Do not imply one party owns every requirement or that every part applies to every deployment.

### W5-C16 — zones/conduits are risk-design concepts, not a universal network drawing
Status: VERIFIED + SCRIPT GUARDRAIL
Support: W5-S11.

### W5-C17 — recovery after cyber/configuration incident is more than restarting machines
Status: VERIFIED PREMISE + V6 GLOBAL INVARIANT
Support: W5-S08 + Waves 01/02.
Claim:
production recovery may require restoring trustworthy configuration, WIP/genealogy, quality state and release evidence in addition to technical service restoration.

### W5-C18 — broad enterprise/cloud connectivity into OT should be consequence/risk controlled
Status: VERIFIED + V6 SYNTHESIS
Support: W5-S08 + IEC 62443 system-risk family.
Guardrail:
do not prescribe one universal DMZ/topology.

## 6. Episode mapping

EP47 — systems of record / PLM-ERP-MES-QMS-SCADA-historian roles:
W5-S01/S02 + internal ownership synthesis.

EP48 — product genealogy / recipes / parameters / measurements:
W5-S04/S05/S06 + Waves 01/02.

EP49 — standards/claims/evidence knowledge graph:
Wave 01 source/claim discipline + W5 provenance sources; graph structure is internal synthesis.

EP50 — Manufacturing Atlas decision system:
P2.08 / ATLAS 10 internal synthesis; embedded technical claims inherit their own locked sources.

EP51 — OPC UA / ISA-95 / semantic integration:
W5-S01/S02/S03/S04/S05.

EP52 — engineering-grade manufacturing data + OT security:
W5-S08–S14 + P2.09 + prior waves.

## 7. Hard guardrails

1. ISA-95 is not a mandatory ERP/MES/SCADA stack.
2. ISA-95 levels are not an OT cybersecurity segmentation standard.
3. ERP/MES/PLM/QMS ownership is organization/object specific.
4. OPC UA endpoint does not equal semantic architecture.
5. OPC UA security features do not equal a complete OT security program.
6. PLC tag/BrowseName/NodeId/database key is not automatically durable global identity.
7. UUID does not by itself create provenance or authority.
8. Serial number alone does not equal genealogy.
9. Blockchain is not required for traceability; NIST IR 8536 is technology-neutral.
10. No IEC 62443 clause-level requirement/security-level target from memory.
11. No one universal zones/conduits topology.
12. NIST SP 800-82 is guidance, not law.
13. Read-only and write-back connectivity must not be treated as equivalent risk.
14. Cyber restart is not full manufacturing/evidence recovery.
15. AI synthesis/model output must not become untraceable release truth.
16. Exact legal/regulatory OT cybersecurity obligations require jurisdiction/sector source.
17. IEC 62443-2-1:2024 has a 2026 stability date and must be rechecked immediately before final recording/publication.

## 8. Current revision/status watch

Checked 2026-09-19:
- ANSI/ISA-95.00.01-2025 is current ISA Part 1 and replaces the 2010 Part 1.
- OPC Foundation Companion-Spec architecture remains current public guidance.
- NIST IR 8536 final superseded the 2024/2025 drafts on 2026-09-09.
- NIST SP 800-82 Rev.3 remains current final, with a 2024 planning note for possible future errata/update.
- IEC 62443-2-1:2024 Ed2 stability date 2026 — publication recheck mandatory.
- IEC 62443-2-4:2023 Ed2 stability 2027.
- IEC 62443-3-2:2020 stability 2027.
- IEC 62443-3-3:2013 stability 2027.
- IEC 62443-4-1:2018 stability 2027.
- IEC 62443-4-2:2019 stability 2027.

## 9. Remaining application gates

Not blockers for current generic scripts:
- exact ISA-95 / IEC 62264 clauses and full object models;
- exact OPC UA core-part/IEC 62541 implementation requirements;
- specific Companion Specification selection for a real machine/product;
- record-retention requirements by regulated sector;
- exact IEC 62443 clauses/SL calculations;
- exact remote-access rules by site/sector;
- exact legal cybersecurity duties by jurisdiction;
- site-specific network topology/firewall/DMZ design;
- cloud/AI vendor architecture;
- real data-retention/backup RTO/RPO requirements.

These require dedicated applicability/source locks if added to final narration.
