# 3.6.7 Electrical Discharge Machining (EDM)

status: Researching
provenance: [GNR]

## Scope
- Wire EDM
- Sinker EDM
- EDM drilling / small-hole EDM

## Definition
EDM removes electrically conductive material by controlled electrical discharges between tool/electrode and workpiece in a dielectric medium.

## Engineering meaning
EDM enables geometry and hard-material machining that may be difficult or impractical with conventional cutting, but introduces its own surface-integrity, electrode/wire, flushing, access and cycle-time constraints.

## DFM questions
- Is the material electrically conductive?
- Is the feature inaccessible to conventional rotating tools?
- Does a sharp internal corner or hardened feature justify EDM?
- Is through-access available for wire EDM?
- Can the required surface integrity tolerate/requires control of recast/altered layer?
- Is a dedicated electrode economical for sinker EDM?

## Wire EDM objects
- start hole
- wire path
- taper cutting
- slug retention
- flushing
- multi-pass skim cuts
- wire break

## Sinker EDM objects
- electrode design
- electrode wear
- orbiting
- flushing
- rough/finish burns
- electrode manufacturing

## Failure / limitation objects
- recast layer
- thermal microcracking
- dimensional overcut
- taper
- wire breakage
- poor flushing
- electrode wear
- long cycle time

## Decision links
- EDM vs milling
- EDM vs grinding
- Wire vs sinker EDM
- machine before vs after heat treatment

## Evidence backlog
Standards, surface integrity studies, electrode/wire wear research, production economics and case studies.