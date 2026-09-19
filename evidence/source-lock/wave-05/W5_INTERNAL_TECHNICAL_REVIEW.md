# Wave 05 Internal Technical Review — EP47 / EP48 / EP49 / EP50 / EP51 / EP52

status: PASS TO SCRIPT OUTLINE WITH CONTROLLED STANDARDS/SECURITY GATES
review_date: 2026-09-19
review_type: internal technical consistency + source-boundary + architecture review
human_independent_review: NOT CLAIMED

inputs:
- SOURCE_LOCK_WAVE_05_ATLAS_DIGITAL_THREAD_OT_SECURITY_REGISTER.md
- W5_EP47_EP48_EP49_EP50_EP51_EP52_CLAIM_LOCK.md
- P2.08 Atlas / Sentinel implementation
- P2.09 IEC 62443 / OT security packs
- EP47–52 Production Blueprints
- Waves 01–04 source-lock packages
- frozen Knowledge Backbone V1 invariants

## 1. Review purpose

Test whether the connected-manufacturing arc can advance to scripts without:
- turning software categories into normative systems-of-record roles;
- treating serial number as complete genealogy;
- treating a PDF repository or vector search as evidence architecture;
- presenting the Manufacturing Atlas as an external standard;
- confusing connectivity with semantics;
- treating OPC UA as a complete business ontology;
- misusing ISA-95 levels as cybersecurity segmentation;
- collapsing IEC 62443 role responsibilities;
- prescribing one OT network topology/security level;
- reducing recovery to restarting machines.

# 2. EP47 — Systems of Record

Result: PASS WITH OWNERSHIP GUARDRAILS.

Strengths:
1. starts from information objects/decisions, not software brands;
2. preserves definition vs transaction vs execution vs quality vs machine-history distinctions;
3. ISA-95 used as enterprise/manufacturing integration reference only.

Guards:
### EP47-G01 — category roles
PLM/ERP/MES/QMS/SCADA/historian role descriptions are practitioner architecture patterns, not universal ISA-95 mandates.

### EP47-G02 — one master of everything
Avoid suggesting every object has one global master system. Authority can differ by object/attribute/state/decision, but ambiguity must be explicit.

### EP47-G03 — replication/caching
Copied data may be valid operational replicas; the risk is competing authority without ownership/effectivity rules.

Decision: PASS TO OUTLINE.

# 3. EP48 — Genealogy

Result: PASS.

Strengths:
- linked-event/history model aligns strongly with final NIST IR 8536;
- durable-ID and digital-thread premises are well supported;
- rework/history invariant stays intact.

Guards:
### EP48-G01 — serial number
A serial is an identity anchor, not full genealogy.

### EP48-G02 — UUID
UUID can improve durable identity but does not establish authenticity, authority or provenance alone.

### EP48-G03 — timestamps
No universal synchronization precision is asserted; precision depends on reconstruction/causality need.

### EP48-G04 — retention
Record-retention duration is sector/jurisdiction/customer specific.

Decision: PASS TO OUTLINE.

# 4. EP49 — Claim/Evidence Knowledge Graph

Result: PASS WITH FRAMEWORK-OWNERSHIP GUARDS.

Strengths:
- clear distinction among source, claim, applicability, evidence and conclusion;
- directly supports frozen source-verification discipline;
- contradictions/uncertainty remain visible.

Guards:
### EP49-G01 — graph technology
Do not imply a graph database is required; "knowledge graph" here describes linked semantic objects/relationships.

### EP49-G02 — standards text
Do not ingest/reproduce protected standards content. Preserve citation metadata/location and controlled licensed access as applicable.

### EP49-G03 — AI
Search/model confidence is not evidence maturity.

Decision: PASS TO OUTLINE.

# 5. EP50 — Manufacturing Atlas

Result: PASS.

Strengths:
- Atlas correctly presented as internal synthesis;
- decision context/alternatives/evidence/outcome are explicit;
- hard stops prevent weighted-score abuse.

Guards:
### EP50-G01 — no autonomous authority
Do not imply Atlas/AI should replace accountable engineering approval.

### EP50-G02 — no duplicate SoR
Atlas should link authoritative systems/objects, not silently become a competing source of product or release truth.

### EP50-G03 — scoring
Decision matrices can assist comparison but cannot average away mandatory safety/regulatory/evidence constraints.

Decision: PASS TO OUTLINE.

# 6. EP51 — OPC UA / ISA-95 / Semantics

Result: PASS WITH TERMINOLOGY GUARDRAILS.

Strengths:
- connectivity/syntax/semantics distinction is strong;
- public OPC Foundation source directly supports infrastructure vs Companion-model layering;
- 2025 ISA-95 Part 1 status is current.

Guards:
### EP51-G01 — ISA-95 levels
Use them as functional/information reference concepts. Do not present them as network zones, Purdue cybersecurity architecture, or mandatory software tiers.

### EP51-G02 — OPC UA identifiers
Do not claim NodeIds are universally temporary or unusable. Claim only that a source identifier should not automatically be assumed to be the organization's durable cross-system semantic identity without governance.

### EP51-G03 — Companion Specs
"Evaluate applicable Companion Specs first" is engineering guidance, not a universal requirement that one must exist/use one.

### EP51-G04 — security
OPC UA security capabilities do not replace OT-security program/system risk architecture.

Decision: PASS TO OUTLINE.

# 7. EP52 — Engineering Data + OT Security

Result: PASS WITH HIGH SECURITY-APPLICABILITY DISCIPLINE.

Strengths:
- starts from decision-grade context rather than data volume;
- responsibility split across IEC 62443 parts is accurate at public-scope level;
- NIST SP 800-82 provides open generic OT-security grounding;
- recovery/evidence invariant is strong.

Guards:
### EP52-G01 — IEC 62443 role split
Do not say each organization maps one-to-one permanently to one part. Roles can coexist; applicability depends on actual responsibilities.

### EP52-G02 — zones/conduits
Do not prescribe count/topology/security level.

### EP52-G03 — remote access
May discuss risk-controlled remote access generically; exact controls/design depend on system/site/standards applicability.

### EP52-G04 — least privilege
Use as security design principle, not as a substitute for full OT risk architecture.

### EP52-G05 — write-back
Read-only vs write-back is a useful authority/risk distinction, but read-only connectivity is not automatically safe.

### EP52-G06 — recovery
Do not claim every cyber event invalidates all manufacturing evidence. Assess which configuration/data/quality dependencies may have been affected.

### EP52-G07 — current-status watch
IEC 62443-2-1:2024 has IEC stability date 2026; must be rechecked immediately before final publication lock.

Decision: PASS TO OUTLINE.

# 8. Cross-episode boundary review

EP47 vs EP51:
EP47 owns software/system responsibility boundaries; EP51 owns semantic integration/protocol/context. PASS.

EP48 vs EP49:
EP48 owns physical/unit production history; EP49 owns engineering claim/evidence knowledge. PASS.

EP49 vs EP50:
EP49 owns knowledge representation/provenance; EP50 owns decision workflow. PASS.

EP50 vs EP52:
EP50 owns decision support; EP52 owns decision-grade dataset/security/recovery. PASS.

EP51 vs EP52:
EP51 may preview security boundary; EP52 owns OT security. PASS.

# 9. Global invariant check

Definition/as-built/evidence distinction: PASS.
Rework adds history: PASS.
Evidence bounded by applicability/configuration: PASS.
Change invalidation is dependency based: PASS.
Cyber/configuration events can invalidate affected evidence: PASS.
Recovery requires trustworthy production/evidence state: PASS.
AI/synthesis ownership visible: PASS.

No backbone change required.

# 10. Script-entry decision

EP47: PASS TO SCRIPT OUTLINE.
EP48: PASS TO SCRIPT OUTLINE.
EP49: PASS TO SCRIPT OUTLINE.
EP50: PASS TO SCRIPT OUTLINE.
EP51: PASS TO SCRIPT OUTLINE.
EP52: PASS TO SCRIPT OUTLINE — publication recheck on IEC 62443-2-1 required.

**WAVE 05 INTERNAL TECHNICAL REVIEW: PASS**
