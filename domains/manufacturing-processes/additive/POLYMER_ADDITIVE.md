# 3.11.2 Polymer Additive Manufacturing

status: Researching
provenance: [GNR]

## Process families
### Material extrusion
- FFF/FDM
- filament/pellet feed
- nozzle/extrusion temperature
- bed/chamber temperature
- raster/toolpath
- layer bonding
- support

### Vat photopolymerization
- SLA
- DLP
- resin
- exposure
- supports
- washing
- post-cure

### Powder-based polymer routes
- SLS
- MJF/process-boundary family
- powder spreading
- thermal control
- nesting
- depowdering

## Key engineering objects
- layer adhesion
- orientation-dependent properties
- warpage
- support marks
- stair stepping
- minimum feature
- trapped powder/resin
- moisture/feedstock conditioning
- post-cure
- surface finishing
- inserts/threads

## DFM questions
- Which surfaces should face/support/build direction?
- Can holes/threads be printed or should they be post-machined?
- Can support or powder/resin be removed from internal cavities?
- Are material properties representative of production conditioning and orientation?
- Is the polymer AM material suitable for service temperature, chemicals, creep, UV and aging?

## Decision objects
### D-AM-POLY-001 — FFF, vat photopolymerization, SLS/powder route or conventional polymer process?
### D-AM-POLY-002 — Print feature or machine/install it after build?
### D-AM-POLY-003 — Prototype-only material/process or production-intent route?

## Cross-links
Polymer AM <-> injection molding
Polymer AM <-> machining
Polymer AM <-> elastomer/TPE boundary
Post-cure <-> material properties
Orientation <-> anisotropy

No universal dimensional/material capability is asserted.