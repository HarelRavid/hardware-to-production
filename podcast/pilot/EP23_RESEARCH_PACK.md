# Episode 23 Research Pack — DFMEA, PFMEA, Control Plans and Quality Gates

status: CLAIM SET STABLE
season: Season 4 — Prove Quality, Reliability & Compliance
primary_audience: Audience B — NPI / manufacturing / quality teams
secondary_audience: founders, design engineers, supplier quality, test engineers
lifecycle: LVP-FIRST / CROSS-STAGE
entry_point: INDEPENDENT PRACTITIONER ENTRY WITH SHORT RECAP
technical_depth: practitioner
backbone_anchor: P2.03 Quality Chain

## 1. Episode promise
Teach how product risk is translated into process controls without turning DFMEA, PFMEA and Control Plan into paperwork rituals.

Canonical listener question:
> How do we turn what can go wrong with the product and process into controls that actually prevent, detect and react to failures during production?

## 2. Navigation card
**You are here:** Production-intent design → controlled LVP → production validation.

**Best for:** teams preparing pilot/LVP builds, supplier transfer, controlled work instructions or quality plans.

**You should already know:** basic idea of requirements/CTQs; provide a short recap so standalone entry remains possible.

**You will leave with:** Risk-to-Control Chain worksheet + Quality Gate Design Check.

**Prototype shortcut:** engineering inspection and informal reactions can be acceptable while failure mechanisms are still being discovered.

**Shortcut expires when:** multiple operators/suppliers/units are involved, acceptance/release depends on the result, or the same failure mechanism can recur without a defined prevention/detection/reaction method.

**Next:** Episode 24 Production Testing/MSA → Episode 32 SPC/Capability → Episode 33 NCR/MRB/CAPA.

## 3. Audience contract
### DEV takeaway
Use early failure analysis to learn what characteristics and interfaces deserve attention; do not build a full production control bureaucracy around an unstable concept.

### Prototype shortcut
Informal engineering checks may be acceptable for a few learning units if failures remain visible and configuration is known.

### Shortcut expiration
As soon as repeat builds, supplier handoff or production release depends on the result, critical controls need defined method, ownership, evidence and reaction.

### LVP change
Translate recurring/product-critical risks into CTQs, process characteristics, controlled inspection/test, mistake prevention and reaction plans.

### SVP evidence
Controls must be demonstrated effective with capable measurement/process evidence and sustained reaction/learning loops.

### Manufacturing-debt prevention
Do not wait until pilot failure to decide what could go wrong and how the process should detect/prevent it.

## 4. Canonical quality chain
Requirement / function
→ product risk / DFMEA perspective
→ process step
→ process failure mechanism / PFMEA perspective
→ CTQ / key process characteristic
→ prevention control
→ detection control
→ measurement/test method
→ reaction plan
→ evidence / trend / CAPA learning

Episode guardrail:
DFMEA, PFMEA and Control Plan are related artifacts with different questions; they should not be collapsed into one checklist.

## 5. Core claim register — stabilized
| ID | Claim | Class | Priority | Status | Note |
|---|---|---|---|---|---|
| EP23-C01 | Product/design risk and manufacturing/process risk are related but distinct analysis perspectives. | V1/V2/V6 | P0 | SOURCE LOCATED / STABLE | AIAG-VDA FMEA handbook distinguishes Design FMEA and Process FMEA methods; exact handbook language still requires purchased-source verification before final script. |
| EP23-C02 | A PFMEA should connect process functions/failure modes/causes to prevention and detection controls rather than exist as isolated scoring paperwork. | V1/V6 | P0 | SOURCE LOCATED / STABLE | AIAG-VDA FMEA is the authoritative automotive reference method; exact forms/steps remain source-pack work. |
| EP23-C03 | A Control Plan is a structured manufacturing-control artifact linked to APQP/process planning and containing production controls/reaction logic. | V1 | P0 | SOURCE LOCATED / STABLE | AIAG CP-1, 1st Edition, published Mar 2024; final exact-field claims require manual verification. |
| EP23-C04 | Detection alone is not equivalent to prevention; risk reduction should consider preventing causes/failure mechanisms where practical. | V2/V6 | P1 | STABLE SYNTHESIS | General engineering lesson; do not present as a quoted AIAG rule unless exact source verified. |
| EP23-C05 | Measurement adequacy must be established before inspection/test data are treated as strong process-performance evidence. | V1/V2 + P2.03 | P0 | BACKBONE-STABLE / source pack open | Links Episode 24 and MSA. |
| EP23-C06 | Not every dimension should be controlled with equal rigor; control intensity should follow requirement/risk/process dependence. | V6 | P0 | STABLE SYNTHESIS | Do not imply a universal CTQ definition. |
| EP23-C07 | Reaction logic must define what happens to process and affected product/WIP when a control detects a problem. | V1/V2 | P0 | SOURCE LOCATED / STABLE | Control Plan source supports reaction-plan concept; exact wording requires CP-1 source review. |
| EP23-C08 | FMEA prioritization scores do not by themselves prove that risk is controlled. | V1/V6 | P0 | STABLE WITH GUARDRAIL | Discuss conceptually only; numeric tables/thresholds remain blocked until handbook is available. |
| EP23-C09 | Quality gates should be placed where they can prevent escape and avoid unnecessary downstream value-added loss, not simply at final inspection. | V6 + P2.03/P2.04 | P1 | BACKBONE-STABLE | Repository synthesis. |
| EP23-C10 | Control effectiveness must eventually be demonstrated with evidence, not inferred from document completion. | V6 + EFFECTIVENESS EVIDENCE | P0 | BACKBONE-STABLE | Cross-link case-study repair. |

## 6. Current authoritative-source map

### AIAG & VDA FMEA Handbook
Current AIAG product: **AIAG & VDA FMEA Handbook, 1st Edition** (product code FMEAAV-1). AIAG describes it as the harmonized automotive reference manual for Design FMEA, Process FMEA, and Supplemental FMEA for Monitoring and System Response.

Status for this episode:
- source located;
- full licensed handbook not yet ingested into project library;
- exact seven-step method language, tables, Action Priority logic and form details remain P0 verification items before PODCAST READY;
- AIAG errata page also lists an errata document for AIAG & VDA FMEA 1st Edition and must be checked together with the handbook.

Historical note:
AIAG still lists the older **FMEA 4th Edition** as a separate publication. Episode 23 must distinguish legacy/historical practice from the harmonized AIAG-VDA handbook rather than blending them.

### AIAG Control Plan
Current AIAG product: **Control Plan, 1st Edition**, product code CP-1, published March 2024.

AIAG states that Control Plan is now a standalone manual and provides clarification of requirements, linkage to APQP, plan-development guidance, and updated examples/forms/checklists.

Status for this episode:
- source located;
- exact field-level requirements and any Safe Launch details remain blocked until licensed manual verification;
- do not reuse obsolete APQP-embedded Control Plan assumptions without checking the new standalone manual.

### APQP relationship
AIAG currently lists **APQP 3rd Edition** and **Control Plan 1st Edition** separately. Episode 23 may mention their relationship, but APQP-specific required deliverables should remain out of scope unless verified directly from APQP-3.

## 7. Automotive-specific vs generalizable boundary

### Automotive-specific / source-controlled
Treat as automotive methodology unless separate source establishes broader applicability:
- AIAG-VDA FMEA method structure;
- exact FMEA forms/steps;
- Action Priority tables/logic;
- AIAG Control Plan required fields/phases;
- APQP-specific timing/deliverables;
- Safe Launch terminology in the AIAG Control Plan context.

### Generalizable engineering synthesis
Safe to teach as our cross-industry engineering model, while keeping it visibly labeled synthesis:
- connect risk to prevention/detection/reaction;
- distinguish design-side and process-side failure mechanisms;
- place controls near creation of risk where practical;
- verify measurement adequacy;
- preserve affected WIP/product identity;
- require evidence that controls remain effective;
- reassess controls after relevant design/process/supplier changes.

## 8. Listener tool — Risk-to-Control Chain
For each important product/process risk fill:

| Field | Question |
|---|---|
| Requirement/function | What must the product/process achieve? |
| Failure effect | What happens if it fails? |
| Failure mode | What observable failure can occur? |
| Cause/mechanism | Why could it happen? |
| Process step | Where can it be created or controlled? |
| Prevention | What reduces occurrence? |
| Detection | How do we know before escape? |
| Measurement | Can the method reliably distinguish good/bad? |
| Reaction | What happens to machine/process/WIP/product? |
| Evidence | What proves the control works over time? |

## 9. Quality Gate Design Check
Before adding a gate ask:
1. Which failure/claim does this gate protect?
2. Is prevention available upstream?
3. Is the characteristic measurable with adequate method?
4. Is 100% inspection really justified/necessary?
5. What happens when the gate fails?
6. Can affected WIP/serials/lots be identified?
7. Who may disposition/release?
8. Does the control survive operator/shift/supplier variation?
9. How will we know the control is effective over time?
10. Does a process/design change invalidate this control plan?

## 10. Sentinel Node worked example
Failure: connector is only partially seated, causing intermittent field communication.

### Product/design perspective
Potential effects:
- intermittent function;
- field failure;
- difficult diagnosis.

Potential design-side considerations:
- connector geometry/retention;
- access/alignment;
- feedback that seating is complete;
- tolerance stack.

### Process perspective
Process step: connector insertion.

Potential causes:
- wrong orientation;
- insufficient insertion force/stroke;
- damaged part;
- fixture misalignment;
- supplier dimensional variation.

Potential prevention:
- keyed orientation;
- controlled fixture;
- approved supplier/specification;
- defined insertion method.

Potential detection:
- force/displacement signature;
- seating-depth check;
- functional test where appropriate.

Reaction:
- stop/contain defined population;
- diagnose cause;
- rework only by approved method;
- record original fail and final disposition;
- reopen risk/control evidence if repeated signal occurs.

Episode lesson:
A final functional test may catch some failures, but a robust control chain asks whether the defect can be prevented or detected closer to creation and whether the measurement/reaction system is trustworthy.

## 11. Applicability statement
This episode teaches a general risk-to-control engineering chain using DFMEA/PFMEA/Control Plan concepts. Automotive AIAG/VDA manuals are authoritative only for claims within their documented scope/methodology. Other industries may use different mandated risk and quality planning methods. The listener framework is repository synthesis and must not be presented as a universal standard requirement.

## 12. What this episode must NOT claim
- every company must use AIAG/VDA FMEA;
- an RPN or AP threshold universally determines action;
- completing PFMEA proves a process is controlled;
- final inspection can replace process control;
- 100% inspection is always superior;
- every dimension is a CTQ;
- measurement data are trustworthy without considering measurement-system adequacy;
- a Control Plan remains valid after relevant design/process/supplier changes without impact review.

## 13. Common failure modes
### Paper FMEA
Document is updated for audit but does not change process/design controls.

### Copy-paste PFMEA
A generic process FMEA is reused without matching actual process sequence/configuration.

### Detection-heavy quality
Many inspections, little upstream prevention.

### No reaction ownership
A check has limits, but nobody knows what to stop, contain or escalate when it fails.

### Measurement blind spot
A control limit is tighter than the measurement method can credibly resolve.

### Risk score worship
Teams focus on one numeric ranking while severe failure mechanisms or weak controls remain unresolved.

## 14. Quantitative / scoring guardrail
This episode explains FMEA prioritization conceptually but does **not** teach numeric scoring tables or action thresholds until the exact licensed handbook content and errata are verified.

If RPN versus Action Priority is discussed in the final script:
- state the exact handbook/edition;
- distinguish legacy FMEA 4th Edition usage from AIAG-VDA methodology;
- reproduce no controlled table beyond licensing permissions;
- do not create universal numeric action thresholds;
- explain that a prioritization result is not itself evidence that a control works.

## 15. Remaining work before EVIDENCE VERIFIED
1. Ingest licensed AIAG-VDA FMEA 1st Edition and current errata.
2. Ingest licensed AIAG Control Plan 1st Edition.
3. Verify exact DFMEA/PFMEA terminology, method steps and reaction/control fields.
4. Decide final scope of RPN/AP discussion after handbook review.
5. Cross-check Episode 24 MSA and Episode 32 SPC boundaries.
6. Technical review: quality + manufacturing/NPI.

These are source-pack tasks, not claim-set instability.

## 16. Pilot-test objective
Episode 23 tests the Episode Packaging Contract under a standards/manual-heavy practitioner topic.

Pilot PASS signal:
A listener should be able to take one meaningful failure mode and build a coherent chain from requirement/risk → process cause → prevention → detection → measurement → reaction → effectiveness evidence, while understanding which parts are AIAG/VDA methodology and which parts are general synthesis.

## 17. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: HIGH
Quantitative burden: MEDIUM
Backbone risk: CONTROLLED
Source verification: SOURCE LOCATED / licensed-text verification pending
Claim stability: STABLE

Next status target:
`CLAIM SET STABLE → EVIDENCE VERIFIED` after licensed-source ingestion and technical review.
