# 3.8.5 Continuous & Automated Composite Processes

status: Researching
provenance: [GNR]

## Process families
- filament winding
- pultrusion
- automated tape laying (ATL)
- automated fiber placement (AFP)
- automated cutting/kitting
- robotic layup / handling

## Filament winding objects
- mandrel
- winding angle
- tow/band tension
- payout eye
- resin bath/prepreg tow
- geodesic/non-geodesic path
- cure
- mandrel removal

## Pultrusion objects
- reinforcement feed
- resin impregnation
- preforming
- heated die
- pulling system
- cut-off
- constant profile

## ATL/AFP objects
- tow/tape placement
- compaction
- heating
- course planning
- steering
- gaps/overlaps
- tow drops
- inspection

## DFM questions
- Is geometry compatible with continuous reinforcement placement?
- Can winding/placement angles satisfy both structural and manufacturing constraints?
- Is a constant cross-section suitable for pultrusion?
- Does volume/part family justify automation investment?
- Which defects can be detected during automated placement rather than after cure?

## Failure modes
- tow gaps/overlaps
- wrinkles
- bridging
- tension variation
- fiber misalignment
- resin variation
- placement defects
- die/mandrel related dimensional error

## Decisions
### D-COMP-WIND-001 — Filament winding vs alternative hollow-structure route
### D-COMP-PULT-001 — Pultrusion vs extrusion/metal profile/fabrication
### D-COMP-AUTO-001 — Manual layup vs ATL/AFP

## Cross-domain links
Filament winding <-> pressure vessels
Pultrusion <-> continuous profiles
AFP/ATL <-> automation
In-process inspection <-> machine vision/NDT
Toolpath planning <-> CAD/CAM

No universal volume threshold for automation is asserted.