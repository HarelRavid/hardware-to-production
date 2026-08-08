# 3.14.7 Property Verification, Traceability, Automation & Economics

status: Researching
provenance: [GNR]

## Verification objects
- hardness
- hardness traverse/profile
- tensile properties
- impact/toughness boundary
- metallography
- grain size boundary
- microstructure/phase condition
- case depth
- decarburization/oxidation
- dimensional inspection
- surface condition
- destructive coupon/witness sample
- functional test

## Genealogy model
Part/lot -> material heat/lot and incoming condition -> upstream forming/machining history -> furnace ID -> recipe revision -> load ID/location -> fixture/basket -> atmosphere/vacuum record -> temperature/process record -> quench/cooling record -> temper/age cycles -> inspection/test -> downstream operations.

## Automation/data objects
- recipe management
- furnace PLC/control
- historian/data logging
- automatic atmosphere control
- vacuum monitoring
- quench monitoring
- barcode/lot tracking
- alarm/interlock history
- calibration status
- automated hardness/dimensional inspection boundary

## Cost architecture
Cost per good part may include:
- furnace cycle energy/time
- atmosphere/vacuum gas/utilities
- load/fixture labor
- quench/cooling
- furnace occupancy/capacity
- inspection/coupons
- distortion-driven machining
- straightening/rework
- oxidation/scale removal
- scrap/cracking
- outsourced transport/lead time
- qualification/calibration/maintenance

## Decision objects
### D-HT-VER-001 — What proves the required material condition?
### D-HT-TRACE-001 — Required thermal-process genealogy
### D-HT-MAKEBUY-001 — In-house or qualified external heat treater?
### D-HT-ECON-001 — Optimize furnace utilization or dimensional/property yield?

## Principle
Hardness can be a useful process/property indicator but is not automatically a complete substitute for the required microstructure or mechanical-property evidence.