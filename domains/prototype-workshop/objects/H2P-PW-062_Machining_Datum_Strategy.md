---
id: H2P-PW-062
title: Machining Datum Strategy
object_type: Method
domain: Prototype Workshop
subdomain: CNC & Subtractive Prototyping
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, Pilot]
status: Researching
---

# Machining Datum Strategy

## Definition
Planning the reference surfaces, axes and features used to locate a workpiece through machining and inspection so that critical relationships are preserved across setups.

## Core principle
A prototype can be dimensionally acceptable feature-by-feature yet fail assembly if setup changes break the intended relationships between critical features. Datum strategy therefore links design intent, workholding, machining sequence and inspection.

## Practical rules
- Establish stable, accessible references early in the process.
- Reuse machined reference surfaces rather than raw-stock surfaces when tighter relationships are required.
- Align machining datums with functional/inspection datums when practical.
- Avoid unnecessary datum changes across setups.
- Plan flip/second-operation location before first-operation stock removal.
- Preserve enough stock or dedicated locating features for subsequent setups.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| REQUIRED_BY | H2P-PW-049 CNC Milling | Strong | Very High | Multi-operation milling relies on stable references | Machining fundamentals |
| REQUIRED_BY | H2P-PW-050 CNC Turning | Strong | High | Axial/radial references affect coaxial relationships | Machining fundamentals |
| GUIDES | H2P-PW-059 Prototype Workholding | Strong | Very High | Workholding must expose/preserve chosen datums | Machining fundamentals |
| SUPPORTS | H2P-PW-063 Machining Tolerance Strategy | Strong | High | Tolerances are interpreted relative to references | GD&T context |

## Open gaps
Cross-link later to ISO GPS and ASME Y14.5/GD&T entries in the DFM domain.