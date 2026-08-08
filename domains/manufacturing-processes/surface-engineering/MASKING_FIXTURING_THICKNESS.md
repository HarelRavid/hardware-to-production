# 3.12.5 Masking, Fixturing, Racking & Coating Thickness

status: Researching
provenance: [GNR]

## Objects
- masking
- rack / hanger
- electrical contact point
- fixture
- part orientation
- drainage
- air/gas entrapment
- shielding
- current-density distribution
- spray line-of-sight
- edge build
- recess coverage
- coating thickness
- local thickness variation
- dimensional allowance

## Engineering principle
Surface finishing is a geometry-changing manufacturing operation. Nominal coating thickness alone does not define the dimensional result because local deposition/coverage can vary with geometry, process physics, orientation, masking and fixture/contact strategy.

## DFM questions
1. Which surfaces must remain uncoated?
2. Where may rack/contact marks be located?
3. Can trapped solution, powder, paint or process media drain/escape?
4. Are deep recesses, internal passages and sharp edges compatible with the selected process?
5. Which dimensions are specified before finish and which after finish?
6. Do threads, bores, fits, sealing lands or electrical contacts require masking or post-finish machining?
7. Can the fixture hold the part without damaging cosmetic/functional surfaces?

## Decision objects
### D-SURF-MASK-001 — Mask or coat the feature?
Inputs: function, tolerance, corrosion requirement, electrical/thermal role, assembly, rework and cost.

### D-SURF-FIX-001 — Fixture/rack/contact strategy
Inputs: process, geometry, surface class, current/line-of-sight requirements, drainage, handling and automation.

### D-SURF-THK-001 — How is coating thickness represented in dimensional design?
Output must define pre-finish dimension, post-finish requirement, measurement location and tolerance-stack impact where applicable.

## Cross-links
Coating thickness <-> GD&T/tolerance stack
Masking <-> threads/fits/seals
Racking <-> cosmetic requirements
Fixture strategy <-> automation
Drainage <-> cleaning/contamination control

No universal thickness buildup factor is asserted.