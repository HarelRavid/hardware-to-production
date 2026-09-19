# EP12 Source Notes V1 — Polymer Parts: Injection Molding and the Alternatives

status: SOURCE NOTES COMPLETE — READY FOR WAVE 06B PUBLICATION GATE
checked: 2026-09-19
script: EP12_SCRIPT_DRAFT_V1.md
script_review: EP12_SCRIPT_REVIEW_V1.md
source_lock: evidence/source-lock/SOURCE_LOCK_WAVE_06B_POLYMERS_REGISTER.md

## Primary standards/current-status sources

### EP12-S01 — ISO 20457:2026
Plastics moulded parts — Tolerances and acceptance conditions
Edition 2, published 2026-08.
Official:
https://www.iso.org/standard/20457.html

Use:
plastics-specific dimensional/geometrical tolerance and manufacturability context.
Current-status note:
replaces ISO 20457:2018.

Boundary:
sink marks/joint lines are outside its stated scope.

### EP12-S02 — ISO 294-1:2017
https://www.iso.org/standard/67036.html

Use:
injection-moulding test-specimen preparation requires controlled mould/process conditions; exact conditions are material dependent.

Boundary:
not treated as a production-part DFM standard.

### EP12-S03 — ISO 294-4:2018
https://www.iso.org/standard/70413.html

Use:
moulding shrinkage and post-moulding shrinkage; parallel/normal-to-flow distinction.

### EP12-S04 — ISO 62:2008
https://www.iso.org/standard/41672.html

Use:
water/moisture-absorption test context.

## Grade-specific material examples

### EP12-S05 — BASF Ultramid B3WG7
https://plastics-rubber.basf.com/global/en/performance_polymers/products/ultramid/30055646

Use:
illustrates exact-grade directional shrinkage and dry/conditioned property differences.

Boundary:
values are not generalized.

### EP12-S06 — BASF Ultramid Advanced/PPA
https://plastics-rubber.basf.com/emea/en/performance_polymers/fpgs/polyphthalamides

Use:
illustrates grade/family-specific moisture and dimensional behaviour.

## Technical process guidance

### EP12-S07 — Autodesk Moldflow warpage
Use:
differential cooling, shrinkage and orientation mechanisms.

### EP12-S08 — Autodesk Moldflow sink marks / voids
Use:
local thick-section / packing / cooling mechanism.

### EP12-S09 — Autodesk Moldflow weld/meld lines
Use:
flow-front meeting and location/process/material consequence.

### EP12-S10 — Covestro gate design
Use:
gate/flow/packing/surface-quality coupling.

### EP12-S11 — DuPont polymer/mould-design training
Use:
mould design, runners, gates, cooling, ejection, shrinkage and injection-moulding fundamentals.

## Internal synthesis

The following are Hardware-to-Production frameworks:
- Polymer Route Review;
- Moldability / Bridge Review;
- process-family comparison map;
- prototype-to-production evidence backlog;
- bridge-process exit logic.

## Claim map

- exact grade/state → EP12-S03/S04/S05/S06.
- plastics-specific moulded tolerance → EP12-S01.
- directional shrinkage → EP12-S03/S05.
- warpage → EP12-S07.
- sink/void → EP12-S08.
- weld/meld line → EP12-S09.
- tooling/gating/process coupling → EP12-S02/S10/S11.
- prototype-route evidence transfer → Wave 01.
- bridge economics → Wave 06A + Wave 03.

## Quantitative declaration

No generic engineering numeric threshold is used.

Any numbers in BASF or supplier materials remain source-specific and show-notes-only unless deliberately introduced with exact applicability.

## Publication re-check

Before final recording/publication:
1. confirm ISO 20457:2026 remains current;
2. confirm no late edit adds universal wall/draft/rib/shrinkage/drying/tolerance values;
3. confirm any material example names exact grade/state;
4. if a process-specific customer requirement is added, source it separately.

## Gate

Current generic script source blockers: NONE.

**EP12 SOURCE NOTES V1: COMPLETE**
