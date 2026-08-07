# Polymer AM — Design Rules Source Index

Purpose: listener/researcher-facing source map for numerical design rules. Numbers in supplier guides remain supplier/process specific unless independently validated.

## Standards / Authoritative

- ISO/ASTM 52911-2:2019 — Additive manufacturing — Design — Part 2: Laser-based powder bed fusion of polymers. Covers polymer LB-PBF/P process characteristics, limitations, feature constraints, stair-step behavior and dimensional/form/positional accuracy.
- ISO/ASTM 52910:2018 — General AM design requirements, guidelines and recommendations.
- NIST — Measurement Science Roadmap for Polymer-Based Additive Manufacturing.
- NIST — Study of Accuracy of Parts Produced Using Additive Manufacturing.
- NIST — Additive Manufacturing Part Qualification program.

## Industrial Design Guides

### FDM
Forge Labs — FDM Design Guidelines
https://forgelabs.com/design-guides/fdm

Published examples include 1.0 mm minimum wall, 0.5 mm minimum clearance, provider-specific tolerance of ±0.3% with minimum ±0.25 mm, and guidance favoring inserts for most repeated-use threads.

### SLS
Formlabs — Designing for SLS 3D Printing on Fuse 1+ 30W
https://formlabs.com/blog/fuse-1-sls-design-guide/

Useful for minimum-feature framework, powder escape holes, orientation and packing. Exact numerical limits should be taken from the current machine design guide rather than generalized across SLS systems.

### MJF
Forge Labs — MJF Design Guidelines
https://forgelabs.com/design-guides/mjf

Published PA12 examples include 1.0 mm supported walls, 1.5 mm unsupported walls, 0.5 mm minimum hole/gap, provider-specific tolerance of ±0.3% with minimum ±0.5 mm, and warnings about large-flat-surface warpage.

### SLA / Vat Photopolymerization
Simple Machining — SLA 3D Printing Service / Design Guidelines
https://www.simplemachining.com/sla-3d-printing-service

Secondary industrial source useful for initial reference values such as wall thickness, drainage and mating clearances. Treat as a service-provider capability guide and cross-check critical values against the target machine/resin supplier.

## Data-use Rule

Whenever a numerical value from these sources is used in a Knowledge Object or podcast:

1. identify the source/provider;
2. identify process/material where given;
3. state whether it is a recommendation, advertised capability or measured result;
4. do not present it as an ISO requirement unless the standard actually defines that requirement;
5. revalidate against the actual manufacturing route before using it as an acceptance criterion.
