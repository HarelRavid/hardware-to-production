# 3.13 Cleaning, Contamination Control & Clean Manufacturing — Domain Map

status: Researching
provenance: [GNR]

## 3.13.1 Scope
Manufacturing engineering of part cleanliness from incoming condition through cleaning, drying, verification, controlled handling and packaging, including contamination introduced by upstream/downstream processes.

## 3.13.2 Contamination families
- particles
- chips/burr debris
- oils/grease
- machining coolant residue
- fingerprints/handling residue
- ionic contamination
- salts
- organic films
- polishing compounds
- abrasive/blast media
- oxide/corrosion products
- process chemicals
- moisture/water films
- biological/bioburden boundary where application requires it

## 3.13.3 Cleaning process families
- manual wiping
- aqueous cleaning
- spray cleaning
- immersion
- ultrasonic cleaning
- solvent cleaning
- vapor degreasing boundary
- alkaline/acid cleaning
- precision cleaning
- flushing
- high-purity rinsing
- plasma/UV-ozone/special surface activation boundary

## 3.13.4 Cross-cutting objects
- soil/contaminant
- substrate compatibility
- cleaner chemistry
- concentration
- temperature
- time
- mechanical action
- rinse quality
- water quality
- drying
- residue
- bath life
- filtration
- cross-contamination
- handling
- packaging
- cleanliness verification
- clean environment

## 3.13.5 Engineering principle
“Clean” is not a binary material property. A cleanliness requirement must define what contamination matters, where, how much is acceptable, how it is measured and how the verified state is preserved until the next critical operation or service condition.

## 3.13.6 Master decision object
### D-CLEAN-MASTER-001 — What cleanliness system is required?
Inputs: next process/function, substrate, contaminant type, geometry/internal passages, compatibility, allowable residue, particle/ionic/organic limits, drying, environment, packaging, inspection, volume/takt, safety/environmental constraints and supplier capability.

Output: prevention + cleaning route + rinse/dry + verification + handling/packaging + evidence + assumptions/open questions.

## 3.13.7 Cross-domain links
Cleaning <-> joining/adhesive bonding
Cleaning <-> coating/surface engineering
Cleaning <-> machining
Cleaning <-> fluid/gas systems
Cleaning <-> electronics
Cleaning <-> assembly
Cleaning <-> packaging/logistics
Cleaning <-> quality/traceability

## Integrity rule
A cleaning process is not qualified merely because the part looks clean. Quantitative acceptance requires scoped measurement and evidence.