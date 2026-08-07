---
id: H2P-PW-050
title: CNC Turning
object_type: Manufacturing Process
domain: Prototype Workshop
subdomain: CNC & Subtractive Prototyping
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, Pilot]
status: Researching
---

# CNC Turning

## Definition
Subtractive manufacture in which the workpiece rotates while cutting tools generate cylindrical, conical, grooved, threaded and bored features under numerical control.

## Prototype value
Turning is the natural route for shafts, bushings, spacers, threaded cylindrical parts, sealing diameters and rotational interfaces where concentricity and coaxial relationships matter.

## Strengths
- Efficient for rotational geometry
- Good control of concentric diameters and axial features
- Production-grade metal/plastic feedstock
- Useful for seal lands, bearing fits and threaded interfaces

## Limitations
- Geometry must be compatible with rotational access or combined mill-turn operations
- Long/slender parts may deflect and require tailstock/steady-rest strategy
- Chuck/collet grip can mark or distort delicate parts
- Multiple setups can complicate coaxiality if datums are not preserved

## Decision rule
Prefer turning over milling when the critical geometry is fundamentally axisymmetric and the performance question depends on concentricity, diameter control or rotational interfaces.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| SUPPORTS | H2P-PW-173 Prototype Manufacturing Process Selection | Strong | High | Turning is a core subtractive route | Machining fundamentals |
| DEPENDS_ON | H2P-PW-059 Prototype Workholding | Mandatory | Very High | Chuck/collet/tailstock strategy controls stability | Machining fundamentals |
| DEPENDS_ON | H2P-PW-062 Machining Datum Strategy | Strong | High | Axial and radial references must be preserved across setups | Machining fundamentals |
| DEPENDS_ON | H2P-PW-063 Machining Tolerance Strategy | Strong | High | Fits and concentricity drive method and inspection | DFM/GD&T context |

## Open gaps
Add turning-specific DFM ratios, boring/reaming strategies, thread classes and long-slender-part guidelines from authoritative machining handbooks.