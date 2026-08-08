# Hardware-to-Production Data Hub — Master WBS

status: CANONICAL ROADMAP
version: 1.0
purpose: Prevent domain drift, duplicate coverage and accidental renumbering.

## 0. Governance & Knowledge OS
0.1 Scope and methodology
0.2 Source-quality ranking
0.3 Claim/evidence model
0.4 Decision objects
0.5 Provenance and GNR handling
0.6 Standards revision/applicability control
0.7 Cross-domain relationships
0.8 Quality gates / Podcast Ready criteria
0.9 Glossary and ontology
0.10 Source index

## 1. Product Development → Production Readiness
1.1 POC / prototype / MVP / production-intent distinctions
1.2 EVT / DVT / PVT / pilot / ramp
1.3 NPI and industrialization ownership
1.4 Product readiness vs manufacturing readiness
1.5 Hardware Manufacturing Readiness Matrix
1.6 Production-intent evidence and exit criteria

## 2. DFM / DFA / DFT Foundations
2.1 DFM principles and process-driven design
2.2 DFA and mistake prevention
2.3 DFT / calibration / traceability by design
2.4 Tolerances, GD&T and variation
2.5 Material selection for manufacturing
2.6 Reliability/service/repair considerations
2.7 Prototype-to-production representativeness
2.8 Cross-process design decision framework

## 3. Manufacturing Processes

### 3.0 Process Selection Framework
3.0.1 Functional requirements
3.0.2 Material/process compatibility
3.0.3 Geometry and size
3.0.4 Tolerance/GD&T
3.0.5 Surface requirements
3.0.6 Volume/takt
3.0.7 Tooling/NRE
3.0.8 Process capability and yield
3.0.9 Inspection/qualification
3.0.10 Automation potential
3.0.11 Supply-chain maturity
3.0.12 Cost per good part / lifecycle economics
3.0.13 Prototype vs serial-production route
3.0.14 Make/buy and supplier capability

### 3.1 Process Selection / Manufacturing-Process Atlas
Cross-family selection logic and Manufacturing Atlas interface. This is the navigation/decision layer, not a duplicate process encyclopedia.

### 3.2 Polymer Injection Molding
status: architecture built

### 3.3 Metal Casting
status: architecture built

### 3.4 Metal Forming
Includes sheet-metal and bulk-forming families according to existing domain content.
status: architecture built

### 3.5 Joining
Welding, brazing/soldering, adhesive joining, mechanical fastening and applicable polymer joining boundaries.
status: architecture built

### 3.6 Machining & Material Removal
Turning, milling, hole-making, grinding/precision finishing, EDM, tooling, surface integrity and production engineering.
status: architecture closed; population/evidence open

### 3.7 Polymer Forming Beyond Injection Molding
Extrusion, blow molding, thermoforming/vacuum forming, rotational molding, compression/transfer/RIM.
status: architecture closed; population/evidence open

### 3.8 Composite Manufacturing
Layup, vacuum bagging/infusion, RTM, prepreg/autoclave/OOA, filament winding, pultrusion, compression composites, ATL/AFP, sandwich/joining/machining.
status: architecture closed; population/evidence open

### 3.9 Rubber & Elastomer Manufacturing
Compression/transfer/injection/LSR, extrusion, seals, bonding, cure/post-cure, aging and inspection.
status: architecture closed; population/evidence open

### 3.10 Ceramics & Powder-Based Manufacturing
Powder preparation, forming, tape/slip casting, debinding, sintering, furnace/atmosphere/fixtures, porosity/microstructure, green/hard machining, PM/MIM boundaries.
status: architecture closed; population/evidence open

### 3.11 Additive Manufacturing
Polymer AM, metal AM, DfAM, orientation/supports, feedstock, qualification, post-processing, inspection and AM-vs-conventional decisions.
status: architecture closed; population/evidence open

### 3.12 Surface Engineering & Finishing
LOCKED NEXT DOMAIN.
Scope to include:
3.12.1 Surface preparation and cleanliness state
3.12.2 Mechanical finishing: deburring, blasting, tumbling, polishing, brushing
3.12.3 Plating / electroplating / electroless deposition
3.12.4 Conversion coatings and passivation
3.12.5 Anodizing
3.12.6 Paint / powder coating / liquid coating
3.12.7 PVD / CVD / thermal spray / hard coatings boundaries
3.12.8 Surface hardening / case-treatment boundary with heat treatment
3.12.9 Coating thickness, adhesion, porosity and coverage
3.12.10 Masking, fixturing and rack/contact effects
3.12.11 Corrosion/environmental performance
3.12.12 Surface inspection and testing
3.12.13 Rework/stripping/repair
3.12.14 DFM, economics, automation and process selection

### 3.13 Cleaning, Contamination Control & Clean Manufacturing
Scope to include:
3.13.1 Part cleanliness requirements
3.13.2 Aqueous/solvent/ultrasonic cleaning
3.13.3 Precision cleaning
3.13.4 Particle, ionic, organic and film contamination
3.13.5 Drying and residue control
3.13.6 Cleanroom/controlled-environment boundaries
3.13.7 Packaging after cleaning
3.13.8 Cleanliness verification
3.13.9 Process compatibility and corrosion risk
3.13.10 Automation/economics

### 3.14 Heat Treatment & Thermal Processing
Scope to include:
3.14.1 Annealing / stress relief
3.14.2 Hardening / tempering
3.14.3 Solution treatment / aging
3.14.4 Case hardening / nitriding / carburizing boundaries
3.14.5 Atmosphere/vacuum furnaces
3.14.6 Quenching
3.14.7 Distortion/residual stress
3.14.8 Furnace uniformity/load configuration
3.14.9 Metallurgy/property verification
3.14.10 Qualification/traceability/economics

### 3.15 Manufacturing Process Integration
Cross-process chains and sequence effects.
3.15.1 Near-net + machining
3.15.2 Forming + heat treatment + machining
3.15.3 Joining + finishing
3.15.4 Cleaning before joining/coating
3.15.5 AM + thermal/post-processing + machining
3.15.6 Datum migration across operations
3.15.7 Cumulative variation and distortion
3.15.8 Process-chain cost and yield
3.15.9 Sequence-dependent failure modes
3.15.10 Integrated process-selection decision objects

## 4. Production System Engineering
4.1 EBOM → MBOM
4.2 Process flow / routing
4.3 Tooling, jigs and fixtures
4.4 Work instructions
4.5 Standard work
4.6 Training and operator qualification
4.7 PFMEA / control plans / quality gates
4.8 Production test and calibration
4.9 Measurement-system capability
4.10 Material handling and internal logistics
4.11 Line layout and ergonomics

## 5. Pilot, Validation & Ramp
5.1 Pilot-build planning
5.2 Production validation build
5.3 Yield / FPY / RTY
5.4 Rework and scrap
5.5 Learning curve
5.6 Capacity and bottlenecks
5.7 Takt and line balance
5.8 Supplier readiness
5.9 Engineering changes during ramp
5.10 Ramp exit criteria

## 6. Quality, Reliability & Compliance
6.1 Quality planning
6.2 Incoming/process/final inspection
6.3 MSA
6.4 SPC and process capability
6.5 Nonconformance / MRB / CAPA
6.6 Reliability validation
6.7 Traceability and genealogy
6.8 Standards/regulatory overlays
6.9 Auditability and evidence retention

## 7. Supply Chain & Supplier Industrialization
7.1 Make/buy
7.2 Supplier selection
7.3 Supplier capability evidence
7.4 RFQ technical package
7.5 First article / sample approval
7.6 Supplier quality
7.7 Contract manufacturer management
7.8 Dual sourcing and resilience
7.9 Obsolescence/change control

## 8. Automation & Scale
8.1 When not to automate
8.2 Automation business case
8.3 Semi-automation
8.4 Robotics/cobots
8.5 Machine vision
8.6 Automated inspection/test
8.7 End-of-line systems
8.8 Automation qualification
8.9 OEE / maintenance / spare strategy
8.10 Scaling without automating defects

## 9. Manufacturing Data Hub / Manufacturing Atlas
9.1 Manufacturing ontology
9.2 ISA-95 / IEC 62264 hierarchy alignment
9.3 Equipment/resource model
9.4 Material and product genealogy
9.5 Process/recipe/version model
9.6 Parameter and measurement model
9.7 Historical metadata/effective dates
9.8 Claims/evidence/standards graph
9.9 Manufacturing-process Atlas
9.10 Decision-engine interfaces
9.11 PLM/ERP/MES/QMS/SCADA/historian boundaries
9.12 OPC UA / semantic integration boundary
9.13 Data ownership and authoritative-source model
9.14 Dashboards / analytics / AI interfaces
9.15 Security/permissions/auditability

## 10. Case Studies & Podcast Synthesis
10.1 Hardware launch failures
10.2 Successful industrialization patterns
10.3 Startup manufacturing debt
10.4 Automotive lessons
10.5 Medical-device lessons
10.6 Aerospace lessons
10.7 Industrial-equipment lessons
10.8 Cross-domain decision stories
10.9 Episode research packs
10.10 Show-note source packs

# Universal Domain Template
Every manufacturing-process domain should eventually contain:
1. Principle / physics
2. Process families and boundaries
3. Materials
4. Geometry/design rules
5. Tooling/equipment
6. Process variables
7. Defects/failure modes
8. Inspection/metrology
9. Quality/qualification/traceability
10. Automation
11. Economics / cost per good part
12. Decision objects / process selection
13. Standards/source map
14. Claims/evidence registry
15. Case studies
16. Top questions
17. Common mistakes/myths
18. Lessons learned
19. Cross-domain links
20. Quality Gate / Podcast readiness

# Roadmap Rules
1. This file is the canonical numbering authority.
2. Do not create or renumber a numbered domain without updating this file first.
3. Existing domain numbers 3.2–3.11 are frozen.
4. 3.12 Surface Engineering & Finishing is the next manufacturing-process domain.
5. A domain can be Architecture CLOSED while Knowledge Population and Evidence Verification remain OPEN.
6. Podcast Ready requires evidence verification; architecture completion alone is insufficient.
7. Quantitative rules must retain scope/applicability; do not universalize supplier data or process heuristics.
8. AI-created synthesis remains GNR until evidence-linked.
9. Cross-domain topics should have one authoritative home and links elsewhere rather than duplicate conflicting guidance.
10. The Manufacturing Atlas is a decision/navigation layer over the knowledge domains, not a replacement for them.
