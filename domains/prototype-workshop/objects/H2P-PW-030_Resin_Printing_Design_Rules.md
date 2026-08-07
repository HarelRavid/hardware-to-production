---
id: H2P-PW-030
title: Resin Printing Design Rules
object_type: Method
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [POC, Prototype, Engineering Prototype, EVT]
status: Researching
---

# Resin Printing Design Rules

## Scope
Process-design rules for vat-photopolymerization prototypes including SLA/MSLA/DLP-class processes. Exact capability depends on machine, resin, orientation, support layout, wash and post-cure state.

## Key Rule Categories
- supported vs unsupported wall thickness
- minimum holes and drain holes
- support contact placement
- enclosed resin escape
- cosmetic surface orientation
- mating clearances
- post-cure dimensional change
- brittle vs tough resin geometry

## Example Published Service-Bureau Values
These values are illustrative and must remain tied to the cited service context, not treated as universal SLA limits.

- Minimum rigid-resin wall: 0.5 mm
- Minimum flexible-resin wall: 1.0 mm
- Minimum feature size: 0.2 mm
- Minimum hole diameter: 0.75 mm
- Drain holes: 3.5 mm minimum on hollow sections; two holes recommended for drainage/venting
- Mating-part clearance: around 0.2 mm for assembled parts; tighter press fits require calibration

Source: Simple Machining SLA Design Guidelines.

## Engineering Interpretation
1. Support contact points can damage cosmetic or sealing surfaces; orient them away from critical interfaces.
2. Hollow parts need deliberate resin drainage and cleaning paths.
3. Post-cure is part of the process state and can materially change dimensions and mechanical properties.
4. Thin snap fits or living hinges require resin-family-specific validation; do not transfer rules from tough/ductile resins to high-temperature or rigid glass-filled resins.
5. Critical mating dimensions should be validated with process coupons or post-machined where necessary.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---:|---:|---|---|
| APPLIES_TO | H2P-PW-022 | Mandatory | High | Governs SLA geometry | process definition + industry guidance |
| APPLIES_TO | H2P-PW-023 | Mandatory | High | Also relevant to MSLA-class vat photopolymerization | process similarity |
| DEPENDS_ON | H2P-PW-177 | Strong | High | Resin family changes practical rules | material datasheets |
| DEPENDS_ON | H2P-PW-183 | Strong | High | Post-cure affects final state | manufacturer data |
| DEPENDS_ON | H2P-PW-032 | Strong | High | Support strategy affects surface and feasibility | industrial guidance |
| INFORMS | H2P-PW-173 | Strong | High | Feasibility and finish affect process selection | project synthesis |

## Evidence Note
Numeric design rules remain process/vendor specific until independently validated on the actual machine + resin + post-cure combination.
