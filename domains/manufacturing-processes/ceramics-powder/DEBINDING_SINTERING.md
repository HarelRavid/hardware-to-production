# 3.10.3 Debinding & Sintering Engineering

status: Researching
provenance: [GNR]

## Debinding objects
- thermal debinding
- solvent debinding
- catalytic debinding
- binder burnout
- gas evolution
- diffusion path
- heating rate
- hold/dwell
- cracking/blistering
- residual carbon/contamination

## Sintering objects
- densification
- neck growth
- diffusion mechanisms
- grain growth
- pore evolution
- open vs closed porosity
- shrinkage
- anisotropic shrinkage
- warpage
- atmosphere
- pressure-assisted sintering
- liquid-phase sintering

## Engineering principle
The thermal profile must be interpreted together with part geometry, binder content, green density, thermal mass, furnace loading and gas-transport conditions; a lab recipe is not automatically transferable to a larger batch.

## DFM / scale-up questions
1. What is the longest volatile-transport path in the part during debinding?
2. Can section-thickness variation create local debinding or sintering differences?
3. Is shrinkage isotropic enough for simple scale compensation, or must direction/feature be modeled separately?
4. Does furnace load mass alter ramp/soak behavior or atmosphere exchange?
5. Which properties require density/grain-size control rather than temperature control alone?

## Failure modes
- cracking
- bloating/blistering
- delamination
- incomplete binder removal
- contamination
- differential shrinkage
- slumping
- distortion
- residual porosity
- exaggerated grain growth

## Decision objects
### D-CER-DEBIND-001 — Debinding route and profile
### D-CER-SINT-001 — Pressureless vs pressure-assisted sintering route
### D-CER-CYCLE-001 — Does scale-up require a new instrumented thermal cycle?

## Cross-links
Green density <-> shrinkage
Binder system <-> debinding
Debinding <-> defect inheritance
Sintering <-> density
Sintering <-> grain growth
Furnace load <-> thermal history
Atmosphere <-> chemistry/microstructure

Quantitative profiles and temperatures are material/process-specific evidence objects.