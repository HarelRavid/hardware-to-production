# 3.6.11 Hole Making & Precision Features

status: Researching
provenance: [GNR]

## 3.6.11.1 Process chain objects
- Spot/center preparation
- Drilling
- Step drilling
- Gun/deep-hole drilling
- Boring
- Reaming
- Counterboring
- Countersinking
- Tapping
- Thread milling
- Honing
- Broaching

## 3.6.11.2 Engineering principle
A hole is not a single manufacturing feature. Diameter, straightness, cylindricity, position, finish, thread quality and datum relationship can require different operations and measurement strategies.

## 3.6.11.3 DFM questions
1. Does the functional requirement justify reaming/boring/honing after drilling?
2. Can hole depth-to-diameter and tool access be reduced?
3. Can a blind feature become through-access without harming function?
4. Is the thread best produced by tapping, forming, thread milling or another process?
5. Is the datum strategy compatible with the setup that produces the precision hole?
6. Can multiple precision features be produced in one datum-controlled setup?

## 3.6.11.4 Broaching objects
- Internal broaching
- External broaching
- Keyways
- Splines
- Form broaching
- Broach tool
- Progressive tooth rise
- Tool sharpening/life

Broaching is treated as a high-productivity form-generation option whose economics depend strongly on geometry, volume, dedicated tooling and machine/supplier capability.

## 3.6.11.5 Failure/cost drivers
- Drill wander
- Runout
- Burr formation
- Chip packing
- Tool breakage
- Poor thread engagement
- Bell-mouth/taper
- Datum transfer error
- Excessive setup count
- Dedicated broach tooling cost

## 3.6.11.6 Decision objects
### D-HOLE-001 — Drilled only or precision-finished hole?
### D-HOLE-002 — Ream, bore, grind or hone?
### D-THREAD-001 — Tap, form tap or thread mill?
### D-BROACH-001 — Broach or machine the form?

Each decision must use tolerance/GD&T, surface, depth/access, material, volume, cycle time, tooling cost, inspection and supplier capability as scoped inputs.

## 3.6.11.7 Cross-links
Hole making <-> GD&T
Hole making <-> fasteners
Threads <-> mechanical joining
Precision bores <-> press fits/bearings
Broaching <-> splines/keyways
Deep holes <-> coolant/chip evacuation

Quantitative process capability remains evidence-backlog content, not universal design rules.