# EP26 Script Outline V1 — How to Plan a Pilot Build

status: SCRIPT OUTLINE COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
audience: NPI / manufacturing / quality / engineering leads
lifecycle: LVP → Production Validation
source_lock: evidence/source-lock/wave-03/W3_EP26_EP27_EP28_EP29_EP30_EP31_CLAIM_LOCK.md
technical_review: evidence/source-lock/wave-03/W3_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-3/EP26_PRODUCTION_BLUEPRINT.md

## Listener promise
Plan a pilot as an evidence-generating build with explicit decisions, configuration, data capture, intervention rules, stop logic and exit evidence.

## Cold open
[ILLUSTRATIVE] A team builds 25 units, ships most of them and celebrates. Later nobody knows which units were reworked, what changed mid-build or what the pilot actually proved.

## Beat 1 — Start with the decision after the pilot
Claims: EP26-C01
Tags: [AUTH-GUIDANCE] [SYNTHESIS]
Sources: W3-S02/W3-S03
Question: What decision will this pilot enable?
Guard: pilot quantity is not the objective.

## Beat 2 — Define the evidence envelope
Claims: EP26-C02
Tags: [AUTH-GUIDANCE] [SYNTHESIS]
Source: W3-S02
Map product revision, supplier/material, route, tooling, operators, WI, test/measurement and logistics.

## Beat 3 — Quantity has a rationale, not a magic number
Claims: EP26-C03
Tags: [SYNTHESIS]
Teach examples: enough units to expose an assembly interaction; enough lots/operators to test the intended question; no universal count.

## Beat 4 — Data plan before build
Capture first result, defect/rework, cycle time, interventions, shortages, measurement problems, supplier excursions and configuration identity.
Claims: EP26-C04/C05
Dependencies: Wave 01/02.

## Beat 5 — Allowed intervention and rescue
Engineering help may be appropriate, but every rescue changes what the pilot proves.
Guard: intervention is evidence, not automatic invalidation.

## Beat 6 — Stop / containment logic
Claims: EP26-C06
Risk-based stop conditions for repeated critical defects, unsafe state, measurement invalidity or configuration loss.
No universal numeric stop rule.

## Beat 7 — Daily learning loop
Review defect Pareto, rework, interventions, flow, shortages and changes by effectivity.

## Beat 8 — Exit decision
Claims: EP26-C07
Outputs: proceed to validation, repeat focused pilot, or carry explicit open gaps.

## Listener tool execution — Pilot Build Plan
Decision → objectives → configuration → quantity rationale → route/suppliers → CTQ/test → staffing → data → intervention rule → stop rule → change/effectivity → exit evidence → gaps.

## DEV / LVP / Production Validation
DEV: loose learning builds are fine if labeled.
LVP pilot: controlled identity and visible intervention.
Production validation: tighter representativeness and execution control.

## Misconceptions
- pilot = small production order;
- bigger sample automatically means better evidence;
- engineer rescue should be hidden from yield;
- every change invalidates the pilot;
- shipped pilot unit means learning is complete.

## Closing action
Write the post-pilot decision first. If the current build plan does not generate evidence for that decision, redesign the pilot before building.

## Handoff
EP27 asks what an integrated production-validation build must prove before ramp.