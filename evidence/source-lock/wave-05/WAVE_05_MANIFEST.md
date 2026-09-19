# Source-Lock Wave 05 — Manufacturing Atlas / Digital Thread / OT Security

status: COMPLETE — PUBLICATION WORKFLOW PASS FOR CURRENT GENERIC SCRIPT SCOPE
opened: 2026-09-19
closed: 2026-09-19
scope_type: shared-source-family wave

## 1. Purpose

Advance EP47–52 and P2.08/P2.09 from production architecture into controlled publication packages while separating:
- information ownership/system-of-record decisions;
- genealogy/provenance;
- claims/evidence knowledge;
- Manufacturing Atlas decision support;
- semantic integration/connectivity;
- OT/IACS cybersecurity and recovery.

Pipeline:
Shared Source Lock → Episode Claim Lock → Internal Technical Review → Script Outline → Full Script Draft → Script Review → Source Notes → Publication Gate.

## 2. Direct episode scope

- EP47 — What PLM, ERP, MES, QMS, SCADA and Historians Actually Do
- EP48 — Product Genealogy, Recipes, Parameters and Measurements
- EP49 — Standards, Claims and Evidence as a Manufacturing Knowledge Graph
- EP50 — The Manufacturing Atlas: Turning Knowledge into Decisions
- EP51 — OPC UA, ISA-95 and Semantic Integration Without the Buzzwords
- EP52 — Manufacturing Data Engineers Can Actually Use

Backbone:
- P2.08 — Manufacturing Atlas / Digital Thread / Minimum Viable Atlas
- P2.09 — OT/ICS Cybersecurity / IEC 62443 / Recovery / Remote Access

## 3. Canonical shared register

evidence/source-lock/SOURCE_LOCK_WAVE_05_ATLAS_DIGITAL_THREAD_OT_SECURITY_REGISTER.md

## 4. Current source status checked 2026-09-19

- ANSI/ISA-95.00.01-2025 is current ISA Part 1.
- NIST Digital Thread project updated 2026-08-12.
- NIST IR 8536 final published 2026-09-09; prior drafts obsolete.
- NIST SP 800-82 Rev.3 remains current final OT-security guide.
- IEC 62443-2-1:2024 Ed2 asset-owner program requirements; stability date 2026.
- IEC 62443-2-4:2023 Ed2 service-provider requirements.
- IEC 62443-3-2:2020 system risk / zones-conduits.
- IEC 62443-3-3:2013 system security requirements/security levels.
- IEC 62443-4-1:2018 secure product-development lifecycle.
- IEC 62443-4-2:2019 component security requirements.

## 5. Hard boundaries

1. software category does not automatically determine information authority;
2. serial number alone is not genealogy;
3. documents are source containers, not claim/evidence context by themselves;
4. Atlas/ATLAS 10 is internal synthesis;
5. ISA-95 is not a mandatory software stack or cyber segmentation scheme;
6. OPC UA endpoint is not semantic architecture;
7. UUID alone is not provenance;
8. PLC tag/NodeId/database key is not automatically durable cross-system identity;
9. NIST SP 800-82 is guidance, not law;
10. IEC 62443 applicability is role/system specific;
11. no universal security level or zones/conduits drawing;
12. read-only analytics and operational write-back are distinct authority/risk classes;
13. cyber/configuration recovery is not complete at machine restart;
14. AI/derived data never silently replaces evidence lineage;
15. exact legal/sector obligations remain jurisdiction/application gated.

## 6. Completion criterion

Wave 05 closes when EP47–52 each have:
- claim lock;
- technical review;
- source-linked outline;
- full script draft;
- script review;
- source notes;
- explicit standards/security/applicability gates;
- wave publication-gate record.
