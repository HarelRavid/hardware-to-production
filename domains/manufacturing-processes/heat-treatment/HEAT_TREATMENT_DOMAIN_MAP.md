# 3.14 Heat Treatment & Thermal Processing — Domain Map

status: Researching
provenance: [GNR]

## 3.14.1 Scope
Production heat treatment of metals from incoming material condition through thermal cycle, atmosphere, quench/cooling, distortion control, property verification, traceability and integration with machining/forming/joining/surface engineering.

## 3.14.2 Process families
- annealing
- stress relief
- normalizing boundary
- hardening and tempering
- solution heat treatment
- precipitation aging
- homogenization boundary
- spheroidizing boundary
- carburizing / carbonitriding
- nitriding / nitrocarburizing
- induction/local hardening boundary
- vacuum heat treatment
- controlled-atmosphere heat treatment
- cryogenic/sub-zero treatment boundary

## 3.14.3 Thermal-process objects
- material/alloy/condition
- furnace
- load
- fixture/basket
- part geometry/section thickness
- setpoint/program
- actual part temperature
- ramp/heating rate
- soak/dwell
- atmosphere/vacuum
- quench/cooling rate
- transfer time
- temper/age
- distortion
- oxidation/decarburization
- hardness/microstructure/properties
- genealogy

## 3.14.4 Engineering principle
A furnace recipe is not the same object as the thermal history experienced by every part. Load mass, geometry, position, fixture thermal mass, furnace uniformity, atmosphere and transfer/quench conditions can change the metallurgical result.

## 3.14.5 Master decision object
### D-HT-MASTER-001 — What thermal-processing route is required?
Inputs: alloy/material condition, target properties/microstructure, geometry, section thickness, dimensional requirements, upstream history, downstream machining/coating/joining, atmosphere sensitivity, production volume, furnace/supplier capability, inspection and qualification.

Output: thermal route + furnace/atmosphere + load/fixture strategy + quench/cooling + verification + traceability + evidence + assumptions/open questions.

## 3.14.6 Cross-domain links
Heat treatment <-> forming
Heat treatment <-> casting
Heat treatment <-> machining
Heat treatment <-> welding/joining
Heat treatment <-> additive manufacturing
Heat treatment <-> surface engineering
Heat treatment <-> dimensional control/GD&T
Heat treatment <-> metallurgy/material selection

## Integrity rule
No time/temperature recipe, hardness conversion or distortion allowance is universalized across alloy, section, furnace/load and required material condition.