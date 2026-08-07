---
id: H2P-PW-059
title: Prototype Workholding
object_type: Method
domain: Prototype Workshop
subdomain: CNC & Subtractive Prototyping
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, Pilot]
status: Researching
provenance: [GNR, IND, SYN]
---

# 2.2.4 — Prototype Workholding

## Definition
The strategy used to locate, constrain and support a workpiece during machining while preserving access to required features and maintaining repeatable references between operations.

## Why it matters
Workholding is often a limiting factor in prototype machining because low-volume parts may have irregular geometry, incomplete reference surfaces or insufficient volume to justify dedicated production fixtures.

## Common options
- Standard vise and parallels
- Collets/chucks for rotational work
- Soft jaws
- Fixture plates and dowel/location schemes
- Vacuum workholding for suitable flat parts
- Sacrificial stock / tabs
- Rotary or 4th/5th-axis fixtures
- Tailstock or steady-rest support for slender turned parts

## Prototype strategy
Prefer the simplest workholding that reliably preserves datum relationships, tool access and part stiffness. For one-off prototypes, extra sacrificial material can be cheaper and faster than building a complex fixture. For repeat builds, soft jaws or modular fixtures can reduce setup variation.

## Failure modes
- Part movement under cutting load
- Distortion from over-clamping
- Lost datum after flipping
- Inaccessible features
- Insufficient support of thin walls/tall features
- Clamp marks on cosmetic or sealing surfaces
- Fixture collision or reduced tool reach

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| REQUIRED_BY | H2P-PW-049 CNC Milling | Mandatory | Very High | Milling requires stable constraint | Machining fundamentals |
| REQUIRED_BY | H2P-PW-050 CNC Turning | Mandatory | Very High | Turning requires chuck/collet/support strategy | Machining fundamentals |
| USES | H2P-PW-060 Soft Jaws | Strong | High | Soft jaws adapt low-volume workholding | Industry practice |
| USES | H2P-PW-061 Modular Fixturing | Medium | High | Modular fixtures can reduce prototype setup time | Industry practice |
| DEPENDS_ON | H2P-PW-062 Machining Datum Strategy | Strong | Very High | Workholding must preserve references | Machining fundamentals |

## Evidence notes
Commercial workholding documentation illustrates vise, chuck, collet, rotary and support categories across mills and lathes. Product-specific hardware is treated as examples, not normative recommendations.

## Open gaps
Add formal fixture-design references, 3-2-1 location principles, clamp-force considerations and distortion studies.
