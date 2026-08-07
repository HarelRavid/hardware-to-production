---
id: H2P-PW-194
title: SLA High-Temperature Resin
object_type: Material Family
parent_process: H2P-PW-022
status: Researching
lifecycle: [Prototype, Engineering Prototype]
tags: [SLA, high-temperature, engineering-resin, polymer-am]
---
# SLA High-Temperature Resin

## Definition
Photopolymer formulations optimized for elevated-temperature dimensional stability rather than high ductility or impact resistance.

## Engineering use
Useful for hot-air/fluid-path prototypes, thermally loaded mounts, rapid tooling and test fixtures where thermal response is the primary learning objective.

## Evidence-backed example
Formlabs High Temp Resin demonstrates why cure state must be part of the material definition: HDT at 0.45 MPa is reported as 49 °C in the green state, 120 °C after a 60 °C post-cure, and 238 °C after an extended high-temperature cure. Elongation at break simultaneously decreases from 14% green to 2.3% after the extended cure.

## Decision criteria
Use only when the required thermal condition and load level match the tested data. High HDT does not imply high toughness, long-term creep resistance, chemical compatibility or production-material representativeness.

## Relationships
| Type | Target | Strength | Reason |
|---|---|---|---|
| MATERIAL_FOR | H2P-PW-022 | Strong | SLA engineering-resin family. |
| SELECTED_BY | H2P-PW-177 | Strong | Resin family selection drives use. |
| REQUIRES | H2P-PW-183 | Mandatory | Cure schedule materially changes properties. |
| REQUIRES_CHECK_OF | H2P-PW-180 | Strong | Temperature and chemical environment require application-specific validation. |
| LIMITED_BY | H2P-PW-174 | Strong | Thermal performance alone does not establish production representativeness. |

## Podcast use
Prototype Shop — separating heat resistance from toughness and understanding cure-dependent SLA properties.
