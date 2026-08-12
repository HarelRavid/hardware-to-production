# P2.07 — Automation Qualification / Release Gate + Safety Applicability Map

Status: ACTIVE — RELEASE GATE CAPTURED
Provenance: [GNR] synthesis; standards applicability/version/clauses require source-level verification before Podcast Ready.

## Purpose

Define the evidence required before an automated or semi-automated manufacturing process is released for production, and prevent the common error of treating a robot/cobot component label as proof that the integrated application is safe and production-ready.

Canonical chain:

Manufacturing need → Process/failure mechanism → Automation concept → Risk assessment → Design/integration verification → Process qualification → Rate/recovery demonstration → Controlled release → Monitoring → Change/requalification

## Sentinel Node application

Process: connector insertion and seating verification.

Candidate solution: operator-loaded semi-automatic station with keyed nest, controlled force/displacement insertion, automatic seating verification, serial-number association and result capture.

The release claim is deliberately narrow:

> The station is released to manufacture the approved Sentinel Node configuration within the demonstrated product/process envelope, using trained personnel and controlled recipes/tooling, at the demonstrated production conditions.

It is NOT a claim that:
- every future product variant is qualified;
- every supplier substitution is covered;
- every recipe change is harmless;
- the cell is safe under unassessed modifications;
- the demonstrated OEE is guaranteed indefinitely;
- the station automatically establishes system-level capacity.

## AUTOMATION RELEASE 12

### Gate 1 — Problem and requirement

Evidence:
- manufacturing problem is defined;
- CTQs/failure mechanisms are identified;
- required quality/rate/safety outcomes are explicit;
- simpler interventions were considered.

Sentinel example: prevent connector misalignment/pin damage while controlling seating depth and preserving traceability.

### Gate 2 — Configuration baseline

Evidence:
- approved machine/tooling configuration;
- PLC/robot/software/recipe versions identified;
- product/BOM/firmware variants inside the qualified envelope identified;
- calibration/configuration files controlled.

Connect to P2.02: released definition must be distinguishable from as-built/as-run configuration.

### Gate 3 — Risk assessment and safeguards

Evidence:
- hazards assessed at application/task level;
- normal and abnormal operating modes considered;
- safeguards/protective functions selected and verified as applicable;
- residual risk communicated and controlled.

Hard stop: a robot or cobot component declaration does not replace application-level risk assessment.

### Gate 4 — Installation and integration verification

Evidence:
- utilities and interfaces correct;
- sensors/actuators/interlocks behave as intended;
- tooling is installed and identified;
- network/data interfaces work;
- safe-state behavior is verified for relevant utility/interface losses.

### Gate 5 — Measurement and quality adequacy

Evidence:
- CTQ measurement is fit for purpose;
- force/displacement/seating logic is correlated to actual product quality;
- false accept and false reject behavior are understood;
- test records associate correctly to product genealogy.

Connect to P2.03: automation does not remove the need to trust the measurement system.

### Gate 6 — Process envelope

Evidence:
- expected component/material variation exercised;
- tooling wear or drift considered;
- recipe/process limits defined;
- environmental/utility variation addressed where relevant;
- boundary conditions and prohibited conditions documented.

### Gate 7 — Fault detection and containment

Evidence:
- representative faults deliberately injected;
- unsafe/unknown product states are contained;
- suspect WIP can be identified;
- genealogy is preserved through fault handling.

Sentinel injections include wrong orientation, partial insertion, sensor disagreement, recipe mismatch and jam.

### Gate 8 — Recovery and restart

Evidence:
- fault is diagnosable;
- required skill level is known;
- safe recovery sequence is defined;
- restart does not bypass quality controls;
- first-good-piece/restart verification is defined where needed;
- MTTR/recovery burden is measured for dominant losses.

### Gate 9 — Rate and sustainable flow

Evidence:
- cycle-time distribution measured;
- accepted throughput demonstrated;
- availability/recovery losses included;
- rework burden included;
- WIP/queue behavior observed;
- system bottleneck impact understood.

Connect to P2.04: machine speed is not system capacity.

### Gate 10 — Maintainability

Evidence:
- preventive maintenance defined;
- calibration/verification intervals controlled;
- wear items and spares identified;
- service access and recovery responsibilities defined;
- maintenance actions that can alter configuration trigger control/reverification as needed.

### Gate 11 — Economics and operating model

Evidence:
- staffing and support assumptions are realistic;
- maintenance/downtime/yield assumptions are evidence-linked;
- lifecycle economics remain acceptable;
- automation addresses the real constraint/problem.

Connect to P2.05: lowest nominal unit cost does not prove best investment.

### Gate 12 — Release, monitoring and change control

Evidence:
- release authority defined;
- approved envelope documented;
- production monitoring/reaction plan defined;
- software/recipe/tooling/product/supplier changes have triggers for impact assessment;
- requalification scope is risk/evidence based.

Connect to P2.02: approval is valid only inside the demonstrated configuration/process envelope.

## Release outcomes

GREEN — released inside the demonstrated envelope.

AMBER — conditional release with explicit containment, owner, expiry/stop condition and closure evidence.

RED — critical evidence missing or contradictory; production release unsupported.

No arithmetic score may override a RED hard stop in safety, configuration identity, quality detection, uncontrolled fault/recovery behavior or inability to identify affected product.

## Safety applicability map

This is an applicability map, not a declaration that every listed standard applies to every machine. Exact editions, regional adoption, legal status and clauses must be verified during source packaging.

### Layer A — Machinery/system risk

Typical question:
- What hazards are created by the complete machine/system and how are risks reduced?

Common reference family to verify:
- ISO 12100 — machinery risk assessment and risk reduction principles.

Use as conceptual backbone for hazard identification/risk reduction, subject to current edition/applicability review.

### Layer B — Safety-related control functions

Typical question:
- What safety function is required, and what integrity/performance must the safety-related control system achieve?

Common reference families to verify:
- ISO 13849 series;
- IEC 62061.

Do not present these as interchangeable without an applicability/design-method explanation.

### Layer C — Robot system / robot application

Typical question:
- What requirements apply to the industrial robot and integrated robot application?

Common reference family to verify:
- ISO 10218 series.

Key podcast guardrail:

> Compliance of a robot component is not compliance of the integrated robot application.

### Layer D — Collaborative operation

Typical question:
- If human and robot share workspace/tasks, what hazards, limits, contact scenarios and protective measures apply?

Reference family to verify against current ISO 10218 treatment and current status of ISO/TS 15066 or successor/integrated requirements.

Do not use “cobot” as a safety conclusion.

### Layer E — Electrical equipment of machinery

Typical question:
- What electrical design, protective, control and documentation requirements apply to the machine electrical equipment?

Common reference family to verify:
- IEC 60204-1.

### Layer F — Guards, interlocks and protective devices

Typical questions:
- How are access and hazardous motion controlled?
- What guarding/interlocking/protective-device requirements apply?

Potential reference families depend on solution and must be verified, e.g. guard/interlock/electro-sensitive protective-device standards.

### Layer G — Regional legal/regulatory framework

The engineering standard stack sits inside jurisdiction-specific legal requirements. EU machinery law/CE obligations, US OSHA/consensus-standard context, Israeli requirements or other local frameworks cannot be inferred from the generic engineering map. Episode claims must state jurisdiction where legal obligations are discussed.

## Safety claim hierarchy

Weak claim:
“The cobot is safe.”

Better claim:
“The robot has safety-rated features.”

Engineering claim:
“The integrated application has been risk-assessed and the required protective measures/functions have been designed and verified for the defined tasks and operating modes.”

Evidence-backed release claim:
“The approved application configuration has demonstrated the defined safety functions and operating controls inside its assessed envelope; changes are controlled and reassessed when they can affect risk.”

## Change/requalification triggers

Automation release must be reconsidered when changes can affect the evidence envelope, including:
- product geometry/variant;
- connector/supplier/material substitution;
- tooling/nest geometry;
- robot/PLC/control software;
- recipe limits;
- sensor or safety-device replacement;
- guarding/layout;
- cycle-speed increase;
- staffing/task allocation;
- recovery procedure;
- network/data architecture where it affects safe/reliable operation;
- maintenance modification.

Decision logic:

Change → affected claim/hazard/CTQ → evidence dependency → invalidated assumption? → targeted reverification/requalification → effectivity → controlled release.

## Sentinel Node release decision example

Assume the semi-automatic station demonstrates:
- keyed alignment prevents wrong orientation;
- force/displacement signature detects partial insertion;
- seating-depth measurement is adequate;
- serial/result association is verified;
- injected fault/recovery cases pass;
- dominant recovery burden is acceptable;
- accepted throughput supports the required envelope;
- maintenance/calibration controls exist;
- approved product/tooling/recipe configuration is baselined.

Then GREEN release is justified only for that envelope.

If the connector supplier changes and insertion-force distribution shifts, the correct action is not “machine already qualified.” The change enters P2.02/P2.06 logic, affected process/quality evidence is identified, and targeted requalification is performed before unrestricted release.

## Listener tool — RELEASE 12

Before saying “the automation is production ready,” ask:

1. What exact production claim are we releasing?
2. Which product and machine configurations does it cover?
3. What hazards and abnormal states were assessed?
4. Were safeguards and safety functions verified at application level?
5. Can we trust the CTQ/test measurement?
6. What process variation was exercised?
7. What happens when faults occur?
8. Can normal operators/technicians recover safely and correctly?
9. Was accepted throughput sustained under representative conditions?
10. Can the cell be maintained without losing control of configuration/quality?
11. Does the economics case survive actual yield/availability/support evidence?
12. Which changes force reassessment or requalification?

## Canonical P2.07 chain

Problem
→ Mechanism
→ Simplest effective intervention
→ Automation level
→ Risk/safety architecture
→ Qualification
→ Measurement/quality
→ Fault/recovery
→ OEE/loss decomposition
→ Sustainable system throughput
→ Maintainability/economics
→ Controlled release
→ Monitoring/change/requalification

## P2.07 completion assessment

Existing package now includes:
- automation intervention ladder;
- Sentinel Node worked example;
- OEE worked example;
- equal-OEE/different-loss example;
- fault/recovery dataset;
- AUTOMATE 10;
- LOSS 8;
- RELEASE 12;
- automation qualification/release gate;
- safety applicability map;
- cross-links to configuration, quality, capacity and economics logic.

Remaining before Podcast Ready:
1. verify current editions/status and exact applicability of safety standards;
2. attach primary-source citations/clauses appropriate to episode claims;
3. technical review of safety language;
4. episode-level source-note packaging.

Recommended status after this artifact: NEAR PODCAST READY.
