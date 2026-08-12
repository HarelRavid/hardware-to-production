# P2.08 — Minimum Viable Manufacturing Atlas + Data Hub Validation Map

Status: NEAR PODCAST READY — architecture validated against Sentinel Node implementation example
Provenance: [GNR] synthesis supported by the repository Data Hub architecture; standards/source claims require episode-level verification.

## Purpose

Translate the Manufacturing Data Hub from a large enterprise architecture into a staged implementation that a small hardware team can actually use.

The goal is NOT:
- to prescribe PLM + ERP + MES + QMS + historian + data lake on day one;
- to reproduce every ISA-95 object;
- to force a startup into enterprise software before the process deserves it.

The goal IS:

> Preserve the identities, relationships, evidence and history that become expensive or impossible to reconstruct later.

Canonical principle:

**Start with the information obligations, not the software categories.**

---

# 1. Maturity language

Use three distinct maturity states:

1. **Architecture drafted** — concepts and relationships are defined.
2. **Architecture validated against implementation example** — a representative product genealogy can be reconstructed and required queries can be answered by the model.
3. **Implementation validated** — an actual deployed system has demonstrated integrity, performance, permissions, integrations, backup/recovery and operating workflows.

P2.08 reaches State 2 for the Sentinel Node example. It does not claim State 3.

---

# 2. What must survive from DEV to SVP

Even when the tools change, preserve these core identities:

1. Product / part identity
2. Revision / configuration identity
3. Requirement / CTQ identity
4. Material / component lot or serial identity where risk requires it
5. Process / operation identity
6. Equipment / fixture / recipe identity where relevant
7. Measurement / test result identity
8. Nonconformance / deviation / rework identity
9. Change / effectivity identity
10. Evidence / approval identity
11. Personnel/authorization identity where required
12. Time / sequence / genealogy

If these are lost, later software cannot magically recreate the truth.

---

# 3. Minimum Viable Manufacturing Atlas by stage

## 3.1 DEV — Learning System

Primary objective: learn what the product and process actually are.

Minimum required information:
- unique prototype/unit identifier;
- current drawing/BOM/configuration identifier;
- build date;
- critical component identity where failure learning depends on it;
- build/process notes;
- test results linked to the unit;
- failures and rework history;
- engineering change history;
- explicit distinction between planned definition and what was actually built.

Acceptable implementation:
- controlled Git/document repository;
- disciplined spreadsheet/database;
- structured test files;
- simple serial/lot labels;
- issue/NCR log.

Not yet mandatory merely because it exists in enterprise manufacturing:
- full MES;
- full ERP routing execution;
- historian infrastructure;
- complex automated genealogy;
- enterprise ontology platform.

DEV exit question:

> Can we reconstruct why Prototype 17 differs from Prototype 12 and which evidence belongs to each configuration?

---

## 3.2 LVP — Controlled Execution System

Primary objective: repeatedly build tens/hundreds of units without losing configuration, genealogy or quality learning.

Add to DEV minimum:
- released product/BOM revision;
- work-order/batch identity;
- operation/routing identity;
- incoming material/lot status for critical items;
- operator/workstation/fixture association where needed;
- controlled process parameters/recipes;
- structured CTQ measurements;
- pass/fail test execution linked to serial;
- NCR/deviation/rework workflow;
- disposition and release status;
- supplier lot genealogy;
- change effectivity/cut-in;
- WIP status;
- calibration/tool status where measurement/process evidence depends on it.

Tooling approach:
- lightweight ERP/MRP may become valuable;
- QMS workflows may become formalized;
- simple MES-like execution can be custom/lightweight;
- barcode/QR capture becomes highly valuable;
- avoid duplicate manual transcription between systems where possible.

LVP exit question:

> For any shipped serial, can we reconstruct what it was supposed to be, what it actually was, what happened during production, what failed, what changed, and why it was accepted?

---

## 3.3 SVP — Scalable Manufacturing Information System

Primary objective: sustain volume, multiple products/lines/suppliers and faster decision cycles without losing control.

Add/strengthen:
- formal system-of-record boundaries;
- scalable resource/equipment hierarchy;
- production scheduling/execution integration;
- automated genealogy/event capture;
- supplier/sub-tier integration where justified;
- historian/time-series integration where useful;
- machine/OPC UA or other semantic interfaces where justified;
- role/permission separation;
- auditability;
- data-quality controls;
- master-data governance;
- analytics interfaces;
- decision-engine interfaces;
- evidence/applicability graph;
- backup/recovery/retention;
- OT/ICS cybersecurity architecture.

SVP question:

> Can the organization scale throughput, products, sites and automation while preserving trustworthy identity, context, evidence and decision history?

---

# 4. System categories are implementation choices, not the ontology

Typical systems may include:
- PLM/PDM;
- ERP/MRP;
- MES/MOM;
- QMS;
- SCADA/historian;
- CMMS/EAM;
- supplier portals;
- data platform/warehouse/lakehouse;
- knowledge/evidence graph.

But the Atlas should not define truth by vendor category.

Example:

A serial's as-built configuration may be assembled from authoritative records across PLM definition, MES execution, ERP material genealogy and QMS exception history.

The canonical object is the manufacturing truth; the software is the custodian of parts of that truth.

---

# 5. Data Hub validation map

The existing `domains/manufacturing-data-hub` architecture is tested against the Sentinel Node implementation example.

## 5.1 MANUFACTURING_ONTOLOGY_CORE.md

Validation status: **VALIDATED AGAINST EXAMPLE**

Sentinel proof:
- Product Definition → Product Instance SN-0284;
- Material Definition → Lot/serialized component instance;
- Process Definition → Operation Execution;
- Equipment Asset → execution context;
- Measurement/Test → Evidence/Decision.

Remaining gap before implementation validation:
- production schema constraints;
- lifecycle/API behavior;
- scale/performance testing.

## 5.2 ISA95_RESOURCE_HIERARCHY.md

Validation status: **PARTIALLY VALIDATED AGAINST EXAMPLE**

Sentinel proof:
- Site/Area/Work Center/Work Unit/Equipment context can be attached to operation execution.

Remaining gap:
- multi-site/multi-line example;
- resource scheduling/capability semantics;
- exact current ISA-95 terminology/source verification.

## 5.3 MANUFACTURING_PROCESS_ATLAS.md

Validation status: **VALIDATED AGAINST EXAMPLE**

Sentinel proof:
- process definition is separated from operation execution;
- CTQs, equipment, parameters and output evidence are linked to execution.

Remaining gap:
- broader process-family taxonomy;
- process capability library population.

## 5.4 PARAMETER_MEASUREMENT_MODEL.md

Validation status: **VALIDATED AGAINST EXAMPLE**

Sentinel proof:
- seating depth measurement 4.76 mm FAIL and 5.02 mm PASS remain distinct observations;
- measurement context supports quality decision rather than overwriting history.

Remaining gap:
- uncertainty/calibration data implementation;
- high-rate time-series treatment.

## 5.5 SYSTEM_OF_RECORD_BOUNDARIES.md

Validation status: **VALIDATED CONCEPTUALLY**

Sentinel proof:
- definition, material transaction, execution and exception records can have different authoritative custodians while joining through stable identities.

Remaining gap:
- actual multi-system integration demonstration;
- conflict-resolution rules when systems disagree.

## 5.6 OPC_UA_SEMANTIC_INTEGRATION.md

Validation status: **ARCHITECTURE DRAFTED — NOT IMPLEMENTATION-VALIDATED**

Sentinel proof:
- model identifies why machine tags should map to semantic process/equipment/parameter identities.

Remaining gap:
- actual OPC UA server/client information model;
- Companion Specification selection;
- namespace/version lifecycle;
- event ingestion demonstration.

## 5.7 DATA_OWNERSHIP_AUTHORITY.md

Validation status: **VALIDATED CONCEPTUALLY**

Sentinel proof:
- product definition, execution result, NCR disposition and evidence approval require different authorities.

Remaining gap:
- real organizational RACI/permissions;
- conflict/escalation workflow.

## 5.8 CLAIMS_EVIDENCE_STANDARDS_GRAPH.md

Validation status: **VALIDATED AGAINST EXAMPLE**

Sentinel proof:
- Claim → Evidence → Applicability Statement is instantiated;
- evidence is limited to the demonstrated configuration/process envelope.

Remaining gap:
- primary-standard citation population;
- automated invalidation/review logic.

## 5.9 DECISION_ENGINE_INTERFACES.md

Validation status: **PARTIALLY VALIDATED AGAINST EXAMPLE**

Sentinel proof:
- release/rework/change decisions can consume configuration, genealogy and evidence objects.

Remaining gap:
- executable decision engine;
- explainability/approval behavior;
- human-in-the-loop boundaries.

## 5.10 ANALYTICS_AI_INTERFACES.md

Validation status: **ARCHITECTURE DRAFTED — NOT IMPLEMENTATION-VALIDATED**

Sentinel proof:
- reconstructed genealogy creates contextualized data suitable for analytics/AI.

Remaining gap:
- actual feature/data contracts;
- training/evaluation lineage;
- access control and model feedback behavior.

## 5.11 SECURITY_PERMISSIONS_AUDITABILITY_QUALITY_GATE.md

Validation status: **PARTIALLY VALIDATED CONCEPTUALLY**

Sentinel proof:
- immutable history, authority separation and audit events are required by the SN-0284 reconstruction.

Remaining gap:
- actual RBAC/ABAC implementation;
- audit-log integrity;
- backup/recovery;
- IEC 62443/OT security mapping — deferred to P2.09.

## 5.12 DATA_HUB_RECONCILIATION_MAP.md

Validation status: **VALIDATED AGAINST EXAMPLE**

Sentinel proof:
- the Data Hub can remain a manufacturing operational/evidence layer without duplicating the wider Knowledge OS.

Remaining gap:
- implementation boundary tests against future repositories/services.

---

# 6. What the startup should NOT do

## Anti-pattern 1 — Buy enterprise software before defining identities

Result:
- expensive software containing inconsistent part names, uncontrolled revisions and weak genealogy.

## Anti-pattern 2 — Spreadsheet shame

A controlled spreadsheet with stable IDs, ownership, validation and backup can be better than a poorly implemented MES.

The issue is not whether Excel exists.
The issue is whether manufacturing truth is controlled and reconstructable.

## Anti-pattern 3 — Store only final PASS

This destroys learning and hides process instability.

SN-0284 must retain:
- initial 4.76 mm FAIL;
- NCR;
- rework action;
- changed component genealogy;
- 5.02 mm PASS;
- final test/release evidence.

## Anti-pattern 4 — Let every system invent identifiers

A part called `CONN-A`, `J4`, `SupplierBlue-Conn`, `Item-4481` and `PLC_Tag_32` cannot be safely joined without controlled identity/alias mapping.

## Anti-pattern 5 — Automate bad semantics

Automatic capture of a million values does not create a digital thread if nobody knows which product, operation, recipe, equipment state and requirement they belong to.

---

# 7. Minimum Viable Atlas — 12 objects

For a small hardware company, begin with twelve canonical object classes:

1. Product/Part Definition
2. Product/Part Revision
3. Product Instance / Lot
4. Requirement / CTQ
5. Material/Component Instance or Lot
6. Process/Operation Definition
7. Operation Execution
8. Resource/Equipment/Tool
9. Measurement/Test Result
10. Exception — NCR/Deviation/Rework
11. Change/Effectivity
12. Claim/Evidence/Approval

This is a conceptual minimum, not a prescribed database schema.

Everything else can grow around these objects as scale and risk justify it.

---

# 8. Minimum Viable Atlas — 10 relationships

At minimum, preserve relationships equivalent to:

1. instance **conforms-to / was-built-against** revision;
2. revision **contains/requires** component definition;
3. installed component instance/lot **is-used-in** product instance;
4. operation execution **executes** process definition;
5. operation execution **acts-on** product instance;
6. execution **uses** equipment/tool/recipe configuration;
7. measurement **observes** CTQ on an instance/execution;
8. exception/rework **affects** product/execution/component;
9. change **changes/effectively-applies-to** definition/process population;
10. decision/claim **is-supported-by** evidence under an applicability envelope.

---

# 9. Migration rule — grow without rebuilding truth

A good DEV data structure should migrate into LVP/SVP rather than be discarded.

Example path:

DEV:
Git + controlled spreadsheet + serial folders

→ LVP:
ERP/MRP + structured QMS + lightweight execution/genealogy database

→ SVP:
PLM/ERP/MES/QMS/historian integrations + governed data/evidence layer

Stable IDs and relationships survive the migration.

Bad migration:
- new system creates new identifiers;
- historical serial genealogy is not migrated;
- old revisions lose effectivity;
- test data become detached files;
- NCR/rework history becomes PDF archive only.

---

# 10. Listener tool — ATLAS 10

Before buying or building manufacturing software, ask:

1. **Identity** — what objects must have stable IDs?
2. **Definition** — what was the approved configuration?
3. **Execution** — what actually happened on the floor?
4. **Genealogy** — which materials/components entered which units?
5. **Context** — which process/equipment/recipe/operator conditions matter?
6. **Quality** — where are raw measurements, tests and exceptions?
7. **Change** — can we determine effectivity and affected populations?
8. **Evidence** — why was a product/process/supplier released?
9. **Authority** — which system/person is allowed to establish each truth?
10. **Reconstruction** — can we answer these questions years later without tribal memory?

---

# 11. Canonical podcast messages

> You do not need an MES to start manufacturing. You need manufacturing truth you can reconstruct.

> Software maturity should follow process and information maturity — not replace them.

> The most expensive data to collect later is the data you failed to identify during the build.

> Digital thread is not “all data in one database.” It is trustworthy identity, context and relationships across the lifecycle.

> A spreadsheet is not automatically immature; uncontrolled identity and unreconstructable history are immature.

---

# 12. P2.08 completion gate

P2.08 now contains:
- Sentinel Node serial genealogy worked example;
- Claim→Evidence→Applicability example;
- relationship graph;
- mock relational model;
- executable-style genealogy/effectivity query tests;
- Data Hub validation map;
- DEV/LVP/SVP Minimum Viable Atlas;
- 12-object conceptual minimum;
- 10-relationship conceptual minimum;
- ATLAS 10 listener tool;
- explicit architecture maturity language.

## Remaining before Podcast Ready

1. Verify primary sources/current editions for ISA-95/IEC 62264 and any OPC UA claims used in episodes.
2. Technical review of system-of-record and semantic integration language.
3. Add episode-level source notes and claim provenance.
4. Do not claim implementation validation until a deployed implementation exists.

Recommended P2.08 status: **NEAR PODCAST READY**.

Next package: **P2.09 — OT/ICS Cybersecurity / IEC 62443 applicability and manufacturing-system security architecture.**
