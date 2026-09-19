# Wave 06E Internal Technical Review — EP15 Composite Manufacturing

status: PASS TO FINAL SCRIPT OUTLINE
review_date: 2026-09-19
review_type: internal technical / source-boundary / aerospace-transfer review
human_independent_review: NOT CLAIMED

inputs:
- SOURCE_LOCK_WAVE_06E_COMPOSITES_REGISTER.md
- W6E_EP15_CLAIM_LOCK.md
- EP15 Production Blueprint
- composites domain map / quality gate
- Wave06A/06D
- Wave01/02/03

## 1. Decision

EP15 can advance to final Claude-handoff outline.

The episode must teach the manufacturing logic of polymer-matrix composites without becoming an aerospace design-allowables course.

## 2. Material definition

Result: PASS.

Core lesson:
reinforcement + matrix + architecture + process state.

Guard:
do not let “carbon fiber” stand as a complete material identity.

## 3. Layup / orientation / stacking

Result: PASS.

ASTM D3039 directly supports that material preparation, lay-up and stacking sequence affect measured response.

Guard:
- no generic laminate stacking rule;
- no quasi-isotropic recipe;
- no ply-angle allowable.

## 4. Cure / consolidation / storage

Result: PASS.

CMH-17 public scope strongly supports process variability, storage, construction, cure/consolidation, process control and material/process change.

Guard:
no universal prepreg storage/out-time/cure/autoclave settings.

## 5. Defects

Result: PASS as mechanism-level teaching.

Allowed:
voids/porosity, wrinkles, delamination, dry/resin-rich zones, misorientation, contamination.

Guard:
- no universal defect acceptance;
- no claim every listed defect applies equally to every composite route.

## 6. Coupon-to-part transfer

Result: STRONG PASS.

This is the episode's main evidence lesson.

Coupon property:
- is produced under a defined material/layup/specimen/conditioning/test state;
- does not automatically become a part-level allowable;
- transfers only where the relevant architecture/process/load/environment assumptions remain representative.

## 7. NDT / inspection

Result: PASS.

Guard:
no universal inspection method, detectability limit, POD or acceptance criterion.

Use only:
inspection must match defect/material/geometry/criticality.

## 8. FAA / CMH-17 applicability

FAA AC 20-107B:
active, but aviation only.

CMH-17:
authoritative composite handbook family, heavily structural/aerospace influenced.

Guard:
extract engineering mechanisms and evidence discipline; do not transfer certification burden to generic hardware.

## 9. Audio density

Composite physics is visually dense.

Spoken dialogue should focus on:
- what the material actually is;
- why process history matters;
- why coupons do not equal parts;
- what evidence must travel into production.

Move:
- bag-stack diagrams;
- ply architecture;
- defect illustrations;
- NDT visual details

to production notes/companion visuals.

## 10. Episode boundary

EP14:
joining-process depth.

EP15:
composite material/process architecture.

EP16:
powder/ceramic/green-body/sintering transformation.

EP18:
surface/thermal post-process depth.

EP19:
integrated process-chain sequencing.

Result:
PASS.

## 11. Claude dialogue opportunity

Speaker B:
“If the supplier uses the same carbon fiber and resin, why isn’t it the same part?”

Speaker A:
Because orientation, layup, cure/consolidation, defects, tooling and inspection can change the realized material state.

The dialogue should repeatedly test the shortcut:
“same material name = same engineering evidence.”

## Decision

**WAVE 06E EP15 TECHNICAL REVIEW: PASS TO FINAL SCRIPT OUTLINE**
