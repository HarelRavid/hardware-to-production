# 3.11.7 Additive Economics & AM-vs-Conventional Decision

status: Researching
provenance: [GNR]

## Cost architecture
Cost per good part may include:
- feedstock
- build preparation/programming
- machine/build time
- build-volume utilization
- supports/sacrificial material
- failed-build risk
- depowdering/washing/cleaning
- support removal
- heat treatment/HIP/debind/sinter
- machining/finishing
- inspection/NDT
- qualification/coupons
- labor/handling
- machine depreciation/service
- powder/material recovery losses
- scrap/rework

## Value objects beyond piece price
- tooling avoidance
- lead-time reduction
- part consolidation
- mass/performance improvement
- internal geometry
- inventory/on-demand production
- design iteration
- repair/remanufacture boundary

## Decision object
### D-AM-NOT-001 — When should we NOT use additive manufacturing?
Warning conditions to evaluate, not automatic exclusions:
- simple geometry efficiently produced conventionally
- high stable volume with mature tooling route
- demanding surface/tolerance dominated by extensive post-machining
- inaccessible supports/feedstock/residue
- critical internal geometry that cannot be verified
- material/process qualification burden exceeds created value
- build size/utilization makes economics poor
- anisotropy/thermal distortion conflicts with requirements
- conventional process provides superior material state or supply-chain maturity

## Master comparison
AM candidates must be compared with machining, casting, forging, sheet fabrication, molding, extrusion, powder routes and hybrid manufacturing where technically relevant.

## Lifecycle economics
Decision should consider NRE/tooling + piece cost + lead time + quality/yield + inspection + inventory + service/repair + design-change cost, not printer hourly rate alone.

No universal break-even volume is asserted.