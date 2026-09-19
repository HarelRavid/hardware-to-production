# EP23 Script Outline V1 — DFMEA, PFMEA, Control Plans and Quality Gates

status: SCRIPT OUTLINE COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
audience: NPI / manufacturing / quality; useful to design and supplier-quality teams
lifecycle: LVP → Production Validation → Ramp
source_lock: evidence/source-lock/wave-02/W2_EP23_EP24_EP32_EP39_EP40_CLAIM_LOCK.md
technical_review: evidence/source-lock/wave-02/W2_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-3/EP23_PRODUCTION_BLUEPRINT.md
entry: standalone with short CTQ/requirements recap

## Listener promise
By the end, the listener can take one meaningful production failure risk and convert it into prevention, detection, measurement and reaction logic instead of merely adding inspection.

## Cold open
[ILLUSTRATIVE]
A connector intermittently fails at final test. The team adds a second final inspection. Six weeks later the failure returns because connector side-loading during assembly was never controlled.

Question: Did we improve quality—or just improve our ability to notice the same problem late?

## Beat 1 — Product risk and process risk are not the same question
Tags: [SYNTHESIS] [PUBLIC METHOD CONTEXT]
Claims: EP23-C01
Sources: W2-S01/W2-S03
Guard: Do not teach the proprietary AIAG/VDA FMEA structure.
Narrative: design risk asks how product function can fail; process risk asks how manufacturing/assembly can create or fail to prevent the condition.
Transition: if process risk is real, it must change execution.

## Beat 2 — Risk analysis only matters when something changes
Tags: [SYNTHESIS]
Claims: EP23-C02, C04
Tool: Risk-to-Control Chain.
Use connector example:
function → failure effect → process step → mechanism → prevention → detection.
Guard: avoid universal prevention hierarchy language.
Key line: A score is not a control.

## Beat 3 — Prevention vs detection
Tags: [SYNTHESIS]
Claims: EP23-C04
Example:
- prevention: fixture geometry reduces angular insertion freedom;
- detection: defined seating check / controlled functional test.
Teach: detection may be necessary, but adding detection does not remove the mechanism.

## Beat 4 — Control Plan as execution layer
Tags: [AUTH-GUIDANCE] [SYNTHESIS]
Claims: EP23-C03
Sources: W2-S03
Narrative: AIAG's current standalone Control Plan is linked to product-quality/process planning.
Podcast use: translate selected risks into characteristic/control/method/frequency/reaction ownership.
Guard: no exact mandatory fields, phases or Safe Launch claims.

## Beat 5 — Measurement is part of the control
Tags: [AUTH-GUIDANCE]
Claims: EP23-C05
Sources: W2-S07/W2-S09
Narrative: a detection control is only as useful as the method used to make the decision.
Set up EP24: calibration sticker does not equal complete measurement-system adequacy.

## Beat 6 — Reaction plan and quality gate
Tags: [SYNTHESIS]
Claims: EP23-C07
Example abnormal connector seating signature:
stop/contain → identify affected WIP boundary → verify fixture/process state → disposition product → restore/verify process → feed learning back into risk/control records.
Guard: no universal sampling/frequency rule.

## Beat 7 — What not to do with RPN / Action Priority
Tags: [SYNTHESIS] [LICENSED-MANUAL-GATED]
Claims: EP23-C08
Narrative: do not let one score become the engineering conclusion.
Do not teach proprietary current method details.
Spoken line: Whatever scoring method your sector uses, the real question is whether the important risk changed the process.

## Listener tool execution
Use the connector failure through:
Requirement/function → failure effect → process step → cause/mechanism → prevention → detection/measurement → gate → reaction → effectiveness evidence.

## DEV / LVP / SVP
DEV: lightweight failure thinking; learn mechanisms.
LVP: formalize repeatable controls/reactions around real build learning.
SVP: sustain linkage as processes, tooling, suppliers and data change.

## Misconceptions to correct
- FMEA = spreadsheet.
- high score automatically dictates one action.
- final test = prevention.
- Control Plan duplicates PFMEA.
- every dimension needs equal control.
- audit completion proves risk is controlled.

## Closing action
Take the top recurring defect from the last build and build one complete Risk-to-Control Chain. If you cannot name prevention, detection and reaction, the process is not yet under explicit control.

## Handoff
EP24 asks whether the measurement/test method itself can be trusted enough to make that control decision.
