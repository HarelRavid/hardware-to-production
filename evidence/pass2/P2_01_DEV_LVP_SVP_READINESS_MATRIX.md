# Pass 2.01 — DEV / LVP / SVP Readiness Matrix

status: ACTIVE — WORKED DECISION TOOL + LISTENER CHECKLIST
created_on: 2026-08-11
maps_to: Opening Arc A1–A8; Episodes 1–5, 26–31, 60
companion: P2_01_HARDWARE_READINESS_DEFINITIONS.md; P2_01_WORKED_EXAMPLE_SENTINEL_NODE.md; P2_01_LISTENER_READINESS_CHECKLIST.md

## Purpose
Turn DEV/LVP/SVP from an editorial lens into a practical decision tool. The matrix does not prescribe universal phase gates. It shows how the burden of evidence changes as a team moves from learning whether the product can work, to proving it can be built repeatedly, to proving the production system can sustain business-required output.

## Governance
DEV, LVP and SVP are podcast shorthand, not standard lifecycle names.

The evidence logic is informed by NASA Production Readiness Review and DoD Manufacturing Readiness Level concepts:
- NASA PRR evaluates readiness to efficiently produce the required number of systems and expects production documentation, controls, enabling resources, risks and personnel to be ready.
- DoD MRL progression distinguishes production-representative/pilot evidence, low-rate production capability and full-rate production capability.

Applicability boundary: aerospace/defense review structures are evidence sources for readiness dimensions, not mandatory startup bureaucracy.

## Three-stage listener lens

### DEV — Development / Learning System
Primary question: **Can the product concept and architecture satisfy the intended need, and what uncertainty must we retire next?**

Optimized for learning speed, technical-risk retirement, architecture exploration, requirements discovery/refinement and fast iteration.

Acceptable when explicit and risk-bounded:
- hand assembly;
- temporary fixtures;
- dev boards and lab equipment;
- engineering-only setup/calibration;
- manual data collection;
- prototype materials/processes;
- limited traceability;
- expensive low-volume processes;
- rework as a learning mechanism.

Dangerous if mistaken for production evidence:
- expert engineer repeatedly rescuing builds;
- uncontrolled BOM substitutions;
- prototype process materially different from target process;
- undocumented tuning;
- pass/fail based on subjective expert judgment;
- test configuration not recorded;
- shortcuts whose expiration condition is unknown.

### LVP — Low-Volume Production / Learning Production System
Primary question: **Can ordinary production resources repeatedly build conforming units using a controlled, increasingly representative process?**

Expected evidence grows materially:
- controlled product configuration/BOM/drawings;
- defined production route/routing;
- production-representative tooling/fixtures where critical;
- trained operators and defined work instructions;
- CTQ-linked inspection/test controls;
- measurement-system adequacy appropriate to decisions;
- lot/unit genealogy where required;
- NCR/deviation/change handling;
- yield/rework/defect data;
- supplier/material status;
- rate/cycle/bottleneck evidence;
- maintenance/recovery assumptions for production equipment.

Still potentially appropriate:
- manual or semi-automated assembly;
- bridge manufacturing;
- selective engineering support;
- temporary tooling when its limitations are understood;
- higher inspection intensity while process knowledge matures.

### SVP — Scaled / Serial Volume Production
Primary question: **Can the production system sustain the business-required rate, quality, cost and change discipline over time?**

Expected evidence:
- sustained capacity/rate evidence under representative mix and downtime;
- stable/capable processes for critical characteristics at context-appropriate levels;
- validated inspection/test systems;
- controlled suppliers/sub-tiers/special processes where applicable;
- actual cost/yield/scrap/rework behavior feeding economics;
- maintenance/spares/recovery system;
- robust genealogy/configuration/change cut-in;
- clear reaction plans and escalation ownership;
- production data and field/service feedback connected to improvement;
- automation justified and qualified where used.

## Readiness matrix by dimension

| Dimension | DEV | LVP | SVP | Sentinel Node illustration |
|---|---|---|---|---|
| Product requirements | learning/refining critical requirements | controlled requirements sufficient for production validation | controlled requirements with disciplined change/field feedback | sensing concept → defined accuracy/sealing/connector CTQs → field-return feedback tied to requirements |
| Configuration | enough identity to know what was tested | reproducible controlled build configuration | full effectivity/change cut-in/genealogy discipline | dev-board/config notes → PCB/BOM/FW revision-controlled builds → returned serial linked to exact HW/FW/gasket/supplier state |
| Materials/components | prototype substitutes may be acceptable if explicit | increasingly production-intent and qualified | controlled approved sources with resilience/change rules | dev-board sensor → intended sensor/PCB/component set → alternate sensor requires controlled qualification/change |
| Manufacturing process | chosen to answer engineering questions | representative route proven through repeated builds | controlled route sustaining rate/quality/cost | CNC enclosure → production-intent molded enclosure validation → controlled molding/assembly route |
| Tooling/fixtures | temporary/rapid tooling acceptable | production-representative for critical operations | production-capable, maintained, controlled, spare/recovery strategy | lab fixture → controlled connector/sealing/calibration fixtures → maintained/spared production fixtures |
| Work instructions | engineer knowledge may dominate | operators can execute defined work with bounded support | scalable standard work/training/change control | designer assembles prototype → operators build from WI → standardized training/change-controlled instructions |
| Measurement/test | lab-grade/engineering test acceptable | production test/inspection adequacy demonstrated | validated, maintained measurement/test system with reaction plans | bench instruments → controlled final/calibration test → sustained test system with maintenance/GR&R-like evidence as relevant |
| Quality controls | defect discovery and learning | PFMEA/control-plan/reaction logic functioning in practice | controls demonstrate sustained effectiveness and capability | sealing/connector failures become PFMEA/control inputs → reaction plan works in LVP → capability/field feedback close loop |
| Yield/rework | informative but often not production representative | FPY/rework/scrap captured by operation/failure mode | sustained yield economics and improvement system | prototype rework accepted → 15% final-test loss traced to connector-pin damage → sustained FPY and cost tracked |
| Suppliers | availability/technical exploration | qualification, first-article/PPAP-type evidence as applicable | ongoing capability, change control, sub-tier/resilience management | prototype sourcing → intended sensor/gasket/PCB suppliers qualified → alternate-source/change discipline |
| Rate/capacity | generally not proven | bottleneck/rate assumptions tested in representative runs | sustained capacity under representative mix/downtime/staffing | assembly looks fast → calibration/test identified as constraint → sustained output validated at required business rate |
| Automation | avoid locking unstable work unless learning requires it | targeted/semi-automation often valuable | automation justified by TCO, qualified, maintainable, change-aware | manual calibration/assembly → selective fixture/semi-auto test → dedicated automation only if economics/process maturity justify |
| Traceability | enough to preserve engineering learning | enough to reconstruct builds, defects and changes | scalable genealogy/effectivity/auditability | prototype notebook/config log → lot/unit build history → serial-level change/field investigation capability |
| Economics | rough architecture/process tradeoffs | cost per good part begins using actual yield/labor/process data | actual TCO/cost/capacity behavior drives decisions | CNC/AM prototype economics → bridge-process cost/yield → serial tooling/TCO based on real production behavior |
| Service/lifecycle | identify foreseeable service constraints | serviceability/spares/diagnostics increasingly validated | field-return/service data closes loop to product/process controls | design for access/diagnostics → repair path/spares defined → returns linked to configuration/process evidence |

## Evidence-transfer rule
Evidence transfers forward only when the changed configuration/process/environment does not invalidate the question previously answered.

At every major change ask:
1. What requirement was the old evidence supporting?
2. What physical/process assumptions made that evidence valid?
3. Which assumptions changed?
4. Does the change require analysis, regression, partial requalification or full re-verification?

Sentinel examples:
- changing sensor mounting can invalidate vibration-response evidence;
- changing CNC enclosure to injection molding can invalidate sealing/warpage/tolerance evidence;
- changing sensor supplier can affect firmware calibration, measurement behavior and qualification evidence;
- changing assembly fixture can alter connector-damage rates and therefore process-control evidence.

## Podcast listener tool
The compact listener-facing version now lives in `P2_01_LISTENER_READINESS_CHECKLIST.md`.

It uses twelve evidence dimensions and a 0–3 maturity indication:
- `0 — unknown/not controlled`
- `1 — engineering/DEV evidence`
- `2 — repeatable LVP evidence`
- `3 — sustained SVP evidence`

Important guardrail: the checklist is not a simple average score. One weak critical dimension can block a transition.

## “Where are we lying to ourselves?”
Ask five questions:
1. **What are we claiming is ready?**
2. **What evidence proves that specific claim?**
3. **Was the evidence generated with a representative configuration/process/environment?**
4. **What expert intervention or hidden workaround was required?**
5. **What changed since the evidence was generated that could invalidate it?**

## Claims
### P2-C-MAT-001 — DEV/LVP/SVP should describe the maturity of the evidence burden, not simply unit-count bands
status: STRONG SYNTHESIS
basis: NASA PRR + DoD MRL progression + A0/A1/A5 evidence.

### P2-C-MAT-002 — Manual production can be legitimate in LVP and even some serial contexts; automation level is not itself a readiness level
status: STRONG SYNTHESIS
basis: readiness evidence concerns repeatability/control/rate; automation is separately justified in A7.

### P2-C-MAT-003 — Engineering intervention that is useful in DEV can become evidence of an uncontrolled production system in LVP/SVP
status: STRONG SYNTHESIS
needs case-study corroboration for Podcast Ready examples.

### P2-C-MAT-004 — Unit count alone cannot define the transition from DEV to LVP or LVP to SVP
status: STRONG SYNTHESIS
basis: NASA PRR focuses required quantity/readiness; DoD MRL uses environment, process control, resources, rate and production maturity rather than a universal quantity threshold.

## Applicability
Use this matrix as a conversation and evidence-planning tool. Tailor depth to product risk, complexity, regulation, lifecycle, volume and business model. A simple low-risk product may need far less formal evidence than aerospace, medical, automotive or safety-critical hardware.

## Next integration
1. Use listener checklist in show notes and episode research packs.
2. Use transition questions to audit Opening Arc A1–A8.
3. Feed configuration/change-control gaps into P2.02.
4. Feed quality evidence gaps into P2.03.
5. Feed pilot/rate gaps into P2.04.

## Readiness
Decision matrix: CAPTURED
Evidence boundaries: CAPTURED
Worked-example linkage: CAPTURED
Podcast-ready checklist: CAPTURED
P2.01 readiness package: NEAR PODCAST READY — technical review/source-note packaging remains