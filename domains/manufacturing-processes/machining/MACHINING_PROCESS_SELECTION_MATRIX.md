# 3.6.16 Machining Process Selection Matrix

status: Researching
provenance: [GNR]

## 3.6.16.1 Purpose
Provide a comparison structure across turning, milling, drilling/boring/reaming, grinding, honing/lapping, broaching and EDM. It is a decision framework, not a universal ranking table.

## 3.6.16.2 Common criteria
- geometry family
- rotational symmetry
- tool access
- aspect ratio / reach
- material hardness and conductivity where relevant
- tolerance/GD&T
- surface texture/integrity
- burr/edge requirement
- production volume
- setup count
- dedicated tooling
- cycle time
- automation
- inspectability
- secondary-process requirement
- supplier capability

## 3.6.16.3 Candidate-process logic
### Turning
Strong candidate when major geometry is rotationally symmetric and can be established efficiently from a spindle datum.

### Milling
Strong candidate for prismatic, pocketed, planar and multi-face geometry where cutter access is available.

### Drilling / Boring / Reaming
Feature-chain candidates where hole function determines whether simple generation or precision finishing is required.

### Grinding
Candidate for hardened materials or functional surfaces requiring higher dimensional/texture control or specific surface generation, subject to surface-integrity risk.

### Honing / Lapping / Superfinishing
Finishing candidates when bore geometry, texture or tribological function justify dedicated secondary finishing.

### Broaching
Candidate for repeatable forms such as internal profiles, splines/keyways or high-volume form generation when dedicated tooling economics are justified.

### EDM
Candidate for electrically conductive materials where conventional cutter access, hardness or intricate geometry make contact cutting unsuitable; recast/surface-integrity implications must be assessed.

## 3.6.16.4 Cross-family comparison
Machining should also be compared against:
- casting + finish machining
- forging + finish machining
- extrusion + finish machining
- sheet-metal fabrication
- additive + finish machining
- molding where material/product context allows

## 3.6.16.5 Decision object
### D-MACH-MASTER-001 — Which material-removal route should produce this functional feature?
Inputs:
- geometry
- material/state
- tolerance/GD&T
- surface function
- volume
- tool/access constraints
- blank route
- automation
- inspection
- cost/lead time

Output should be candidate routes with benefits, risks, required evidence and open questions rather than a single unqualified recommendation.

## 3.6.16.6 GNR rule
Any qualitative comparison icons, rankings or generic volume thresholds added later remain GNR until each cell is scoped and evidence-linked.