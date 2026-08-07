---
id: H2P-PW-199
title: Support-Induced Surface and Geometry Effects
object_type: Concept
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
---

# Support-Induced Surface and Geometry Effects

## Definition
Surface, dimensional and geometric effects caused by support contact, support removal, local thermal history, or orientation choices made to enable additive manufacture.

## Why it matters
For support-dependent processes such as FDM/FFF and many vat-photopolymerization workflows, support contact can change local surface finish, edge quality and dimensional condition. Removing supports can also damage thin features or change fit-critical surfaces.

## Engineering implications
- Keep critical sealing, bearing, cosmetic and datum surfaces away from support contact when practical.
- Treat support scars as a process condition, not cosmetic noise, when surface condition affects function.
- Include support strategy in orientation decisions rather than optimizing only print time.
- Consider machining or secondary finishing allowance on critical interfaces.
- Record orientation/support state in build records when results are used for comparative testing.

## Process distinction
### FDM / FFF
Support interfaces can leave roughness, witness marks and local geometry changes; soluble support can reduce removal damage but does not eliminate orientation effects.

### SLA / MSLA
Support touchpoints and removal can mark surfaces and damage fine features; orientation is often selected to trade support placement against peel forces, drainage and accuracy.

### SLS / MJF
Loose powder generally provides self-support, so dedicated support contact is avoided, but powder removal, thermal distortion and surface texture remain relevant constraints.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| DEPENDS_ON | H2P-PW-032 Additive Support Strategy | Mandatory | Very High | Support strategy creates or avoids contact regions | Process logic |
| AFFECTS | H2P-PW-037 Additive Prototype Surface Finish | Strong | Very High | Contact/removal alters local surface | Process guidance |
| AFFECTS | H2P-PW-036 Additive Prototype Accuracy | Strong | High | Thin features and fit surfaces can shift or be damaged | NIST/process guidance |
| AFFECTS | H2P-PW-030 Resin Printing Design Rules | Strong | High | SLA support placement is a design variable | Industry guidance |
| AFFECTS | H2P-PW-029 FDM Design Rules | Strong | High | Support accessibility and interface quality affect design | Industry guidance |

## Open gaps
Add quantified surface-roughness and dimensional-change studies by process/support-interface type without generalizing one machine/material combination to the full process family.