# Pass 2.03 — LVP Quality / PFMEA-to-Reaction Worked Example

status: ACTIVE — WORKED EXAMPLE
created_on: 2026-08-12
maps_to: Quality foundations; LVP readiness; Sentinel Node
companions: P2_03_QUALITY_CHAIN_WORKED_EXAMPLE.md; P2_03_MSA_SPC_CAPABILITY_NUMERICAL_EXAMPLE.md

## Purpose
Show what a hardware team should do during low-volume production when it has too little data to make mature process-capability claims, while still applying disciplined risk control, measurement, learning and reaction planning.

## Core principle
Low sample count is not permission to ignore quality engineering. It changes the strength and type of claims the team can make.

For a young LVP process, the useful sequence is:

Requirement/CTQ → PFMEA risk → prevention/detection control → measurement adequacy → time-ordered data → reaction plan → learning → updated controls → later capability evidence.

Do not force a mature Cpk claim from an immature dataset.

## Sentinel Node scenario
CTQ: connector seating depth.
Specification: 5.00 ± 0.20 mm.
Failure effect: insufficient seating can damage pins, compromise electrical contact and cause final-test failure.

During an early LVP build of 24 units, the team has not yet accumulated enough independent, representative observations to claim mature capability. NIST guidance notes that capability-index estimates generally need a sufficiently large sample, commonly about 50 independent observations, and assumes an in-control process and appropriate distributional assumptions.

Therefore the team does not use `Cpk >= X` as its primary LVP release argument.

## PFMEA → Control Plan linkage
### PFMEA entry — simplified teaching example
Process step: connector insertion.
Failure mode: connector not fully seated / skewed insertion.
Potential effects:
- damaged pins;
- intermittent electrical connection;
- final functional-test failure;
- possible latent field failure if detection coverage is inadequate.

Potential causes:
- fixture misalignment;
- excessive insertion force;
- operator technique;
- connector tolerance interaction;
- worn/damaged fixture datum;
- contamination or obstruction.

Controls should follow the identified causes/failure modes rather than exist as unrelated inspection paperwork.

### Control Plan — LVP phase
Characteristic: seating depth.
Method: qualified depth measurement method / fixture.
Frequency: initially 100% during controlled LVP learning phase.
Additional prevention:
- keyed/aligned fixture;
- defined insertion method;
- operator training;
- fixture condition check.

Additional detection:
- visual seating criterion;
- final electrical/functional test;
- damage inspection when abnormal insertion force or seating is observed.

The 100% measurement here is a temporary learning/containment decision, not proof that 100% inspection guarantees zero escapes.

## Reaction Plan
A Control Plan without a defined response to an abnormal result is incomplete operationally.

### Trigger A — individual unit outside specification
1. Stop release of the affected unit.
2. Identify and segregate the unit.
3. Do not automatically rework until the failure mechanism and allowed disposition are understood.
4. Check measurement validity.
5. Inspect connector/pins/PCB for collateral damage.
6. Record NCR/nonconformance and disposition.
7. Review adjacent units since the last known-good verification if a common cause is plausible.

### Trigger B — SPC/process-behavior signal while all units are still inside specification
1. Do not classify the units automatically as defective merely because the process signal fired.
2. Pause/contain the process as defined by risk.
3. Verify the measurement system and data integrity.
4. Check fixture, method, operator, material lot and recent changes.
5. Define the potentially affected time/serial window.
6. Correct assignable cause where found.
7. Verify restart conditions with defined evidence.
8. Update PFMEA/Control Plan if a new cause or inadequate control was discovered.

### Trigger C — final-test failure associated with connector damage
1. Contain affected WIP/finished units.
2. Link the failure back to the process step and as-built genealogy.
3. Confirm whether seating depth, insertion method or fixture condition is correlated.
4. Increase containment temporarily if justified.
5. Implement corrective action at the process, not only at final inspection.
6. Reduce enhanced inspection only after evidence supports doing so.

## What to do with only 20–30 units
The team can still make strong engineering progress without pretending it has mature capability statistics.

Use the early dataset to:
- preserve time order;
- identify obvious special causes and shifts;
- compare operators/lots/fixtures where meaningful;
- verify that the measurement method is fit for the decision;
- quantify observed yield and rework honestly;
- identify recurring failure modes;
- validate work instructions and reaction mechanisms;
- improve fixture/process design;
- accumulate representative data for later capability assessment.

Avoid statements such as:
- “Cpk is 1.6, therefore production is proven” from a tiny convenience sample;
- “24/24 passed, therefore defect rate is zero”;
- “everything is inside spec, therefore the process is stable”;
- “100% inspected, therefore no defect can escape.”

## LVP evidence ladder
### Level 0 — anecdotal
“We built some and they worked.”

### Level 1 — controlled observations
Configuration known, measurements recorded, failures traceable, method documented.

### Level 2 — repeatability evidence
Multiple builds/operators/lots show similar behavior; measurement and reaction system are functioning; special causes are being identified and removed.

### Level 3 — statistical process evidence
Sufficient representative data exist to evaluate stability and, where assumptions are justified, capability with stated uncertainty/limitations.

### Level 4 — sustained production evidence
The process maintains quality/rate under representative production conditions across time, normal variation, maintenance, material/supplier variation and controlled changes.

LVP normally aims to move deliberately through Levels 1–2 and begin earning Level 3; it should not claim Level 4 because one small build passed.

## Worked 24-unit interpretation
Suppose all 24 connector-depth measurements are within 4.80–5.20 mm and final test passes 23/24 units.

Correct conclusions may include:
- observed dimensional conformance was 24/24 for this build;
- observed final-test FPY was 23/24 = 95.8%;
- one failure requires failure-mechanism investigation;
- the build contributes evidence about the current controlled configuration/process.

Incorrect conclusions include:
- true long-term defect rate is 4.2%;
- process capability is proven;
- the process is statistically stable solely because all 24 dimensions were in specification;
- future lots/suppliers/operators are represented automatically.

## Quality feedback loop
A useful production quality system closes the loop:

PFMEA risk
→ Control Plan prevention/detection
→ actual production data
→ abnormality/failure
→ containment and root-cause work
→ corrective action
→ PFMEA update
→ Control Plan/work-instruction/test update
→ effectiveness verification

The PFMEA is therefore not a one-time pre-production document. Production learning should be able to change it.

## Listener tool — LVP Quality Gate
Before saying “our LVP process is ready,” ask:

1. What are the critical product/process characteristics?
2. Which failure modes matter and why?
3. Which controls prevent them and which only detect them?
4. Can the measurement system support the decision being made?
5. Is the data preserved in production/time order?
6. What happens when a unit is out of spec?
7. What happens when process behavior changes before a unit is out of spec?
8. Can we identify the potentially affected serial/lot/WIP population?
9. Are yield and rework calculated from honest denominators and definitions?
10. Have production failures changed PFMEA/Control Plan/work instructions where appropriate?
11. What claims can this sample size actually support?
12. What evidence must still be accumulated before capability or sustained-production claims are justified?

## Evidence guardrails
- AIAG training/materials explicitly link PFMEA information to construction of Control Plans and include reaction/control concepts.
- NIST defines process capability against specifications for an in-control/stable process and notes that capability-index estimates generally require sufficiently large independent samples; approximately 50 observations is given as a common rule of thumb.
- The specific Sentinel controls, triggers and reaction workflow above are a teaching synthesis, not a universal mandated AIAG/NIST procedure.
- Exact sampling frequency, capability acceptance thresholds, escalation rules and required studies depend on product risk, customer/sector requirements and the process.

## Podcast teaching line
**With 24 parts, your job is not to manufacture statistical confidence. Your job is to manufacture trustworthy evidence.**

## Next P2.03 work
1. package PFMEA → Control Plan → MSA → SPC → Capability → Reaction as one canonical visual/framework;
2. add source notes and applicability statements;
3. technical-review the numerical examples;
4. produce a one-page show-note quality checklist;
5. move P2.03 toward NEAR PODCAST READY.