# 3.10.4 Furnace, Atmosphere, Setters & Dimensional Control

status: Researching
provenance: [GNR]

## Furnace objects
- chamber furnace
- tube furnace
- continuous furnace
- vacuum furnace
- controlled-atmosphere furnace
- hot press / HIP boundary
- thermocouple placement
- controller vs load temperature
- thermal uniformity
- gas flow/exchange
- furnace calibration/qualification

## Atmosphere objects
- air/oxidizing
- inert
- reducing
- vacuum
- reactive atmosphere
- dew point / oxygen potential where applicable
- purge strategy

## Setter/fixture objects
- setter plate
- support geometry
- contact area
- coating/release layer
- sag support
- stack height
- loading density
- thermal mass
- interaction/reaction with part

## Dimensional-control objects
- sintering allowance
- shrinkage map
- directional shrinkage
- warpage compensation
- fixture constraint
- free sintering
- creep/slump at temperature
- batch position effect

## Questions
1. Is controller SV representative of actual part/load temperature?
2. Which load positions see different thermal or atmosphere histories?
3. Does fixture/support geometry create local distortion or reactions?
4. Can a scale factor be used, or is feature/direction-specific compensation required?
5. How should furnace-load configuration be frozen/qualified for serial production?

## Decisions
### D-CER-FURN-001 — Furnace/atmosphere route
### D-CER-SET-001 — Free sinter vs setter/support strategy
### D-CER-SHRINK-001 — Global scale factor vs feature-specific compensation model

## Cross-links
Furnace uniformity <-> process capability
Setter design <-> warpage
Atmosphere <-> chemistry
Load mass <-> thermal response
Shrinkage model <-> tooling/CAD compensation

No furnace ramp/temperature or shrinkage factor is universalized.