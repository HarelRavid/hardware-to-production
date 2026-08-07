---
id: H2P-PW-029
title: FDM Design Rules
object_type: Method
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [POC, Prototype, Engineering Prototype, EVT]
status: Researching
---

# FDM Design Rules

## Purpose
Provide process-specific starting rules for geometry intended for material-extrusion/FDM prototypes.

## Key Rule Categories
- wall thickness and unsupported features
- mating clearances
- holes and bores
- printed threads vs inserts
- support access
- orientation-sensitive strength and accuracy
- warpage and shrinkage allowance

## Provider-Specific Reference Values
These are **not universal process capability values**. They are examples published by one industrial FDM service provider and must remain tied to that provider/process context.

- General tolerance: ±0.3% with a minimum ±0.25 mm
- Minimum wall thickness: 1.0 mm
- Minimum unsupported wall thickness: 1.0 mm
- Minimum pin diameter: 3.0 mm
- Minimum moving-part clearance: 0.5 mm
- Minimum hole diameter: 0.5 mm
- Suggested hinge gap: 0.6 mm
- Large printed threads may be possible, but inserts are recommended for most repeated-use threaded joints

Source: Forge Labs FDM Design Guidelines.

## Engineering Interpretation
1. Treat these numbers as supplier capability guidance, not ISO limits.
2. Tight fits should be calibrated on the actual printer/material pair using test coupons.
3. Critical bores should usually be drilled, reamed, bored or otherwise post-machined when dimensional capability matters.
4. Horizontal and vertical holes may behave differently because of layer geometry and support conditions.
5. Threaded inserts or post-machined threads are generally more reliable than fine printed threads for repeated assembly.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---:|---:|---|---|
| APPLIES_TO | H2P-PW-021 | Mandatory | High | Rules govern FDM/FFF parts | ISO/ASTM 52903 family; industrial guidance |
| DEPENDS_ON | H2P-PW-033 | Strong | High | Orientation changes accuracy, support need and strength | academic/industrial evidence |
| DEPENDS_ON | H2P-PW-176 | Strong | High | Material changes shrinkage, ductility and process limits | material datasheets |
| RECOMMENDS | H2P-PW-182 | Strong | High | Inserts often outperform fine printed threads for repeated use | industrial guidance |
| INFORMS | H2P-PW-173 | Strong | High | Design-rule feasibility affects process selection | project synthesis |

## Evidence Notes
- ISO/ASTM 52903-1 and 52903-2 provide the material-extrusion feedstock and equipment framework.
- Numeric minimums above are provider-specific examples and require machine/material validation before being used as release criteria.
