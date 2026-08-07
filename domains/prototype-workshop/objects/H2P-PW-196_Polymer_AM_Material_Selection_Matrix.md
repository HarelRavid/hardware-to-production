---
id: H2P-PW-196
title: Polymer AM Material Selection Matrix
object_type: Decision Aid
status: Researching
lifecycle: [POC, Prototype, Engineering Prototype]
tags: [polymer-am, material-selection, decision-matrix]
---
# Polymer AM Material Selection Matrix

## Purpose
Provide a consistent first-pass material selection framework across FDM/FFF and SLA families before machine-specific quantitative validation.

## First-pass matrix
| Need | Likely starting point | Key caution |
|---|---|---|
| Fast low-cost geometry iteration | PLA / Tough PLA | Low heat capability; not a proxy for production thermoplastic behavior |
| Tough general functional FDM prototype | PETG | Verify Z-direction strength and chemical/thermal environment |
| Tougher/higher-temperature thermoplastic prototype | ABS | Warpage/process control; not outdoor-UV optimized |
| Outdoor/UV-exposed prototype | ASA | Verify exact formulation/weathering data |
| Wear/fatigue/low-friction thermoplastic prototype | Nylon family | Exact PA grade and moisture conditioning are mandatory |
| Flexible/compliant prototype | TPU family | Hardness/formulation and sealing behavior must be validated |
| Stiff fixture/tool | Reinforced FDM polymer | Stiffness gain may trade against toughness; abrasive feedstock |
| Smooth detailed rigid functional prototype | SLA engineering resin | Post-cure state is part of the material definition |
| Highly ductile/impact-tolerant SLA prototype | Tough resin family | Temperature/creep limits remain formulation-specific |
| High-temperature SLA prototype | High-temp resin | High HDT does not imply toughness |
| Low-friction/compliant SLA prototype | Durable/low-friction resin | Lower thermal capability than high-temp families |
| Functional nylon batch without support structures | SLS/MJF PA family | Specify exact PA11/PA12/filled grade and process system |

## Decision sequence
1. Define the engineering intent: geometry, load, heat, environment, friction/wear, flexibility, appearance or production representativeness.
2. Decide whether thermoplastic behavior itself is important. If yes, FDM/PBF or CNC may be more representative than generic SLA.
3. Decide whether the exact production material/process is required for the learning objective. If yes, escalate toward production-representative prototype routes.
4. Select material family.
5. Validate machine/process-specific dimensional and mechanical capability.
6. Record orientation, conditioning, post-processing and test method with all numeric data.

## Relationships
| Type | Target | Strength | Reason |
|---|---|---|---|
| USES | H2P-PW-176 | Strong | FDM material-selection framework |
| USES | H2P-PW-177 | Strong | SLA resin-family selection |
| USES | H2P-PW-178 | Strong | Polymer PBF material selection |
| SUPPORTS | H2P-PW-173 | Strong | Feeds the overall prototype manufacturing process decision |
| REQUIRES | H2P-PW-174 | Strong | Material choice must be checked against production representativeness |
| REQUIRES | H2P-PW-180 | Strong | Environmental compatibility must be verified |

## Status note
This matrix is intentionally qualitative. Numeric limits will be added only where source, material formulation, process, orientation, conditioning, post-processing and test method are traceable.
