# 3.11.5 Orientation, Supports, Anisotropy & Defects

status: Researching
provenance: [GNR]

## Orientation decision dimensions
- load direction
- anisotropy
- support requirement
- thermal history
- residual stress/distortion
- surface quality
- dimensional accuracy
- build height/time
- packing/nesting
- post-machining access
- inspection/cleaning access

## Support objects
- structural support
- thermal support
- anchoring
- overhang support
- sacrificial interface
- support removal
- inaccessible support risk

## Defect families
- lack of fusion / incomplete bonding
- porosity/voids
- keyhole-type porosity boundary
- cracking
- delamination/layer separation
- warpage/curling
- recoater/spreading defects
- inclusions/contamination
- surface-connected defects
- trapped feedstock
- geometric nonconformance

## Engineering principle
Build orientation is a multi-objective manufacturing decision, not a cosmetic slicer setting.

## Decision objects
### D-AM-ORI-002 — Orientation optimization
Return candidate orientations with trade-offs rather than one universal optimum.

### D-AM-SUP-001 — Can support be eliminated, relocated or made removable?

### D-AM-DEF-001 — Which defects are critical for this application and how are they prevented/detected?

## Relationships
Orientation -> influences -> anisotropy
Orientation -> influences -> support
Orientation -> influences -> surface condition
Orientation -> influences -> distortion
Support -> influences -> post-processing
Thermal history -> influences -> residual stress
Defect detectability -> influences -> inspection architecture

All comparative claims remain GNR until process/material evidence is linked.