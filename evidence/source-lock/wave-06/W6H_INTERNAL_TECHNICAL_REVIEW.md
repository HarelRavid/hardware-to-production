# Wave 06H Internal Technical Review — EP18 Surface Engineering, Cleaning and Heat Treatment

status: PASS TO FINAL SCRIPT OUTLINE
review_date: 2026-09-19
review_type: internal technical / process-state / revision-watch review
human_independent_review: NOT CLAIMED

inputs:
- SOURCE_LOCK_WAVE_06H_SURFACE_CLEANING_HEAT_TREAT_REGISTER.md
- W6H_EP18_CLAIM_LOCK.md
- EP18 Production Blueprint
- surface-engineering domain
- heat-treatment domain
- Wave06C/06D
- Wave01/02/03

## 1. Decision

EP18 can advance to final Claude-handoff outline.

The episode should teach state transformations and process-sequence compatibility, not coating catalogues or heat-treatment recipes.

## 2. Cleaning

PASS.

Core lesson:
“clean” must be tied to contamination/function/downstream process and verification.

Guard:
no universal cleanliness class or solvent/process recipe.

## 3. Surface preparation / coating system

PASS.

Use:
surface preparation + pretreatment + coating + cure/post-treatment + inspection as one system.

Guard:
no generic coating thickness or corrosion system.

## 4. Corrosion testing

PASS.

ISO 9227 is useful as method context.

Guard:
salt-spray hours are not direct field-life equivalence and the standard itself does not define universal exposure duration/result interpretation.

## 5. Heat treatment

PASS.

AMS2750H and CQI-9 support controlled thermal-processing evidence and pyrometry/system discipline.

Guard:
- aerospace/automotive applicability remains explicit;
- no TUS/SAT/furnace-class/recipe requirement is generalized.

## 6. Dimensional/material-state impact

PASS.

Teach:
heat treatment/coating can move dimensions/properties and affect later machining/tolerance/joining.

## 7. Rework / stripping / reheat

PASS as synthesis.

Core rule:
state-changing rework adds history and may affect prior evidence.

## 8. Sequence interaction

PASS.

EP18 should preview:
clean before bond;
heat-treat before/after machining;
mask before coating;
final dimension after state-changing process.

EP19 owns the full chain framework.

## 9. Revision watch

- CQI-9 4th Edition currently listed; new version anticipated Q4 2026.
- ISO 12944 family revisions underway.
- AMS2750H current.
- ISO 9227:2022 current.

## 10. Dialogue opportunity

Speaker B:
“If the part already passed machining inspection, why should coating or heat treatment force us to revisit dimensions?”

Speaker A:
Because the final product state exists after the state-changing operation, not before it.

## Decision

**WAVE 06H EP18 TECHNICAL REVIEW: PASS TO FINAL SCRIPT OUTLINE**
