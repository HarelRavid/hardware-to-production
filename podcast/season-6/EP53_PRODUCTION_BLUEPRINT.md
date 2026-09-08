# Episode 53 Production Blueprint — Hardware Launch Failures and What Was Missed

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
primary_audience: both — cross-functional technical leaders, founders, NPI/manufacturing/quality teams
lifecycle: CROSS-STAGE — DEV → LVP → SVP → FIELD
maps_to: MASTER_WBS 10.1 + cross-domain evidence/application
source_basis: `EP53_CASE_EVIDENCE_PACK.md`
entry_point: YES WITH COMPACT FRAMEWORK RECAP
technical_depth: practitioner

## Listener transformation
Before: treats launch failures as isolated stories of bad design, bad suppliers, bad operators or bad luck.
After: reconstructs a failure as a broken/unsupported evidence chain — identifying the claim, configuration/population, lifecycle stage, missing interaction, detection/escape path, corrective action and effectiveness evidence without overstating causation.

## Narrative hook
A replacement Galaxy Note7 — supplied as the corrective action for the first recall — is itself later included in an expanded recall. The opening question is not “how did Samsung miss a bad battery?” but:

> What evidence proves that a fix is actually a fix?

## Teaching flow
1. Five-minute Season 6 orientation: this season applies earlier frameworks; it does not create a new manufacturing theory.
2. Case reconstruction rule: FACT → SOURCE INTERPRETATION → OUR FRAMEWORK LESSON.
3. Note7: remedy population, field evidence and EFFECTIVENESS EVIDENCE.
4. Tesla Model 3 ramp: selected automation introduced faster than some processes matured; temporary manual/semi-automatic bridge; MOVING CONSTRAINT LOOP.
5. Boeing 737 MAX JATR: discrete-change evidence vs cumulative/system/human INTERACTION CLAIMS and inherited assumptions.
6. Peloton Tread+: FIELD EVENT → SIGNAL AGGREGATION → containment/escalation, with explicit legal-source wording discipline.
7. Compare four cases without forcing one universal root-cause template.
8. Close with the recurring operating rule: evidence supports a defined claim only inside a defined configuration/applicability envelope; change and field evidence can invalidate that trust.

## Core framework — CASE 12 reconstruction
Use the existing canonical case-analysis framework, editorially surfaced as:
`Case/configuration → claim believed → evidence available → evidence boundary → change/interaction → failure/event → detection/escape → affected population → containment → corrective action → effectiveness evidence → transferable lesson + limit`.

Do not invent an EP53-specific replacement framework.

## Case spine
### Case 1 — Samsung Galaxy Note7
Owns: corrective action / replacement population / effectiveness evidence.
Guardrail: Samsung technical root-cause conclusions remain attributed; CPSC recall facts remain regulator facts.

### Case 2 — Tesla Model 3 ramp
Owns: automation/process maturity, controlled bridge production, moving constraint.
Guardrail: Tesla SEC filing supports Tesla's account; do not conclude automation caused all ramp problems or that manual production is inherently superior.

### Case 3 — Boeing 737 MAX JATR
Owns: changed-product interaction, cumulative effects, assumption evidence.
Guardrail: aviation certification context and JATR scope must be explicit; do not claim the Changed Product Rule alone caused the accidents.

### Case 4 — Peloton Tread+
Owns: field signal aggregation and escalation/containment.
Guardrail: distinguish CPSC staff charges from Peloton admission/non-admission in the settlement record.

## Listener tool — Failure Reconstruction Sheet
For a real launch/ramp problem capture:
`Exact affected configuration/population → claim that failed → evidence originally supporting it → what changed/was outside scope → event/signal → how it escaped → containment → corrective action → what new evidence proves effectiveness → what remains uncertain`.

## DEV / LVP / SVP / FIELD
DEV: explicitly identify assumptions and interactions that a prototype has not proven.
LVP: treat every process/supplier/tool/change as an evidence-envelope transition; preserve enough genealogy to isolate learning.
SVP: maintain scalable signal aggregation, containment and corrective-action effectiveness across larger populations/suppliers.
FIELD: field events can invalidate product/process evidence; complaints/returns/recalls must feed back into configuration-specific engineering decisions.

## Prototype shortcut / expiration
Shortcut: narrow prototype evidence and expert judgment may be acceptable for learning.
Expires when: the same claim is used to release a larger population, changed configuration or production process without representative evidence.

## Common mistakes
- starting with “root cause” before reconstructing facts/configuration;
- treating passed tests/audits as unlimited evidence;
- assuming the corrective action is effective because it is technically plausible;
- counting complaints without population/configuration/time context;
- blaming one operator/supplier when the public record supports a system interaction;
- using hindsight to claim teams “should have known” facts that were not available at the time;
- generalizing an aviation/medical/consumer-product obligation outside its applicability.

## Source / script gates
Before script lock:
- verify every consequential date/population/quantity;
- retain exact JATR section/page locators for cited findings;
- re-check Tesla quantitative ramp values if narrated;
- preserve company-vs-regulator attribution in Note7/Tesla;
- conduct legal wording review for Peloton.

## Season handoff
EP53 teaches **how to read failure**. EP54 now asks the harder mirror question: when industrialization succeeds, which patterns are genuinely transferable and which are merely survivorship stories?
