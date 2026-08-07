---
id: H2P-PW-180
title: Polymer AM Environmental Compatibility
object_type: Method
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
---

# Polymer AM Environmental Compatibility

## Definition
Assessment of whether a printed polymer prototype remains meaningful under expected temperature, UV/light, humidity, chemical, wear and time-dependent exposure.

## Core principle
A prototype may pass geometry and fit checks while being invalid for service-condition evaluation if its printed material does not reproduce the relevant environmental behavior.

## Assessment dimensions
- Heat / HDT / continuous exposure
- Thermal cycling
- UV / sunlight
- Water / humidity
- Chemical splash or immersion
- Fuels / oils / cleaners where applicable
- Creep under sustained load
- Wear / friction
- Sterilization or cleaning exposure
- Aging duration

## Examples
Commercial PA12 SLS guidance highlights relatively low moisture uptake and good light, heat and chemical resistance compared with many common nylons. By contrast, SLA resin families can have very different thermal and aging behavior and must be assessed by formulation and cure state.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| DEPENDS_ON | H2P-PW-176 FDM / FFF Material Selection | Strong | High | Environmental behavior is material-family dependent | TDS/literature |
| DEPENDS_ON | H2P-PW-177 SLA Resin Family Selection | Strong | High | Resin chemistry/cure controls performance | TDS |
| DEPENDS_ON | H2P-PW-178 Polymer PBF Material Selection | Strong | High | Powder family controls environment capability | TDS |
| SUPPORTS | H2P-PW-174 Prototype Production Representativeness | Strong | High | Service-condition fidelity is part of representativeness | Project model |

## Open gaps
Build condition-specific compatibility matrices from primary polymer data and standardized testing, not crowd-sourced compatibility charts.