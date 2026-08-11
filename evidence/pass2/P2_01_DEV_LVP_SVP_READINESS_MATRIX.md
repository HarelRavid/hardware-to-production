# Pass 2.01 — DEV / LVP / SVP Readiness Matrix

status: ACTIVE — WORKED DECISION TOOL
created_on: 2026-08-11
maps_to: Opening Arc A1–A8; Episodes 1–5, 26–31, 60
companion: P2_01_HARDWARE_READINESS_DEFINITIONS.md; P2_01_WORKED_EXAMPLE_SENTINEL_NODE.md

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

Optimized for:
- learning speed;
- technical-risk retirement;
- architecture exploration;
- requirements discovery/refinement;
- fast iteration.

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

Exit direction toward LVP:
The product and production-intent definition must become stable enough that repeated builds teach us about the intended production system rather than only about prototype craftsmanship.

### LVP — Low-Volume Production / Learning Production System
Primary question: **Can ordinary production resources repeatedly build conforming units using a controlled, increasingly representative process?**

Optimized for:
- repeatability learning;
- production-risk retirement;
- yield/defect discovery;
- operator and work-instruction learning;
- supplier/process qualification;
- test/inspection validation;
- capacity-model validation;
- controlled engineering change.

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

Red flags:
- every unit needs engineering intervention;
- configuration cannot be reconstructed;
- process settings depend on tribal knowledge;
- production route changes without revalidation assessment;
- yield only reported after rework;
- rate calculated from ideal machine cycle rather than accepted system output;
- supplier qualification inferred from one good sample.

Exit direction toward SVP:
Demonstrate that the integrated production system can sustain required output, quality and economics under defined operating assumptions without exceptional intervention.

### SVP — Scaled / Serial Volume Production
Primary question: **Can the production system sustain the business-required rate, quality, cost and change discipline over time?**

Optimized for:
- sustained output;
- controlled variation;
- predictable quality/cost/delivery;
- supply resilience;
- maintenance and recovery;
- scalable training/operations;
- controlled product/process change;
- field/service feedback and continuous improvement.

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

Red flags:
- volume increase is achieved only through overtime/firefighting;
- quality is maintained only by sorting/containment;
- automation hides an unstable process;
- alternate suppliers/components bypass qualification;
- change implementation cannot identify affected serial/lot range;
- cost model still relies mainly on prototype quotations/ideal cycle assumptions.

## Readiness matrix by dimension

| Dimension | DEV | LVP | SVP |
|---|---|---|---|
| Product requirements | learning/refining critical requirements | controlled requirements sufficient for production validation | controlled requirements with disciplined change/field feedback |
| Configuration | enough identity to know what was tested | reproducible controlled build configuration | full effectivity/change cut-in/genealogy discipline |
| Materials/components | prototype substitutes may be acceptable if explicit | increasingly production-intent and qualified | controlled approved sources with resilience/change rules |
| Manufacturing process | chosen to answer engineering questions | representative route proven through repeated builds | controlled route sustaining rate/quality/cost |
| Tooling/fixtures | temporary/rapid tooling acceptable | production-representative for critical operations | production-capable, maintained, controlled, spare/recovery strategy |
| Work instructions | engineer knowledge may dominate | operators can execute defined work with bounded support | scalable standard work/training/change control |
| Measurement/test | lab-grade/engineering test acceptable | production test/inspection adequacy demonstrated | validated, maintained measurement/test system with reaction plans |
| Quality controls | defect discovery and learning | PFMEA/control-plan/reaction logic functioning in practice | controls demonstrate sustained effectiveness and capability |
| Yield/rework | informative but often not production representative | FPY/rework/scrap captured by operation/failure mode | sustained yield economics and improvement system |
| Suppliers | availability/technical exploration | qualification, first-article/PPAP-type evidence as applicable | ongoing capability, change control, sub-tier/resilience management |
| Rate/capacity | generally not proven | bottleneck/rate assumptions tested in representative runs | sustained capacity under representative mix/downtime/staffing |
| Automation | avoid locking unstable work unless learning requires it | targeted/semi-automation often valuable | automation justified by TCO, qualified, maintainable, change-aware |
| Traceability | enough to preserve engineering learning | enough to reconstruct builds, defects and changes | scalable genealogy/effectivity/auditability |
| Economics | rough architecture/process tradeoffs | cost per good part begins using actual yield/labor/process data | actual TCO/cost/capacity behavior drives decisions |
| Service/lifecycle | identify foreseeable service constraints | serviceability/spares/diagnostics increasingly validated | field-return/service data closes loop to product/process controls |

## What is allowed to stay “dirty”?
The right question is not whether a shortcut exists. It is whether the shortcut:
1. is visible;
2. is bounded to a maturity stage/use case;
3. does not invalidate the evidence being claimed;
4. has an owner/expiration trigger;
5. is retired before it becomes a hidden production dependency.

### Example — acceptable DEV shortcut
Sentinel Node uses a bench power supply instead of the target internal power architecture to validate the sensing principle.

Valid evidence: sensing concept can work under controlled electrical conditions.
Invalid inference: target power architecture, EMC behavior, thermal behavior and production test are validated.

### Example — dangerous LVP shortcut
Every Sentinel Node requires the design engineer to manually adjust a hidden calibration coefficient until final test passes.

This is no longer merely fast learning. It is evidence that the production definition/process/test system is incomplete or uncontrolled.

## Evidence-transfer rule
Evidence transfers forward only when the changed configuration/process/environment does not invalidate the question previously answered.

At every major change ask:
- What requirement was the old evidence supporting?
- What physical/process assumptions made that evidence valid?
- Which of those assumptions changed?
- Does the change require analysis, partial regression, requalification or full re-verification?

This prevents the common failure mode: “we tested it on the prototype” when the production-intent material, geometry, supplier, firmware, tooling or assembly method has changed.

## Minimum transition questions

### DEV → LVP
- Is the build configuration reproducible?
- Are production-intent differences from prototypes explicit?
- Can non-designers build/test it from controlled information?
- Are CTQs/failure mechanisms linked to controls?
- Can we identify what changed between units/lots?
- Are critical suppliers/processes sufficiently representative?
- Will the planned build teach us about the intended production route?

### LVP → SVP
- Is accepted output sustainable, not just briefly demonstrated?
- What is the true constraint/bottleneck?
- What happens to yield and cycle time without engineering rescue?
- Are measurement and controls trustworthy for CTQ decisions?
- Can supply support planned rate and changes?
- Are maintenance/downtime/recovery included in capacity?
- Is cost per good part based on actual production behavior?
- Can product/process changes be cut in without losing genealogy or evidence?

## Podcast listener tool — “Where are we lying to ourselves?”
Ask five questions:
1. **What are we claiming is ready?** Technology, design, process, supplier, quality system, rate or business economics?
2. **What evidence proves that specific claim?**
3. **Was the evidence generated with a representative configuration/process/environment?**
4. **What expert intervention or hidden workaround was required?**
5. **What changes since the evidence was generated could invalidate it?**

If the team cannot answer these, the readiness label is probably ahead of the evidence.

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
1. Map Sentinel Node examples into each matrix row.
2. Convert the matrix into a compact listener checklist for show notes.
3. Use the transition questions to audit Opening Arc A1–A8.
4. Feed configuration/change-control gaps into P2.02.
5. Feed quality evidence gaps into P2.03.
6. Feed pilot/rate gaps into P2.04.

## Readiness
Decision matrix: CAPTURED
Evidence boundaries: CAPTURED
Worked-example linkage: PARTIAL — NEXT
Podcast-ready checklist: NEXT
