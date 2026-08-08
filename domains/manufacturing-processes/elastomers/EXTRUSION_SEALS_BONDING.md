# 3.9.3 Extrusion, Seals & Bonding

status: Researching
provenance: [GNR]

## Elastomer extrusion
Objects:
- profile extrusion
- hose/tube extrusion
- die swell
- drawdown
- dimensional control
- continuous cure/vulcanization
- cooling
- cut-to-length
- splicing/joining

Failure modes:
- profile distortion
- dimensional drift
- surface defects
- porosity
- under/over cure
- splice weakness

## Seals and O-rings
Objects:
- O-ring
- gasket
- lip seal
- static seal
- dynamic seal
- groove/gland
- squeeze
- stretch
- compression set
- extrusion gap
- surface finish
- lubrication

Engineering rule: seal performance must be linked to geometry, compound, surface, pressure, motion, temperature, media and aging; no seal design value is universalized without context.

## Rubber-to-metal / substrate bonding
Objects:
- insert preparation
- primer/adhesive system
- overmolding
- chemical bonding
- mechanical interlock
- contamination control
- bond verification

## DFM questions
- Is a standard seal preferable to a custom molded geometry?
- Can the groove and surface finish be manufactured and inspected repeatably?
- Is extrusion appropriate for the profile and volume?
- Does bonded insert geometry support load transfer and process repeatability?
- Is the prototype using the final compound/cure/bond system?

## Decisions
### D-SEAL-001 — Standard seal or custom molded seal?
### D-ELAST-EXT-001 — Extruded profile or molded part?
### D-ELAST-BOND-001 — Chemical bond, mechanical retention or hybrid?

## Cross-links
Seals <-> surface texture/GD&T
Seals <-> chemical compatibility
Bonding <-> adhesive joining
Extrusion <-> continuous manufacturing
Compression set <-> reliability/aging

All design thresholds remain evidence backlog content.