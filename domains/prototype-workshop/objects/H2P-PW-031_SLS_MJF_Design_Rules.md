---
id: H2P-PW-031
title: SLS/MJF Design Rules
object_type: Method
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, Low-volume Production]
status: Researching
---

# SLS/MJF Design Rules

## Scope
Design rules for polymer powder-bed processes used for functional prototypes and low-volume production. SLS and MJF share powder-bed constraints but must not be treated as identical processes.

## Cross-Process Principles
- Surrounding powder usually provides self-support, so dedicated support structures are generally not required as in FDM/SLA.
- Enclosed cavities require powder escape paths.
- Large flat sections can distort due to thermal history and shrinkage.
- Clearance, wall thickness and small-feature rules are machine/material specific.
- Surface finish and hole quality may require secondary finishing or machining.

## MJF Example Values
One industrial service provider publishes the following PA12 starting values:
- General tolerance: ±0.3% with minimum ±0.5 mm
- Minimum supported wall: 1.0 mm
- Minimum unsupported wall: 1.5 mm
- Minimum pin diameter: 2.0 mm
- Minimum hole/gap: 0.5 mm
- Large flat planes identified as warpage risk
- Printed threads recommended at M6 or larger in that provider's process, with coarse profiles preferred

Source: Forge Labs MJF Design Guidelines. Values are provider-specific examples, not universal HP or ISO capability limits.

## SLS Standards Context
ISO/ASTM 52911-2:2019 specifically addresses laser-based powder bed fusion of polymers. Its design scope includes process benefits and limitations, feature constraints, overhang/stair-step behavior, and dimensional/form/positional accuracy.

## Engineering Interpretation
1. Use SLS/MJF when nested geometry, functional nylon parts, and support-free packing are valuable.
2. Avoid assuming that absence of supports means absence of design constraints; powder evacuation and thermal distortion remain important.
3. Critical bores, bearing interfaces, threads and sealing features should be verified or post-machined.
4. Maintain separate capability records for SLS vs MJF and for PA12 vs PA11 vs reinforced or flexible powders.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---:|---:|---|---|
| APPLIES_TO | H2P-PW-024 | Mandatory | High | Rules apply to polymer SLS/LB-PBF | ISO/ASTM 52911-2 |
| APPLIES_TO | H2P-PW-025 | Strong | High | Many powder-bed design concerns apply to MJF | industrial process guidance |
| DEPENDS_ON | H2P-PW-178 | Strong | High | Powder family affects capability | manufacturer data |
| DEPENDS_ON | H2P-PW-034 | Strong | High | Shrinkage/compensation affects final dimensions | standard + industrial guidance |
| DEPENDS_ON | H2P-PW-037 | Medium | High | Surface state affects fits and finishing | industrial guidance |
| INFORMS | H2P-PW-173 | Strong | High | Design feasibility informs process selection | project synthesis |
