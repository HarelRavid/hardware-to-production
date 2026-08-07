---
id: H2P-PW-181
title: Additive Support Strategy
object_type: Method
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [Prototype, Engineering Prototype, EVT]
status: Researching
---

# Additive Support Strategy

## Definition
Planning whether support structures are required, where they contact the part, how they affect geometry and surface, and how they will be removed without invalidating the prototype.

## Process differences
### FDM / FFF
Supports may be same-material breakaway, soluble, or machine-specific. They influence print time, material use, contact-surface finish, dimensional access and orientation choice.

### SLA / MSLA
Supports are commonly required to anchor and stabilize geometry during photopolymer printing. Contact-point placement affects surface and post-processing effort.

### SLS / MJF
The surrounding powder bed is self-supporting for most geometry, eliminating conventional attached support structures. This is a major geometric and nesting advantage, but trapped powder, escape access and thermal behavior remain design considerations.

## Decision criteria
- Unsupported span / angle
- Cosmetic and sealing surfaces
- Datum and tolerance surfaces
- Internal channels / powder evacuation
- Post-processing access
- Risk of deformation
- Build time / material penalty

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| INTERACTS_WITH | H2P-PW-033 Additive Orientation Strategy | Mandatory | High | Orientation and support design are coupled | Process physics |
| APPLIES_TO | H2P-PW-021 FDM / FFF Printing | Strong | High | Supports often required | Process guidance |
| APPLIES_TO | H2P-PW-022 SLA Printing | Strong | High | Supports commonly required | Process guidance |
| CONTRASTS_WITH | H2P-PW-024 SLS Polymer Printing | Strong | High | Powder bed provides self-support | ISO/process guidance |
| CONTRASTS_WITH | H2P-PW-025 MJF Printing | Strong | High | Powder bed provides self-support | Process guidance |

## Open gaps
Add quantitative design-rule ranges only after machine/process-specific validation.