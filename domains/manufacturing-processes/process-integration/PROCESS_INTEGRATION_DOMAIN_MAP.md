# 3.15 Manufacturing Process Integration — Domain Map

status: Researching
provenance: [GNR]

## 3.15.1 Scope
Engineering of complete manufacturing process chains, including sequence effects, cumulative variation, datum migration, thermal/mechanical history, contamination/finish interactions, cross-process failure modes, yield, inspection placement and total process-chain economics.

## 3.15.2 Core principle
A manufacturing process cannot always be optimized independently. The output state of one operation becomes the input condition of the next, and local optimization can degrade total product quality, yield, cost or reliability.

## 3.15.3 Process-chain object
A process chain is represented as ordered operations plus state transitions.

Operation N -> changes material/geometry/surface/stress/cleanliness/property state -> Operation N+1.

Each transition may carry:
- dimensions/GD&T state
- datum state
- surface/cleanliness state
- material/microstructure state
- residual stress/distortion state
- coating/oxide state
- moisture/chemical state
- traceability state
- inspection/release state

## 3.15.4 Canonical chain examples
- Casting -> heat treatment -> machining -> cleaning -> coating -> assembly
- Forging -> heat treatment -> rough machining -> finish machining -> surface treatment
- Sheet forming -> joining -> cleaning -> coating -> final assembly
- Additive build -> stress relief/HIP boundary -> machining -> cleaning -> inspection
- Composite cure -> trim/drill -> clean -> bond -> cure -> NDT
- Injection molding -> trim/degate -> conditioning -> assembly -> test

## 3.15.5 Master decision object
### D-INT-MASTER-001 — What is the optimal manufacturing process chain?
Inputs: function, material, geometry, tolerance, surface, properties, cleanliness, joining, inspection, volume, supplier boundaries, automation, logistics, rework, yield and lifecycle cost.

Output: candidate process sequences + intermediate-state requirements + inspection gates + risks + assumptions + evidence.

## 3.15.6 Cross-domain links
Process integration links all 3.x manufacturing domains and connects them to Production System Engineering, Quality, Supplier Industrialization, Automation and the Manufacturing Atlas.

## Integrity rule
Do not infer whole-chain capability by combining isolated best-case capability numbers from individual processes.