---
id: H2P-PW-178
title: Polymer PBF Material Selection
object_type: Method
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
---

# Polymer PBF Material Selection

## Definition
Selection method for SLS/MJF polymer powders based on required strength, ductility, thermal stability, dimensional behavior, surface, environmental stability and reuse economics.

## Core principle
Powder-bed fusion polymer choice must be treated as a material/process-system decision. Polymer family, powder aging/refresh rate, process parameter set and orientation can materially change properties.

## Main families
### PA12
General-purpose functional prototype and low-volume production material. Current SLS data from Formlabs Nylon 12 reports UTS 50 MPa, tensile modulus 1.85 GPa, elongation X/Y 11% and Z 6%, HDT 87 °C @1.8 MPa. EOS PA2200 data also demonstrates orientation-dependent ductility and process-parameter dependence.

### PA12 Tough / ductile variants
Useful where snap fits, hinges, impact and compliance dominate. Example commercial data shows much higher elongation than standard PA12 but lower stiffness/thermal performance in some conditions.

### PA11
Typically selected when higher ductility/impact behavior is required, subject to system-specific data and powder handling requirements.

### PA12 GF
Used for greater stiffness and thermal/dimensional stability. Example SLS data reports modulus around 2.8 GPa and HDT 113 °C @1.8 MPa but much lower elongation than unfilled PA12.

### TPU
Used for elastomeric/compliant components; dimensional accuracy and surface/fine feature performance must be considered separately.

## Selection criteria
- Static and impact load
- Flexibility / snap-fit behavior
- Temperature
- Warpage / large-section geometry
- Environmental stability
- Detail / surface
- Powder refresh rate and cost
- Atmosphere requirements
- Post-processing requirements
- Production representativeness

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| APPLIES_TO | H2P-PW-024 SLS Polymer Printing | Mandatory | High | Powder selection defines process capability | ISO 52911-2 + TDS |
| APPLIES_TO | H2P-PW-025 MJF Printing | Strong | Medium | Similar powder-family decision logic; system data differs | Manufacturer data |
| DEPENDS_ON | H2P-PW-174 Prototype Production Representativeness | Strong | High | Material selection determines functional relevance | Project method |
| INTERACTS_WITH | H2P-PW-033 Additive Orientation Strategy | Strong | High | Direction-specific data exists even in PBF | EOS/Formlabs data |

## Open gaps
Add current HP MJF PA12/PA11/TPU data and independent SLS-vs-MJF comparisons under matched test conditions.