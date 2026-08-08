# 3.7.9 Polymer Extrusion

status: Researching
provenance: [GNR]

## 3.7.9.1 Process Families
- Profile extrusion
- Sheet extrusion
- Film extrusion
- Tube / pipe extrusion
- Co-extrusion
- Crosshead extrusion

## 3.7.9.2 Core Objects
- Hopper / feeding
- Screw
- Barrel
- Melt zone
- Screen pack / breaker plate
- Die
- Calibrator
- Cooling
- Haul-off
- Cut-to-length / winding
- Downstream sizing

## 3.7.9.3 DFM Principles
Extrusion is fundamentally suited to products whose geometry is generated continuously along a primary axis. DFM therefore focuses on cross-section geometry, wall balance, melt flow, die design, cooling, puller stability and downstream operations.

Key design questions:
- Can the geometry be represented as a constant or intentionally varying continuous cross-section?
- Are wall thicknesses and flow paths balanced enough to avoid distortion or differential cooling?
- Can assembly features be created inline, post-machined, punched, welded or added as separate components?
- Is a standard extrusion profile sufficient instead of a custom die?

## 3.7.9.4 Failure / Variation Objects
- Melt fracture
- Die swell
- Draw-down variation
- Warpage / bow
- Twist
- Thickness variation
- Surface lines
- Gel / contamination defects
- Dimensional drift
- Inadequate cooling

## 3.7.9.5 Economics
Primary drivers:
- custom die/tooling
- line speed
- material throughput
- scrap during startup/changeover
- secondary operations
- inline automation
- profile complexity
- dimensional inspection

## 3.7.9.6 Decision Objects
### D-POLY-EXT-001 — Custom extrusion or standard profile?
### D-POLY-EXT-002 — Extrude or machine the section?
### D-POLY-EXT-003 — Inline feature or secondary operation?

## 3.7.9.7 Why Projects Fail
- designing a profile that forces difficult die balancing for negligible product benefit
- ignoring downstream cooling and puller effects
- specifying tolerances without understanding line capability
- treating secondary punching/machining as an afterthought
- assuming prototype-machined material reproduces extrusion-induced orientation and residual stress

## 3.7.9.8 Evidence Backlog
Populate process windows, allowable section ratios and material-specific limits only from resin processor guides, extrusion handbooks and validated sources.