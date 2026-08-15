# Episode 23 Research Pack — DFMEA, PFMEA, Control Plans and Quality Gates

status: RESEARCH PACK OPEN
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

## 5. Core claim register — draft
| ID | Claim | Class | Priority | Status | Note |
|---|---|---|---|---|---|
| EP23-C01 | Product/design risk and manufacturing/process risk are related but distinct analysis perspectives. | V1/V2/V6 | P0 | UNVERIFIED | Exact AIAG-VDA framing requires source verification. |
| EP23-C02 | A PFMEA should connect process steps/failure modes to controls and reaction rather than exist as isolated scoring paperwork. | V1/V6 | P0 | UNVERIFIED | Standards/manual source needed. |
| EP23-C03 | A Control Plan should reflect the characteristics, controls, methods and reactions needed to control the manufacturing process. | V1 | P0 | UNVERIFIED | AIAG Control Plan exact edition/source required. |
| EP23-C04 | Detection alone is not equivalent to prevention; stronger process design can remove or reduce failure opportunities upstream. | V2/V6 | P1 | UNVERIFIED | Support via quality/mistake-proofing sources. |
| EP23-C05 | Measurement adequacy must be established before using inspection/test data as strong evidence of process performance. | V1/V2 + P2.03 | P0 | BACKBONE-STABLE / source pack open | Links Episode 24. |
| EP23-C06 | Not every dimension should be controlled with equal rigor; control intensity should follow requirement/risk/process dependence. | V6 | P0 | CLAIM DRAFT | Avoid unsupported universal CTQ definitions. |
| EP23-C07 | Reaction plans should define what happens to process, WIP/product and escalation when a control detects loss of control/nonconformance. | V1/V2 | P0 | UNVERIFIED | Exact Control Plan/manual support required. |
| EP23-C08 | FMEA scoring or RPN/AP-style prioritization does not by itself prove risk is controlled. | V1/V6 | P0 | UNVERIFIED | Need exact AIAG-VDA language and careful edition distinction. |
| EP23-C09 | Quality gates should be placed where they can prevent escape and minimize downstream value-added loss, not simply at final inspection. | V6 + P2.03/P2.04 | P1 | BACKBONE-STABLE | Synthesis; source enrichment useful. |
| EP23-C10 | Control effectiveness must eventually be demonstrated with evidence, not inferred from document completion. | V6 + EFFECTIVENESS EVIDENCE | P0 | BACKBONE-STABLE | Cross-link case-study repair. |

## 6. Standards / source targets
P0 verification targets before EVIDENCE VERIFIED:

- AIAG & VDA FMEA Handbook — current applicable edition/status.
- AIAG Control Plan reference/manual — current edition/status.
- AIAG APQP only where the episode makes APQP-specific claims.
- AIAG MSA for measurement-system claims carried into Episode 24.
- AIAG SPC for process-monitoring/capability boundaries carried into Episode 32.

Guardrail:
This episode must distinguish between:
1. external AIAG/VDA requirements/methodology;
2. automotive-specific applicability;
3. our general hardware risk-to-control synthesis.

Do not imply that every startup or every industry is contractually required to use automotive core tools.

## 7. Listener tool — Risk-to-Control Chain
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

## 8. Quality Gate Design Check
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

## 9. Sentinel Node worked example
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

## 10. Applicability statement
This episode teaches a general risk-to-control engineering chain using DFMEA/PFMEA/Control Plan concepts. Automotive AIAG/VDA manuals will be treated as authoritative only for claims within their documented scope/methodology. Other industries may use different mandated risk and quality planning methods. The listener framework is repository synthesis and must not be presented as a universal standard requirement.

## 11. What this episode must NOT claim
- every company must use AIAG/VDA FMEA;
- an RPN threshold universally determines action;
- completing PFMEA proves a process is controlled;
- final inspection can replace process control;
- 100% inspection is always superior;
- every dimension is a CTQ;
- measurement data are trustworthy without considering measurement-system adequacy;
- a Control Plan remains valid after relevant design/process/supplier changes without impact review.

## 12. Common failure modes
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

## 13. Quantitative / scoring guardrail
This episode should explain FMEA prioritization conceptually but avoid teaching numeric scoring tables or action thresholds until the exact applicable handbook edition is verified.

If RPN versus Action Priority is discussed:
- state handbook/edition;
- show the methodological distinction accurately;
- do not create universal numeric action thresholds;
- clearly separate historical/legacy practice from current guidance.

## 14. Research backlog before CLAIM SET STABLE
1. Obtain/verify current AIAG-VDA FMEA source and exact terminology.
2. Obtain/verify current AIAG Control Plan source and exact required fields/concepts.
3. Map which statements are automotive-specific versus transferable engineering principles.
4. Verify prevention/detection/reaction language.
5. Decide scope of RPN/AP discussion after source review.
6. Cross-check P2.03 Quality Chain, Episode 24 and Episode 32 boundaries.
7. Technical review: quality + manufacturing/NPI.

## 15. Pilot-test objective
Episode 23 tests the Episode Packaging Contract under a standards/manual-heavy practitioner topic.

Pilot PASS signal:
A listener should be able to take one meaningful failure mode and build a coherent chain from requirement/risk → process cause → prevention → detection → measurement → reaction → effectiveness evidence, while understanding which parts are AIAG/VDA methodology and which parts are general synthesis.

## 16. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: HIGH
Quantitative burden: MEDIUM
Backbone risk: MEDIUM — terminology/applicability discipline required
Source verification: OPEN

Next status target:
`RESEARCH PACK OPEN → CLAIM SET STABLE`
