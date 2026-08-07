---
id: H2P-PW-176
title: FDM / FFF Material Selection
object_type: Method
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [POC, Prototype, Engineering Prototype, EVT]
status: Researching
---

# FDM / FFF Material Selection

## 1. Definition
A structured method for selecting material-extrusion feedstock based on the prototype purpose and required mechanical, thermal, environmental, manufacturing, and economic behavior.

## 2. Core principle
Do not select filament by nominal polymer name alone. Printed-part behavior depends on polymer formulation, reinforcement, moisture condition, process parameters, build orientation, geometry and machine condition.

ISO/ASTM 52903-1:2020 provides a framework for defining feedstock requirements for unfilled, filled and reinforced plastics used in material-extrusion AM.

## 3. Selection dimensions
- Required stiffness and strength
- Ductility / impact resistance
- Temperature exposure and HDT
- UV / outdoor exposure
- Chemical exposure
- Moisture sensitivity
- Dimensional stability and warpage risk
- Creep / sustained loading
- Surface / appearance needs
- Support strategy and soluble-support compatibility
- Reinforcement need (CF/GF)
- Nozzle wear and machine capability
- Cost and material availability

## 4. Material-family guidance
### PLA / Tough PLA
Best for fast concept and form-fit prototypes where printability and speed dominate. Limited for elevated temperature or long-term functional service.

### PETG
General-purpose functional prototyping with better toughness and heat resistance than basic PLA in many commercial systems.

### ABS
Useful for functional prototypes requiring higher heat resistance and toughness than PLA, but more sensitive to warpage and enclosure/process control.

### ASA
Strong candidate for outdoor/UV-exposed prototypes and housings; generally used when ABS-like behavior plus better weathering resistance is needed.

### PA / Nylon
Useful for mechanically functional parts requiring toughness, fatigue resistance and lower friction, but moisture management becomes important.

### TPU/TPE
Used for flexible, compliant or impact-damping prototypes; printability, dimensional control and fine-feature performance are usually more difficult than rigid materials.

### CF/GF-reinforced materials
Increase stiffness and can improve dimensional stability, but reduce ductility, increase abrasiveness and require process/machine compatibility.

## 5. Example manufacturer evidence
Ultimaker currently lists representative properties including PETG tensile strength 50 MPa / HDT 70 °C, ABS 43 MPa / HDT 84 °C, ASA 49 MPa / HDT 96 °C and Nylon 66 MPa / HDT 91 °C for its Method-series materials. These values are machine/material-system specific and must not be generalized to all printed parts.

## 6. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| APPLIES_TO | H2P-PW-021 FDM / FFF Printing | Mandatory | High | Material selection is integral to FDM capability | ISO/ASTM 52903-1 |
| DEPENDS_ON | H2P-PW-003 Prototype Purpose Classification | Strong | High | Material choice must follow what the prototype must prove | Prototyping literature |
| DEPENDS_ON | H2P-PW-174 Prototype Production Representativeness | Strong | High | Material may need to represent final product behavior | Project method |
| INTERACTS_WITH | H2P-PW-033 Additive Orientation Strategy | Strong | High | Material data cannot be separated from orientation | AM literature |

## 7. Open gaps
Build manufacturer-independent comparison tables only after collecting test-condition-normalized datasets. Add moisture, UV and chemical-compatibility evidence by polymer family.