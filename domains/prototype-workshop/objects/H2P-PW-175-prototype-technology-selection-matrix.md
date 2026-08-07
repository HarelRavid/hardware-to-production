---
id: H2P-PW-175
title: Prototype Technology Selection Matrix
aliases: [Prototype Process Comparison Matrix]
object_type: Decision Tool
domain: Prototype Workshop
subdomain: Capability & Technology Selection
lifecycle: [POC, Prototype, Engineering Prototype, EVT, DVT]
status: Draft
tags: [ProcessSelection, RapidPrototyping, CNC, AdditiveManufacturing, SheetMetal]
created: 2026-08-07
last_reviewed: 2026-08-07
---

# Prototype Technology Selection Matrix

This matrix is an initial qualitative decision layer. It is not a machine-vendor capability chart. Values must later be refined by material, equipment class and supplier capability.

Legend: **Strong** = commonly advantageous; **Conditional** = depends strongly on geometry/material/equipment; **Weak** = generally not the reason to choose the process.

| Criterion | FDM/FFF | SLA/MSLA | SLS/MJF | CNC Milling | CNC Turning | Laser-cut Sheet | Waterjet | Bent Sheet Metal |
|---|---|---|---|---|---|---|---|---|
| Very fast one-off iteration | Strong | Strong | Conditional | Conditional | Conditional | Strong | Strong | Conditional |
| Low setup / no hard tooling | Strong | Strong | Strong | Conditional | Conditional | Strong | Strong | Conditional |
| Complex enclosed geometry | Strong | Strong | Strong | Weak | Weak | Weak | Weak | Weak |
| Fine visual detail | Conditional | Strong | Conditional | Strong | Strong | Conditional | Conditional | Conditional |
| Functional engineering plastics | Conditional | Conditional | Strong | Strong | Strong | Weak | Conditional | Weak |
| Production-grade metal behavior | Weak | Weak | Weak | Strong | Strong | Strong | Strong | Strong |
| Tight machined interfaces | Weak | Conditional | Conditional | Strong | Strong | Weak | Conditional | Conditional |
| Large flat 2D parts | Weak | Weak | Weak | Conditional | Weak | Strong | Strong | Strong |
| Representative sheet-metal geometry | Weak | Weak | Weak | Weak | Weak | Conditional | Conditional | Strong |
| Internal channels / lattices | Strong | Strong | Strong | Weak | Weak | Weak | Weak | Weak |
| Low-volume batch without tooling | Strong | Conditional | Strong | Conditional | Conditional | Strong | Strong | Strong |
| Easy local design changes | Strong | Strong | Strong | Conditional | Conditional | Strong | Strong | Conditional |
| Production-process representativeness | Weak–Conditional | Weak | Conditional | Conditional | Conditional | Strong for cut sheet | Strong for cut profile | Strong for sheet products |
| Typical post-processing burden | Medium | Medium–High | Medium | Medium | Medium | Low–Medium | Low–Medium | Medium |

## Selection Sequence
1. Define the question to be answered.
2. Define the minimum required fidelity dimensions.
3. Identify must-match material/functional properties.
4. Eliminate processes that cannot satisfy geometry or loading.
5. Evaluate production representativeness requirement.
6. Compare total lead time, not only machine cycle time.
7. Compare total cost, including setup, post-processing, inspection and engineering labor.
8. Check internal capability and supplier risk.
9. Record what the chosen process cannot prove.

## Evidence Notes
- NIST highlights AM's ability to avoid tooling lead time, accelerate iteration and improve low-volume economics.
- NIST research demonstrates high-speed CNC machining as a competitive rapid-prototyping route for functional metallic prototypes.
- MIT 2.008 treats manufacturing choices in the integrated context of process, cost, quality and flexibility and includes machining, sheet metal, molding and additive manufacturing.
- ISO/ASTM 52910 and 52911 reinforce that additive-process design decisions are process-specific rather than generic to all 3D printing.

## Relationships
| Type | Target Object | Strength | Confidence | Reason |
|---|---|---|---|---|
| IMPLEMENTS | H2P-PW-173 Prototype Manufacturing Process Selection | Strong | High | Provides a common comparison surface for the selection method. |
| USES | H2P-PW-174 Prototype Production Representativeness | Strong | High | Representativeness is a separate selection dimension. |
| COMPARES | H2P-PW-021 FDM / FFF Printing | Medium | High | Candidate process. |
| COMPARES | H2P-PW-022 SLA Printing | Medium | High | Candidate process. |
| COMPARES | H2P-PW-024 SLS Polymer Printing | Medium | High | Candidate process. |
| COMPARES | H2P-PW-025 MJF Printing | Medium | Medium | Candidate process. |
| COMPARES | H2P-PW-049 CNC Milling | Medium | High | Candidate process. |
| COMPARES | H2P-PW-050 CNC Turning | Medium | High | Candidate process. |
| COMPARES | H2P-PW-068 CO2 Laser Cutting | Medium | Medium | Candidate process. |
| COMPARES | H2P-PW-069 Fiber Laser Cutting | Medium | Medium | Candidate process. |
| COMPARES | H2P-PW-070 Waterjet Cutting | Medium | Medium | Candidate process. |
| COMPARES | H2P-PW-072 Sheet Metal Bending | Medium | High | Candidate process. |

## Research Gaps
The matrix deliberately avoids numeric tolerances and cost thresholds until process-specific objects are researched. Those values depend on material, machine architecture, part size, orientation and supplier capability and would be misleading if generalized too early.
