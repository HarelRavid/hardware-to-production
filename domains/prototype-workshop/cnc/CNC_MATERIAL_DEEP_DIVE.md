# 2.2.7 CNC Materials — Deep Dive

provenance: [GNR, GOV, IND, SYN]
status: Researching

## 2.2.7.1 Selection principle
Choose the exact material grade to match the prototype question. For fit/geometry work, machinability and lead time may dominate. For functional validation, thermal, chemical, stiffness, fatigue, conductivity or friction behavior may dominate. Same-family labels are not sufficient for engineering decisions.

## 2.2.7.2 Metal groups
### Aluminum alloys
Common prototype choices include 6061 and 7075. 6061 is often preferred for general mechanical prototypes because it is widely available and comparatively easy to machine; 7075 is selected when higher strength is needed. Do not infer production-process fidelity merely from alloy match.

### Carbon and alloy steels
Useful where stiffness, wear resistance, strength or magnetic behavior matter. Hardness and heat-treatment state strongly influence cutting force, tool wear and achievable finish.

### Stainless steels
Austenitic grades such as 304/316 are common for corrosion-sensitive prototypes but are more demanding to machine than free-cutting steels due to work hardening, adhesion and chip-control behavior. Tooling and process parameters should be chosen specifically for the grade and condition.

### Titanium alloys
Useful when high specific strength, corrosion resistance or biocompatibility are part of the learning objective. Titanium is commonly treated as a difficult-to-machine material because low thermal conductivity, strength and adhesive behavior increase tool-temperature and wear challenges. Seco notes that machinability is influenced by adhesion, strain hardening, thermal conductivity, hardness and abrasiveness.

### Brass and copper
Brass is generally favorable for machining and is useful for fittings, small precision parts and low-friction interfaces. Copper is important where electrical or thermal conductivity matters, but grade and temper influence machinability.

## 2.2.7.3 Engineering plastics
### POM / acetal
Useful for low-friction mechanisms, wear surfaces and dimensionally stable plastic prototypes. Machining can produce geometry and bulk-material behavior without AM layer effects.

### PEEK
Useful for high-temperature, chemical and high-performance engineering prototypes. Material cost is high; use only where the prototype question requires it.

### PTFE
Useful for chemical resistance and low friction, but soft behavior and dimensional instability can complicate tight tolerances and surface control.

### Polycarbonate / PMMA
Useful for transparent or semi-transparent prototypes, covers, guards and optical-mechanical evaluation. Machining strategy must account for cracking, heat and finish requirements.

### HDPE / UHMWPE
Useful for low-friction, chemical-resistant and wear-related prototypes. Their low stiffness can make thin or weakly supported geometry difficult to hold accurately during machining.

## 2.2.7.4 Machinability rule
Machinability is not a single material constant. Seco describes it as an average comparative rating influenced by chip formation, cutting forces, temperature, tool wear and workpiece quality. Treat machinability as a system property of material + condition + tool + machine + process parameters.

## 2.2.7.5 Plastic-machining note
Ensinger machining guidance for engineering plastics highlights that material-specific behavior can include moisture sensitivity, flash formation and surface roughness effects. Plastics should not be treated as 'easy aluminum'.

## 2.2.7.6 Decision logic
1. Define the property to be validated.
2. Decide whether exact production grade is required.
3. Confirm stock availability and condition.
4. Check machining difficulty and thermal/chip-control risks.
5. Decide whether alternate material can answer the same prototype question faster or cheaper.
6. Record any substitution explicitly in the build record.

## Relationships
- SUPPORTS -> H2P-PW-064 Prototype Machining Material Selection
- SUPPORTS -> H2P-PW-174 Prototype Production Representativeness
- AFFECTS -> H2P-PW-065 CNC Tooling Selection
- AFFECTS -> H2P-PW-199 CNC Prototype Cost Drivers
- AFFECTS -> H2P-PW-200 CNC Prototype Lead-Time Drivers

## Sources
- NIST high-speed CNC prototype work
- Seco Tools: difficult-to-machine materials and machinability concepts
- Ensinger machining guidelines for semi-finished engineering plastics
