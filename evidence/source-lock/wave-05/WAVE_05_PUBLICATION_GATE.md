# Source-Lock Wave 05 — Publication Gate

status: PASS — PUBLICATION WORKFLOW COMPLETE FOR CURRENT GENERIC SCRIPT SCOPE
closed: 2026-09-19
scope: EP47 / EP48 / EP49 / EP50 / EP51 / EP52
shared_backbone: P2.08 Manufacturing Atlas / Digital Thread + P2.09 OT/ICS Cybersecurity

## 1. Purpose

Verify completion of the Wave 05 publication workflow:

Shared Source Lock → Claim Lock → Internal Technical Review → Script Outline → Full Script Draft → Script Review → Source Notes → Publication Gate.

## 2. Package completeness

EP47 — Systems of Record:
- source lock COMPLETE
- claim lock COMPLETE
- technical review PASS
- outline COMPLETE
- full draft COMPLETE
- script review PASS
- source notes COMPLETE
- current-script P0 blockers: 0

EP48 — Product Genealogy:
- all publication-package gates COMPLETE/PASS
- current NIST IR 8536 final used
- current-script P0 blockers: 0

EP49 — Claim/Evidence Knowledge Graph:
- all publication-package gates COMPLETE/PASS
- current-script P0 blockers: 0

EP50 — Manufacturing Atlas:
- all publication-package gates COMPLETE/PASS
- Atlas explicitly internal synthesis
- current-script P0 blockers: 0

EP51 — OPC UA / ISA-95 / Semantic Integration:
- all publication-package gates COMPLETE/PASS
- current ISA-95 Part 1 2025 status locked
- current-script P0 blockers: 0

EP52 — Manufacturing Data Engineers Can Actually Use:
- all publication-package gates COMPLETE/PASS
- OT-security role/status map locked
- current-script P0 blockers: 0
- final publication recheck required for IEC 62443-2-1 current status due IEC stability date 2026

## 3. Current source findings

Checked 2026-09-19:

- ANSI/ISA-95.00.01-2025 (IEC 62264-1 Mod) is current ISA Part 1 and replaces the 2010 Part 1.
- OPC UA public architecture continues to separate core infrastructure from layered information models/Companion Specifications.
- NIST Digital Thread for Manufacturing updated 2026-08-12.
- NIST IR 8536 final published 2026-09-09; 2024/2025 drafts are obsolete.
- NIST SP 800-82 Rev.3 remains current final OT-security guidance.
- IEC 62443-2-1:2024 Ed2 — asset-owner security program; stability date 2026.
- IEC 62443-2-4:2023 Ed2 — service-provider security program.
- IEC 62443-3-2:2020 — system risk / zones-conduits.
- IEC 62443-3-3:2013 — system security requirements/security levels.
- IEC 62443-4-1:2018 — product secure-development lifecycle.
- IEC 62443-4-2:2019 — component security requirements.

## 4. Workflow findings

### W5-P01 — software category is not manufacturing truth
Information ownership must be defined by object/attribute/decision; PLM/ERP/MES/QMS/SCADA/historian are implementation categories, not automatic universal masters.

### W5-P02 — traceability is relational and historical
Serial identity alone is not genealogy. Current NIST IR 8536 strongly supports linked, temporally ordered provenance/traceability.

### W5-P03 — knowledge needs claim/evidence/applicability context
Document retrieval and AI synthesis do not replace source authority, configuration scope and evidence maturity.

### W5-P04 — Atlas is decision synthesis, not a standard
ATLAS 10/Decision Cards are internal frameworks that reuse externally verified technical premises.

### W5-P05 — connectivity is not semantics
OPC UA can carry structured information models; semantic identity/ownership/effectivity governance remains necessary.

### W5-P06 — ISA-95 is not cyber segmentation
ISA-95 remains an enterprise/manufacturing-control integration reference; OT cybersecurity architecture is owned by NIST/IEC 62443 context.

### W5-P07 — IEC 62443 is role-distributed
Asset owner, service provider, system risk/security and product/component responsibilities are distinct and can coexist in one organization.

### W5-P08 — OT recovery is production recovery
Restoring services is insufficient when configuration, WIP/genealogy, quality or release evidence may have been affected.

## 5. Cross-episode ownership

EP47: information authority/system-of-record map.
EP48: physical/unit genealogy and provenance.
EP49: claims/evidence/standards knowledge relationships.
EP50: context-aware decision workflow / Atlas.
EP51: semantic integration / ISA-95 / OPC UA.
EP52: decision-grade manufacturing datasets + OT security/recovery.

Result:
PASS — no merge, reorder or backbone redesign required.

## 6. Remaining application gates

Not blockers for current generic scripts:
- exact ISA-95/IEC 62264 clauses/object models;
- exact OPC UA/IEC 62541 implementation requirements;
- site-specific Companion Specification selection;
- regulated retention requirements;
- exact IEC 62443 clauses/security-level calculations;
- site-specific zone/conduit/network architecture;
- remote-access controls and legal cybersecurity duties by jurisdiction;
- cloud/AI provider architecture;
- real RTO/RPO and backup requirements.

## 7. Gate decision

Knowledge Backbone change required: NO.
Episode architecture change required: NO.
Source-lock workflow change required: NO.
Current generic-script P0 blockers: 0.
Final status recheck required: IEC 62443-2-1:2024 before EP52 final publication lock.

**SOURCE-LOCK WAVE 05: PASS**

Next source family:
**Wave 06 — Manufacturing Process Families**.
