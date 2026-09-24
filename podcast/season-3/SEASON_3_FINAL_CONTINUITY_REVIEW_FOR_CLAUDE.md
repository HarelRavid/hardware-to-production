# Season 3 — Final Continuity Review for Claude Handoff

status: PASS — READY FOR HANDOFF MANIFEST / CLAUDE PROMPT GENERATION
review_date: 2026-09-19
scope: EP20–EP31
governed_by:
- podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md
- podcast/CLAUDE_EPISODE_HANDOFF_CONTRACT.md
- podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md

## 1. Decision

Season 3 remains structurally sound after completion of the missing Production System Engineering evidence family.

All 12 canonical episodes can move to Claude handoff-package generation.

No architecture redesign is required.

**SEASON 3 FINAL CONTINUITY REVIEW: PASS**

## 2. Final listener journey

EP20 — Product definition → manufacturing definition / routing
→ EP21 — Tooling / fixtures / equipment
→ EP22 — Standard work / operator qualification
→ EP23 — Risk-to-control / PFMEA / Control Plan / gates
→ EP24 — Production measurement / test adequacy
→ EP25 — Layout / material / operator / information flow
→ EP26 — Pilot build as learning experiment
→ EP27 — Production validation evidence
→ EP28 — Yield / rework / scrap learning
→ EP29 — Capacity / constraint / takt / flow
→ EP30 — Supplier / CM readiness
→ EP31 — Controlled engineering change during ramp

Result:
PASS — coherent progression from definition to execution, validation, ramp and controlled change.

## 3. Season-wide narrative rule

The season should feel like one operating system for production, not twelve disconnected manufacturing topics.

Canonical progression:

define work
→ create repeatable physical/human execution
→ connect risk and measurement
→ arrange the physical system
→ exercise it in pilot
→ validate it
→ learn from defects/rework
→ prove capacity
→ extend readiness to external sources
→ change it without losing evidence.

## 4. Episode ownership / anti-duplication

### EP20 — EBOM / MBOM / routing
Owns:
manufacturing execution definition.

Must not:
- become ERP/MES software tutorial;
- duplicate EP19 process-chain physics;
- imply one universal BOM/routing taxonomy.

### EP21 — Tooling / fixtures / equipment
Owns:
physical production-enabling tooling/equipment and evidence of validity.

Must not:
- become machine-safety standards episode;
- re-teach EP24 measurement-system depth;
- introduce generic fixture-tolerance ratios.

### EP22 — Standard work / operator qualification
Owns:
human execution definition and competence evidence.

Must not:
- become training-policy or HR episode;
- imply reading a WI equals competence;
- duplicate EP07 DFA/mistake prevention.

### EP23 — Risk-to-control chain
Owns:
translation of important process risks into prevention/detection/reaction logic.

Must not:
- teach proprietary AIAG/VDA FMEA method details;
- become generic FMEA score tutorial.

### EP24 — Measurement / production test
Owns:
whether the production decision system can be trusted.

Must not:
- teach one universal GR&R/MSA threshold;
- duplicate EP08 product testability architecture.

### EP25 — Layout / flow / ergonomics
Owns:
physical movement and abnormal flow through the cell.

Must not:
- become capacity episode;
- treat all WIP as waste;
- publish generic ergonomic dimensions/lift limits.

### EP26 — Pilot build planning
Owns:
learning-plan design.

Must not:
- turn pilot quantity into success criterion;
- pre-teach EP27 validation acceptance.

### EP27 — Production validation
Owns:
integrated production-system evidence.

Must not:
- treat PVT label as universal;
- duplicate EP29 capacity proof.

### EP28 — Yield / rework / learning
Owns:
hidden rescue, first-pass success, recurrence and process-learning history.

Must not:
- collapse into SPC/capability depth;
- treat final yield as the only quality metric.

### EP29 — Capacity / constraints
Owns:
demand pace, actual constraint, accepted throughput, queues and moving-constraint logic.

Must not:
- reduce system capacity to machine speed;
- re-teach OEE depth.

### EP30 — Supplier / CM readiness
Owns:
source-system readiness during ramp.

Must not:
- duplicate Season 4 sustained supplier-quality/resilience depth;
- equate sample approval with source readiness.

### EP31 — Engineering changes during ramp
Owns:
effectivity across live product/process/supplier/WIP populations.

Must not:
- duplicate A8 generic configuration-management foundation;
- imply every change requires full requalification.

Result:
PASS — no ownership conflict requiring restructuring.

## 5. Two-character strategy

Oz:
Lead Host / Systems Engineer.

Rona:
Practitioner / Challenger.

Recommended recurring challenges:

EP20:
“If engineering released the BOM, why can’t production just build it?”

EP21:
“If the fixture worked for ten units, why treat it like a controlled engineering asset?”

EP22:
“If the WI is correct, isn’t operator variation just a training issue?”

EP23:
“If we found the risk and added inspection, haven’t we controlled it?”

EP24:
“If the gauge is calibrated, why question the measurement?”

EP25:
“If machine capacity is enough, why should layout stop us?”

EP26:
“Why isn’t a bigger pilot automatically better evidence?”

EP27:
“If all product tests pass, how can production validation fail?”

EP28:
“If almost everything eventually passes, why obsess over first-pass yield?”

EP29:
“If each station is faster than takt, why are we missing demand?”

EP30:
“If the supplier made perfect samples, what else must be proven?”

EP31:
“If the ECO is released, isn’t the change done?”

Rona must remain technically competent and push on practical consequences.

## 6. Callback map

EP20:
callbacks A8 / EP19.

EP21:
callbacks EP09 / A4 / EP07.

EP22:
callbacks A5/A6/EP07.

EP23:
callbacks EP07 / EP20–22.

EP24:
callbacks EP08 / EP23.

EP25:
callbacks EP20 routing + EP29 capacity preview.

EP26:
uses EP20–25 system definition.

EP27:
uses EP26 pilot + EP23/24 controls.

EP28:
uses EP23/24/27 evidence history.

EP29:
uses EP28 rework burden + EP25 flow.

EP30:
uses EP29 capacity + supplier evidence from later locked packages as concise context.

EP31:
uses A8 effectivity + EP20 routing + EP30 suppliers.

No episode should re-teach the complete source episode.

## 7. Terminology lock

Use consistently:

- product definition
- manufacturing definition
- operation / routing / output state
- tooling/fixture evidence
- standard work
- operator qualification / demonstrated competence
- CTQ
- prevention / detection / reaction
- measurement adequacy
- WIP
- pilot
- production validation
- first-pass result / eventual accepted output
- accepted sustainable throughput
- constraint / moving constraint
- source readiness
- effectivity
- rework adds history

Do not introduce competing frameworks.

## 8. Standards / source strategy

Season 3 should not sound like an enterprise-standards course.

Use standards only where identity or applicability materially improves the engineering decision.

Specific controls:
- EP20: ISA-95 context only; no mandatory software architecture.
- EP21: machinery-safety/equipment qualification details remain application-specific.
- EP22: NASA/TWI context only; no generic legal competence requirement.
- EP23: AIAG/VDA details remain proprietary/manual-gated.
- EP24: MSA thresholds remain gated; NIST open sources carry generic measurement claims.
- EP25: NIOSH ergonomics is task-specific; no universal lift/layout numbers.
- EP26–31: customer-specific PVT/run-at-rate/change/supplier obligations remain scoped.

## 9. Quantitative continuity

EP20–27:
no engineering-significant universal threshold required.

EP28:
yield language must be defined in episode context.

EP29 approved illustrative arithmetic:
- 80 accepted units / 420 min → takt = 315 s/unit.
- 25,200 / 360 = 70 theoretical cycles.
- at 90% availability → 63 cycles.
- at 92% FPY → 57.96 first-pass accepted.
- first-order rework burden: 360 + 0.08×240 = 379.2 s.
- simplified queue example: arrivals ≈11.43/h; service ≈9/h; queue growth ≈2.43/h before rework.

These are illustrative, not universal capacity thresholds.

EP30–31:
no generic numeric supplier/change gate.

## 10. Visual companion strategy

Useful visuals:
- EP20 EBOM→MBOM/routing map.
- EP21 fixture datum/health diagram.
- EP22 standard-work decision points.
- EP23 risk-to-control chain.
- EP24 measurement-system chain.
- EP25 cell/material/WIP flow map.
- EP26 pilot evidence matrix.
- EP27 production-validation matrix.
- EP28 first-pass/rework history.
- EP29 capacity/constraint diagram.
- EP30 supplier-source system.
- EP31 effectivity timeline.

Claude may mark these as PRODUCTION NOTES — NOT SPOKEN.

## 11. Season pacing

EP20–25:
factory-definition/build-out tone.

EP26–31:
execution/learning/ramp tone.

Avoid checklist recitation.
Every episode should use one concrete production problem to drive the listener tool.

## 12. Source/evidence status

EP20/21/22/25:
Source Lock PASS.
Claim Lock PASS.
Technical Review PASS.
Final Script Outline complete.
Source-Notes Skeleton complete.

EP23/24/26–31:
existing publication packages PASS.
Existing full scripts remain reference inputs only.

## 13. Handoff-generation decision

Every Season 3 episode has sufficient:
- architecture;
- source/claim ownership;
- technical review;
- narrative outline;
- quantitative controls where needed;
- season boundary definition.

Next:
1. create 12 Episode Handoff Manifests;
2. create 12 Claude Writing Prompts;
3. run Season 3 Handoff Exit Audit;
4. mark Season 3 CLAUDE HANDOFF READY.
