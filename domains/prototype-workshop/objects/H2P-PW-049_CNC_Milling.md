---
id: H2P-PW-049
title: CNC Milling
object_type: Manufacturing Process
domain: Prototype Workshop
subdomain: CNC & Subtractive Prototyping
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, Pilot]
status: Researching
---

# CNC Milling

## Definition
Subtractive manufacture of prismatic or freeform parts using numerically controlled rotating cutting tools and controlled workpiece/tool motion.

## Prototype value
CNC milling is especially useful when the prototype must use engineering metal or plastic close to the intended production material, needs controlled interfaces, or requires surface/geometry that would be difficult to interpret from an additive prototype.

## Strengths
- Functional metal and engineering-plastic prototypes
- Tight controlled interfaces relative to many rapid-AM routes
- Broad material availability
- Secondary finishing of AM or molded prototypes
- High production representativeness when production will also be machined

## Limitations
- Tool-access constraints and internal corner radii
- Workholding/setup planning can dominate complexity
- Thin walls and tall features can deflect or chatter
- Tight tolerances increase cost and inspection burden
- Deep cavities and small tools increase risk and cycle time

## Design-rule starting points
Current Protolabs Network guidance recommends, as service-specific starting points, approximately 0.8 mm minimum metal walls and 1.5 mm plastic walls; standard drill sizes and relatively shallow aspect ratios are preferred. These are provider capability guidelines, not universal CNC limits.

## Prototype decision rule
Use CNC when material fidelity, interface precision, functional loading, temperature behavior, or production-representative machining matters more than the geometric freedom and speed advantages of AM.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| SUPPORTS | H2P-PW-173 Prototype Manufacturing Process Selection | Strong | High | CNC is a primary prototype route | NIST/MIT |
| SUPPORTS | H2P-PW-174 Prototype Production Representativeness | Strong | High | Machined material/process may better reproduce production intent | NIST |
| DEPENDS_ON | H2P-PW-059 Prototype Workholding | Mandatory | Very High | Part must be constrained and located | Machining fundamentals |
| DEPENDS_ON | H2P-PW-062 Machining Datum Strategy | Strong | Very High | Multiple setups require controlled references | Machining fundamentals |
| DEPENDS_ON | H2P-PW-063 Machining Tolerance Strategy | Strong | Very High | Tolerance requirements drive process and inspection | DFM guidance |
| USES | H2P-PW-058 CAM for Prototyping | Strong | High | Toolpaths and verification drive execution | NIST high-speed machining |

## Anchor evidence
NIST has documented high-speed CNC machining as a competitive rapid-prototyping route for functional metallic prototypes, emphasizing machine dynamics, tool-wear-aware parameter selection, intelligent toolpath generation and pre-process verification.

## Open gaps
Add authoritative machining handbooks and ISO GPS/GD&T cross-links during the DFM domain.