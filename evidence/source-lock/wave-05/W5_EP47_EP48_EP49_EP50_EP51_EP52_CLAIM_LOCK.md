# Wave 05 Claim Lock — EP47 / EP48 / EP49 / EP50 / EP51 / EP52

status: CLAIM-LEVEL EVIDENCE LOCK COMPLETE FOR CURRENT GENERIC SCRIPT SCOPE
checked: 2026-09-19
shared_register: ../SOURCE_LOCK_WAVE_05_ATLAS_DIGITAL_THREAD_OT_SECURITY_REGISTER.md

## Status vocabulary

- VERIFIED OPEN SOURCE — directly supported by public authoritative source.
- VERIFIED PUBLIC SCOPE — standards/body public scope/status supports premise; protected detail not used.
- VERIFIED + V6 SYNTHESIS — source supports premise, episode framing/tool remains ours.
- DEPENDENCY — source burden already owned by an earlier wave.
- STANDARD CLAUSE GATE — exact normative detail requires controlled standard text/applicability.
- LEGAL/JURISDICTION GATE — exact legal obligation requires jurisdiction/sector source.
- V6 LOCKED AS SYNTHESIS — internal framework.

# EP47 — What PLM, ERP, MES, QMS, SCADA and Historians Actually Do

## EP47-C01
Claim: manufacturing information architecture should begin with information objects/decisions and authority, not software-brand feature lists.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W5-S01/S04/S07.

## EP47-C02
Claim: ISA-95 provides a useful enterprise/manufacturing-control integration reference but does not mandate one PLM/ERP/MES/QMS/SCADA software stack.
Lock: VERIFIED PUBLIC SCOPE.
Source: W5-S01/S02.

## EP47-C03
Claim: PLM, ERP, MES/MOM, QMS, SCADA/HMI and historian roles are useful practitioner categories, but authoritative ownership of each object/attribute must be defined by the implementation.
Lock: V6 LOCKED AS SYNTHESIS, source-informed by W5-S01.
Guard: do not claim ISA-95 normatively assigns these exact vendor-category roles.

## EP47-C04
Claim: duplicated definitions/recipes/status across systems require explicit ownership, revision/effectivity and conflict rules.
Lock: DEPENDENCY — Wave 01 + V6.

## EP47-C05
Claim: lightweight systems are acceptable in DEV if identity/history remain reconstructable; maturity of software tooling is not the maturity definition.
Lock: V6 LOCKED AS SYNTHESIS.

### EP47 gate
Generic script blockers: 0.

# EP48 — Product Genealogy, Recipes, Parameters and Measurements

## EP48-C01
Claim: genealogy is a linked history, not merely a serial number.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W5-S06 + Wave 01/02.

## EP48-C02
Claim: reconstructable history can include product configuration, material/component lineage, process/operation, equipment, recipe/software, critical parameters, measurements, deviations/rework and disposition.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W5-S04/S06.

## EP48-C03
Claim: current master data alone may not reconstruct historical production truth after revisions/effectivity/process changes.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W5-S06 + Wave 01.

## EP48-C04
Claim: persistent/durable identity improves lifecycle traceability across systems.
Lock: VERIFIED OPEN SOURCE.
Sources: W5-S04/S05.

## EP48-C05
Claim: source tag/database identifiers should not automatically be treated as permanent enterprise semantic identity.
Lock: V6 SYNTHESIS supported by W5-S05 durable-ID need.

## EP48-C06
Claim: rework/deviation adds history rather than overwrites it.
Lock: DEPENDENCY — Wave 01/02.

## EP48-C07
Claim: timestamps are useful only when event ordering/time synchronization are adequate for the decision.
Lock: V6 LOCKED AS SYNTHESIS.
No universal synchronization tolerance asserted.

### EP48 gate
Generic script blockers: 0.
Regulated retention obligations: application gated.

# EP49 — Standards, Claims and Evidence as a Manufacturing Knowledge Graph

## EP49-C01
Claim: a document/PDF alone does not preserve the claim, applicability, configuration and evidence relationship needed for future engineering decisions.
Lock: V6 LOCKED AS SYNTHESIS, supported by provenance/digital-thread sources.

## EP49-C02
Claim: consequential engineering claims should preserve source, exact support where needed, applicability/configuration and evidence maturity.
Lock: DEPENDENCY — canonical Source Verification/Packaging Contract + Wave 01.

## EP49-C03
Claim: evidence may support multiple claims only within its demonstrated applicability envelope.
Lock: V6 GLOBAL INVARIANT.

## EP49-C04
Claim: change should trigger dependency-based evidence review rather than blanket deletion or blind reuse.
Lock: DEPENDENCY — Wave 01.

## EP49-C05
Claim: unresolved uncertainty/contradiction and source-vs-synthesis ownership should be first-class knowledge objects.
Lock: V6 LOCKED AS SYNTHESIS.

## EP49-C06
Claim: AI-generated synthesis must remain distinguishable from externally verified fact.
Lock: V6 GLOBAL INVARIANT.

### EP49 gate
Exact normative standard claims continue to require their individual source locks.

# EP50 — The Manufacturing Atlas: Turning Knowledge into Decisions

## EP50-C01
Claim: engineering decisions require context and alternatives, not only fact retrieval.
Lock: V6 LOCKED AS SYNTHESIS.

## EP50-C02
Claim: the Manufacturing Atlas is an internal decision-support synthesis and is not an external industry standard.
Lock: V6 OWNERSHIP RULE.

## EP50-C03
Claim: decision records should preserve context, assumptions, alternatives, evidence, rationale, effectivity and later outcome/learning.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Support: W5-S04/S06 + prior waves.

## EP50-C04
Claim: one weighted score must not override non-compensable safety/regulatory/evidence hard stops.
Lock: V6 GLOBAL HARD-STOP RULE.

## EP50-C05
Claim: AI can assist retrieval/synthesis only if sources, scope, uncertainty and human decision authority remain visible.
Lock: V6 SYNTHESIS + provenance premises.

## EP50-C06
Claim: Atlas should link authoritative systems rather than silently become a competing PLM/MES/QMS source of truth.
Lock: V6 SYNTHESIS, source-informed by W5-S01.

### EP50 gate
Generic script blockers: 0.

# EP51 — OPC UA, ISA-95 and Semantic Integration Without the Buzzwords

## EP51-C01
Claim: connectivity, syntax and semantics are distinct integration problems.
Lock: VERIFIED + V6 SYNTHESIS.
Source: W5-S03.

## EP51-C02
Claim: ISA-95 is a useful scoped reference for enterprise/manufacturing-control hierarchy/information boundaries.
Lock: VERIFIED PUBLIC SCOPE.
Source: W5-S01/S02.

## EP51-C03
Claim: OPC UA provides discovery/transport/information access/security plus object-based information modelling, while Companion Specifications add domain models.
Lock: VERIFIED OPEN SOURCE.
Source: W5-S03.

## EP51-C04
Claim: OPC UA does not automatically solve system-of-record ownership, genealogy, business identity or semantic governance.
Lock: VERIFIED + V6 SYNTHESIS.
Source: W5-S03 + W5-S04/S05.

## EP51-C05
Claim: applicable OPC UA Companion Specifications should be evaluated before inventing proprietary domain models.
Lock: VERIFIED ENGINEERING DIRECTION.
Source: W5-S03.

## EP51-C06
Claim: durable identifiers and semantic mapping require version/effectivity governance.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W5-S05 + Wave 01.

## EP51-C07
Claim: ISA-95 levels should not be presented as a generic cybersecurity segmentation architecture.
Lock: SCRIPT GUARDRAIL.
Cyber segmentation ownership: EP52 / IEC 62443.

### EP51 gate
No exact IEC 62541/ISA-95 clause detail required for current script.

# EP52 — Manufacturing Data Engineers Can Actually Use

## EP52-C01
Claim: decision-grade manufacturing data needs identity/context such as product/configuration, unit/lot, operation, equipment, recipe/software, units/time and quality state appropriate to the decision.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W5-S04/S05/S06 + Wave 02.

## EP52-C02
Claim: more connected tags/data do not automatically create more engineering information.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W5-S03/W5-S04.

## EP52-C03
Claim: OT security must account for performance, reliability and safety consequences.
Lock: VERIFIED OPEN SOURCE.
Source: W5-S08.

## EP52-C04
Claim: read-only analytics and operational write-back are different authority/risk classes.
Lock: VERIFIED PREMISE + V6 SYNTHESIS.
Sources: W5-S08/W5-S11.

## EP52-C05
Claim: IEC 62443 distributes cybersecurity responsibilities across asset owner, service provider, system design/security requirements and product/component supplier roles.
Lock: VERIFIED PUBLIC SCOPE.
Sources: W5-S09–S14.

## EP52-C06
Claim: zones/conduits are risk-design concepts, not one mandatory topology.
Lock: VERIFIED + SCRIPT GUARDRAIL.
Source: W5-S11.

## EP52-C07
Claim: generic application RBAC alone is insufficient to address the OT security problem.
Lock: VERIFIED + V6 SYNTHESIS.
Sources: W5-S08/W5-S11/W5-S12.

## EP52-C08
Claim: cyber/configuration recovery is incomplete until trustworthy configuration, WIP/genealogy, quality and release evidence are restored where affected.
Lock: VERIFIED PREMISE + V6 GLOBAL INVARIANT.
Sources: W5-S08 + Waves 01/02.

## EP52-C09
Claim: AI/derived features/models require input/model/version/provenance lineage appropriate to consequence.
Lock: V6 GLOBAL INVARIANT supported by W5-S04/S06.

### EP52 gate
No exact security level, zone architecture, remote-access control or legal requirement is asserted.
IEC 62443-2-1 status must be rechecked at final publication lock because stability date is 2026.

# Decision

WAVE 05 CLAIM LOCK: PASS FOR INTERNAL TECHNICAL REVIEW.

No generic episode requires protected standards clauses or site-specific network design to proceed.
