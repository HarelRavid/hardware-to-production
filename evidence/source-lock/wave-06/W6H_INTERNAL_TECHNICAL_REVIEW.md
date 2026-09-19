# Wave 06H Internal Technical Review — EP18 Surface / Cleaning / Heat Treatment

status: PASS TO FINAL SCRIPT OUTLINE
review_date: 2026-09-19
review_type: internal technical / standards-scope / process-sequence review
human_independent_review: NOT CLAIMED

inputs:
- SOURCE_LOCK_WAVE_06H_SURFACE_CLEANING_HEAT_TREATMENT_REGISTER.md
- W6H_EP18_CLAIM_LOCK.md
- EP18 Production Blueprint
- surface-engineering / clean-manufacturing / heat-treatment domain objects
- EP14 Joining
- Waves 01/02/03

## 1. Decision

EP18 can advance to final Claude-handoff outline.

The episode must teach **state transformation and sequence compatibility**, not coating catalogues, cleanliness recipes or heat-treatment recipes.

## 2. Cleaning

PASS.

Teach:
cleanliness requirement follows contaminant/failure mechanism, location and verification method.

Guard:
- no “looks clean” acceptance;
- no universal particle/residue/ionic limit;
- ISO 14644-9 is controlled-environment particle-cleanliness context only.

## 3. Surface preparation and coating

PASS.

Teach:
substrate preparation + process + masking/racking + coating state + measurement + downstream compatibility form one system.

Guard:
- ISO 8501 examples are steel/paint context;
- no coating-thickness target;
- coating-thickness method depends on substrate/coating system;
- no coating name alone proves corrosion/service performance.

## 4. Corrosion/environment testing

PASS.

ASTM D1654 provides scoped comparative corrosion/coating evaluation context.

Guard:
test duration/result is not direct field-life prediction.

## 5. Heat treatment

PASS.

AMS2750H is current pyrometry context for metallic thermal processing.

Teach:
thermal-processing evidence may depend on instrumentation/equipment/load state.

Guard:
- AMS2750H is not universal;
- no TUS/SAT/furnace-class intervals/tolerances;
- no alloy/time/temperature recipe;
- hardness alone is not complete metallurgical proof.

## 6. Dimensional/material-state impact

PASS.

NIST residual-stress/distortion evidence supports the mechanism that prior thermal/mechanical state can affect later dimensional outcome.

## 7. Sequence interaction

STRONG PASS.

Use examples:
- clean before bonding;
- prepare before coating;
- mask functional surfaces;
- heat treat before/after finish machining depending route;
- inspect after the final state-changing step relevant to the claim;
- stripping/recoat/reheat can change the evidence state.

EP19 owns the full-chain framework.

## 8. Rework

PASS.

State-changing rework adds history and can affect prior evidence.
Do not assume “restore to original.”

## 9. Current-status watch

Checked 2026-09-19:
- ISO 14644-9:2022 current.
- ISO 8501-1:2007 current; revision active.
- ISO 8501-4:2020 current/confirmed 2026.
- ISO 2178:2016 current/confirmed 2026.
- ISO 2360:2017 current.
- ISO 4518:2021 current.
- ASTM E376-26 active.
- ASTM D1654-24e1 active.
- SAE AMS2750H current, July 2024.

## 10. Audio-density rule

Spoken audio:
state → mechanism → side effect → verification → next operation.

Move detailed process taxonomy and standards metadata to companion visual/show notes.

## 11. Dialogue opportunity

Speaker B:
“If the part passed dimensional inspection before coating, why isn’t that enough?”

Speaker A:
“Because the released product is the state after the final transformation that affects the claim.”

## Decision

**WAVE 06H EP18 TECHNICAL REVIEW: PASS TO FINAL SCRIPT OUTLINE**
