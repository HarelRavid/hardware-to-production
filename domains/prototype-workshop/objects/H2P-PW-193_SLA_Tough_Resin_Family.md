---
id: H2P-PW-193
title: SLA Tough Resin Family
object_type: Material Family
parent_process: H2P-PW-022
status: Researching
lifecycle: [Prototype, Engineering Prototype]
tags: [SLA, tough-resin, engineering-resin, polymer-am]
---
# SLA Tough Resin Family

## Definition
Engineering photopolymer formulations designed to provide greater toughness, ductility and fracture resistance than standard display/model resins.

## Engineering use
Useful for functional housings, snap fits, compliant features, impact-resistant prototypes and jigs/fixtures where standard brittle SLA resin would provide misleading mechanical learning.

## Decision criteria
Select the exact formulation according to stiffness, elongation, impact/fatigue, creep and temperature requirements. `Tough resin` is not one property set. For example, current Formlabs Tough 1000 and Tough 1500 formulations target different stiffness/ductility balances.

## Evidence examples
- Formlabs Tough 1000 reports 180% elongation at break, 932 MPa tensile modulus and HDT 55.3 °C at 0.45 MPa under its stated print/cure conditions.
- Tough 1500 V2 reports 155% elongation, 1460 MPa tensile modulus and HDT 66 °C at 0.45 MPa, targeting PP-like resilient behavior.

These are vendor/system-specific examples, not universal SLA material values.

## Relationships
| Type | Target | Strength | Reason |
|---|---|---|---|
| MATERIAL_FOR | H2P-PW-022 | Strong | SLA engineering photopolymer family. |
| SELECTED_BY | H2P-PW-177 | Strong | Resin family selection determines formulation. |
| REQUIRES | H2P-PW-183 | Mandatory | Final properties depend on defined post-cure state. |
| COMPARED_WITH | H2P-PW-196 | Strong | Durable formulations occupy a different compliance/friction trade space. |
| LIMITED_BY | H2P-PW-174 | Strong | Thermoplastic-like behavior does not make the process equivalent to molded thermoplastic production. |

## Podcast use
Prototype Shop — choosing SLA engineering resin for functional rather than purely visual prototypes.
