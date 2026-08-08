# 3.10.8 Economics, Process Selection & Quality Gate

status: Researching
provenance: [GNR]

## Cost architecture
Cost per good part includes:
- powder/raw materials
- formulation/mixing/milling
- granulation/feedstock preparation
- forming labor/machine time
- molds/dies/tooling amortization
- drying/debinding
- furnace cycle energy and occupancy
- atmosphere/gas
- setters/fixtures and replacement
- yield/scrap/rework
- machining/finishing
- inspection/metrology
- batch genealogy/traceability
- maintenance and furnace downtime

## Scale-up risk objects
- batch size
- furnace thermal mass
- gas flow/distribution
- part spacing
- setter stack/load
- powder/green-body consistency
- cycle duration
- bottleneck operation
- yield loss after long-value-add cycle

## Master decision
### D-CPM-MASTER-001 — Which powder/ceramic manufacturing route should be used?
Candidate routes may include pressing, CIP, slip casting, tape casting, extrusion, ceramic injection molding, PM, MIM, additive powder routes, machining from stock, or alternate material/process families.

Inputs: material system, geometry, thickness, anisotropy, density/porosity, surface, tolerance, functional microstructure, annual volume, tooling, thermal process, atmosphere, secondary machining, inspection, supplier capability and lifecycle cost.

## Architecture coverage
- domain taxonomy: COMPLETE
- powder preparation: COMPLETE architecture
- forming: COMPLETE architecture
- debinding/sintering: COMPLETE architecture
- furnace/atmosphere/fixtures: COMPLETE architecture
- shrinkage/dimensional control: COMPLETE architecture
- porosity/microstructure: COMPLETE architecture
- machining/metrology: COMPLETE architecture
- PM/MIM boundary: COMPLETE architecture
- economics/selection: COMPLETE architecture

## Open evidence/population work
- standards/source map and revisions
- quantitative powder characterization methods
- material-specific sintering/cure kinetics
- debinding defect literature
- furnace/load scale-up evidence
- dimensional capability and shrinkage datasets
- porosity/property evidence
- industrial case studies
- additive-manufacturing boundary evidence
- top questions/decisions/mistakes/myths/lessons
- GNR verification

## Integrity gates before Podcast Ready
1. No universal shrinkage factor.
2. Thermal recipe is distinguished from actual part thermal history.
3. Furnace/load/fixture configuration is represented in scale-up claims.
4. Green-state and final-state measurements are distinguished.
5. Density, porosity and microstructure claims are material/process scoped.
6. Powder family and actual powder specification are distinguished.
7. PM/MIM/ceramic rules are not conflated.
8. Standards carry revision/applicability.
9. Decisions expose assumptions and open questions.
10. AI synthesis remains GNR until verified.

## Status
Architecture: CLOSED
Knowledge population: OPEN
Evidence verification: OPEN
Podcast readiness: NOT READY

## Next domain
3.11 Additive Manufacturing.