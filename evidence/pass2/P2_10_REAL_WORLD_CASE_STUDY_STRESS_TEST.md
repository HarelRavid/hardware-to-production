# P2.10 — Real-World Case Study Stress Test

Status: ACTIVE
Provenance: mixed. Public-source case facts require source-level citation packaging before Podcast Ready. Framework mappings are [GNR] synthesis.

## Purpose

P2.10 is not a collection of interesting manufacturing stories. It is the final stress test of Knowledge Backbone V1.

For each case:
1. establish only facts supported by credible public evidence;
2. reconstruct the failure/response chain without hindsight simplification;
3. map the case to existing Pass-2 frameworks;
4. identify where a framework explains the case well;
5. identify where the backbone is weak or missing a concept;
6. repair the backbone before V1 freeze if needed.

Canonical question:

> If our frameworks cannot explain a documented real manufacturing failure or recovery, the framework is not finished.

## Case-selection criteria

A useful case should provide several of the following:
- credible primary/official investigation or company disclosure;
- identifiable design/process/supplier/configuration issue;
- transition from prototype/development to production or scale;
- quality/safety consequences;
- evidence of containment/recovery/change;
- supply-chain or production-system effects;
- enough public detail to avoid speculation.

Cases are selected for learning value, not blame.

---

# Case A — Samsung Galaxy Note7 battery failures and recall

## Public evidence anchors to package

Public reporting and Samsung disclosures describe two battery populations/suppliers with different failure mechanisms. Samsung's investigation reportedly used approximately 200,000 phones, 30,000 batteries and hundreds of engineers, and the company subsequently introduced an expanded battery safety/quality process.

Source packaging should prioritize Samsung's investigation/process disclosures and regulator/independent technical material; secondary reporting may be used for narrative context.

## Backbone stress test

### P2.01 — Hardware Evolution

Question:
- Which assumptions that were acceptable during product development became unacceptable at mass-production scale and field exposure?

Lesson candidate:
- successful design verification or launch evidence does not automatically establish robustness across supplier/process distributions and production volume.

### P2.02 — Configuration / Change / Effectivity

The replacement population matters. A recall/replacement is not merely “same product, fixed.” The changed battery population has its own configuration/evidence envelope.

Questions:
- Can affected units be identified by configuration/supplier population?
- What evidence supports the replacement configuration?
- Which previous claims remain valid and which require new verification?

### P2.03 — Quality Chain

Strong fit.

Potential chain:
Critical battery requirement → failure mechanism → supplier/process controls → detection/testing → field signal → containment → investigation → revised controls.

Stress-test question:
- Would our PFMEA/Control Plan/measurement/reaction logic force different failure mechanisms from different suppliers to be treated separately rather than hidden under one defect label?

### P2.06 — Supplier Industrialization

Very strong fit.

Lesson candidate:
> A second source is not automatically a qualified corrective action merely because it removes exposure to the first supplier's failure mechanism.

Supplier B must earn its own evidence inside its own process envelope.

### P2.08 — Manufacturing Atlas

Traceability/effectivity become essential during recall and replacement.

Questions:
- Which product contains which battery population?
- Which production date/lot/supplier/process configuration applies?
- Can field population and corrective action be reconstructed?

## Framework weakness exposed

Existing backbone handles supplier/process/configuration evidence well, but field-return/recall evidence is not yet explicit enough.

### Proposed backbone addition — FIELD EVIDENCE LOOP

Production release → Field population → Incident/return signal → Population segmentation → Containment/recall → Root-cause evidence → Corrective configuration → Revalidation → Field effectiveness monitoring.

This should become a cross-link to P2.03, P2.06 and P2.08 before V1 freeze.

---

# Case B — Norsk Hydro 2019 cyberattack and manufacturing recovery

## Public evidence anchors to package

Hydro publicly states that the March 2019 cyberattack affected its global organization. Extruded Solutions suffered the greatest operational disruption; other business areas were able to operate near normally using labor-intensive workarounds/manual procedures. Hydro described a staged recovery in which PCs and servers were reviewed, cleaned and safely restored, and reported that one week after the attack many operations had returned toward normal while some plants still used manual operation.

Primary source priority: Norsk Hydro incident/update pages; add government/technical post-incident sources if available.

## Backbone stress test

### P2.09 — OT/ICS Cybersecurity

Extremely strong fit.

The case validates a core distinction:

> Restoring IT assets is not identical to restoring trusted manufacturing capability.

Questions:
- Which production capabilities can continue manually?
- Which dependencies prevent safe/controlled production?
- How is restored infrastructure trusted before reconnection?
- What degraded modes are allowed?

### P2.04 — Capacity / Ramp

Manual workaround is a different production envelope.

A plant operating manually after cyber disruption may have:
- lower throughput;
- different staffing;
- different quality controls;
- changed WIP behavior;
- different recovery risk.

Therefore “production resumed” must not be translated automatically into “normal capacity restored.”

### P2.08 — Manufacturing Atlas

Stress-test questions:
- Can genealogy still be maintained in degraded/manual mode?
- Can data generated during manual operation later be reconciled?
- What is the source of truth when normal systems are unavailable?

### P2.02 — Configuration

Recovery must distinguish a technically running PLC/server/workstation from the approved/trusted configuration.

## Framework weakness exposed

P2.09 already states Backup ≠ Recovery, but the backbone needs a clearer concept of **degraded manufacturing mode**.

### Proposed backbone addition — MINIMUM CONTROLLED PRODUCTION MODE

A deliberately bounded operating mode used when normal manufacturing information/control infrastructure is unavailable.

Minimum questions:
1. What products/processes are permitted?
2. What controls remain available?
3. Which controls are replaced manually?
4. What throughput is allowed?
5. How is genealogy preserved?
6. How are deviations recorded?
7. What release authority applies?
8. How is later reconciliation performed?
9. What conditions force shutdown?
10. What evidence is required to return to normal mode?

Do not claim this term is an IEC 62443 or NIST normative term; it is our synthesis.

---

# Case C — Boeing 737 MAX as a system-safety/configuration evidence case

## Scope guardrail

This case must be handled carefully. It is not primarily a factory process-capability case, and public discussion often collapses certification, software design, human factors, training and manufacturing into one story.

Use official accident/investigation/regulatory sources before episode packaging. Do not use this case to make claims about manufacturing causes that the official evidence does not support.

## Why include it

It stress-tests whether the Hardware-to-Production backbone can handle a product whose critical behavior emerges from hardware + software + sensor + human + operating-context interaction.

### P2.02 — Configuration

Questions:
- Is software behavior part of the product configuration baseline?
- Are hardware/sensor/software/training dependencies represented in effectivity?
- Can a change be “small” in physical BOM terms but system-critical?

This supports the existing principle:

> Product configuration is not only mechanical BOM revision.

### P2.03 — Quality / Evidence

A test result is meaningful only relative to the claim it supports.

Stress-test question:
- Did verification evidence exercise the relevant failure combinations, operating states and human-system interactions?

### P2.07 — Automation / Safety

Strong conceptual fit around automated control authority, abnormal states, recovery and human-machine interaction.

Guardrail:
- factory automation and aircraft flight-control certification are different domains; use the case to illustrate systems-thinking, not to import machinery standards into aviation.

## Framework weakness exposed

The backbone has configuration and qualification, but cross-domain **system interaction evidence** should be more explicit.

### Proposed addition — INTERACTION CLAIM

A claim whose validity depends on multiple configured elements acting together, e.g. hardware + firmware + sensor + operator procedure + environment.

Evidence for individual components does not automatically prove the interaction claim.

Cross-link to P2.02, P2.03 and P2.07.

---

# Cross-case comparison

| Dimension | Note7 | Norsk Hydro | 737 MAX |
|---|---|---|---|
| Product/process configuration | High | Medium | Very high |
| Supplier/process variation | Very high | Low/indirect | Case-specific |
| Quality/field evidence | Very high | Medium | Very high |
| Capacity/continuity | Medium | Very high | Low for selected scope |
| Digital thread/traceability | High | High | High |
| Automation/software interaction | Medium | High | Very high |
| Cybersecurity | Low | Very high | Out of selected scope |
| Recovery/requalification | High | Very high | High |

## What survived the stress test

The following existing frameworks remain strong:
- DEV/LVP/SVP evidence maturity;
- configuration/effectivity envelope;
- Quality Chain;
- supplier evidence envelope;
- capacity versus temporary rate;
- recovery qualification;
- Manufacturing Atlas reconstruction;
- OT cyber → manufacturing evidence link.

## What the cases added

Three concepts should be added before Backbone V1 freeze:

1. **FIELD EVIDENCE LOOP** — production evidence must continue into field population, returns, incidents, recalls and corrective-effectiveness monitoring.
2. **MINIMUM CONTROLLED PRODUCTION MODE** — degraded/manual production after infrastructure loss requires an explicitly bounded control and evidence envelope.
3. **INTERACTION CLAIM** — evidence for individual components does not automatically establish claims that depend on configured hardware/software/human/environment interaction.

These are refinements, not evidence that the existing architecture failed.

---

# CASE 12 — listener framework

When studying a real manufacturing case, ask:

1. What is actually documented versus inferred?
2. What claim failed: function, quality, safety, rate, cost, security or recovery?
3. Which configuration/population was affected?
4. What failure mechanism is supported by evidence?
5. What controls should have prevented or detected it?
6. What evidence existed before release?
7. What evidence appeared only in production/field operation?
8. How was the affected population identified and contained?
9. What changed in the corrective configuration/process?
10. What had to be revalidated?
11. How was effectiveness demonstrated after the change?
12. Which framework assumption does this case challenge?

# Case-study provenance rules

For Podcast Ready:
- prefer official investigation/regulator/company technical disclosure for factual claims;
- separate confirmed fact from interpretation;
- never infer causation from chronology alone;
- never use a famous case as evidence for an unrelated standard requirement;
- state domain-transfer limits explicitly;
- distinguish what was known before the event from hindsight knowledge;
- avoid blame-oriented language where system/process analysis is more accurate;
- attach source to each consequential factual claim.

# P2.10 next step

Before marking NEAR PODCAST READY:
1. add at least one production-ramp/capacity case with strong primary evidence;
2. add one supplier/quality case from a regulated or high-volume manufacturing domain with official investigation material;
3. populate source packets for each selected case;
4. update the affected canonical packs with FIELD EVIDENCE LOOP, MINIMUM CONTROLLED PRODUCTION MODE and INTERACTION CLAIM;
5. run a Pass-2 cross-framework contradiction audit.

P2.10 remains ACTIVE.
