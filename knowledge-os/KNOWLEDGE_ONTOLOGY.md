# Hardware to Production Knowledge Ontology

**Baseline: v1.0**

## 1. Purpose

This ontology defines the stable high-level knowledge architecture used by the Knowledge OS. It is intentionally broader than the podcast episode list.

The stable hierarchy is:

**Knowledge Layer → Domain → Module → Knowledge Object**

Questions drive research and navigation. Claims carry evidence. Decisions consume Claims. Sources support Claims.

## 2. Controlled Object Types

The v1.0 object vocabulary is:

- Domain
- Module
- Knowledge Object
- Engineering Decision
- Engineering Claim
- Engineering Pattern
- Engineering Principle
- Failure Mode
- Standard / Regulation
- Book / Handbook
- Paper / Academic Source
- Template / Checklist
- Case Study
- Open Question
- Engineering Assumption
- Knowledge Conflict

Adding a new top-level object type requires an ADR.

## 3. Domain 01 — Product Development

Modules:
- Systems Engineering
- Requirements Engineering
- Product Architecture
- Concept Development
- Mechanical Design
- Electrical/Electronic Design
- Embedded/Firmware Interfaces
- Industrial Design
- Design Reviews
- Configuration Management
- Product Risk

## 4. Domain 02 — Prototype Workshop

Modules:
- Prototype Strategy
- Rapid Iteration
- Workshop Architecture
- Additive Manufacturing
- CNC Machining
- Turning
- Laser Cutting
- Waterjet / Routing / Other Cutting
- Sheet Metal
- Joining & Welding
- Electronics Prototyping
- PCB Assembly & Rework
- Cable & Harness
- Jigs & Fixtures
- Metrology & Inspection
- Test Equipment
- Workshop Safety
- Maintenance & Calibration
- Inventory & Consumables
- Make vs Buy / Outsourcing

## 5. Domain 03 — Manufacturing Processes

Modules:
- Machining
- Casting
- Injection Molding
- Extrusion
- Blow Molding
- Thermoforming / Vacuum Forming
- Additive Manufacturing
- Sheet Metal Forming
- Metal Forming
- Welding & Joining
- Adhesive Bonding
- Mechanical Fastening
- Heat Treatment
- Surface Treatment
- Coating & Finishing
- Electronics Manufacturing
- Cable/Harness Manufacturing

## 6. Domain 04 — Materials Engineering

Modules:
- Metals
- Polymers
- Elastomers
- Ceramics
- Composites
- Adhesives
- Coatings
- Material Selection
- Compatibility
- Corrosion & Degradation
- Surface Engineering

## 7. Domain 05 — Design for X

Modules:
- DFM
- DFA
- DFT
- DFMA
- Design for Reliability
- Design for Serviceability
- Design for Maintainability
- Design for Automation
- Design for Cost
- Design for Supply Chain
- Design for Compliance
- Robust Design
- Modularity
- Tolerance Design
- GD&T

## 8. Domain 06 — Manufacturing Engineering

Modules:
- Process Planning
- Process Flow
- Routing
- Standard Work
- Work Instructions
- Takt & Cycle Time
- Capacity Planning
- Bottleneck Analysis
- Line Balancing
- Layout
- Workstations
- Ergonomics
- Tooling
- Fixtures
- Material Flow

## 9. Domain 07 — Quality Engineering

Modules:
- APQP
- PPAP
- DFMEA
- PFMEA
- Control Plan
- MSA
- Gauge R&R
- SPC
- Process Capability
- Sampling
- Inspection
- Qualification
- Validation
- First Article Inspection
- 8D
- CAPA
- MRB
- Nonconformance

## 10. Domain 08 — NPI & Industrialization

Modules:
- NPI Frameworks
- Manufacturing Readiness
- Design Transfer
- Phase Gates
- EVT
- DVT
- PVT
- Pilot Builds
- Golden Build / Golden Unit
- Production Readiness
- Safe Launch
- Ramp-up
- Yield Ramp
- Industrialization Ownership
- Cross-functional Handoffs

## 11. Domain 09 — Factory Design

Modules:
- Factory Layout
- Line Architecture
- Utilities
- Material Flow
- Warehouse
- Lean Factory
- Visual Management
- Clean / Controlled Environments
- Safety
- Facility Constraints

## 12. Domain 10 — Automation

Modules:
- Automation Strategy
- Automation Economics
- PLC
- HMI
- SCADA
- MES / MOM
- ERP Integration
- ISA-95 / IEC 62264
- OPC UA
- Robotics
- Cobots
- Machine Vision
- Traceability
- IIoT
- Industrial Data
- OT Cybersecurity

## 13. Domain 11 — Supply Chain

Modules:
- Sourcing
- Supplier Selection
- Supplier Qualification
- Make vs Buy
- Contract Manufacturing
- Dual Sourcing
- Purchasing
- Incoming Quality
- Inventory
- Forecast
- Logistics
- Lead Time
- MOQ
- Obsolescence
- Supply Risk

## 14. Domain 12 — Business & Manufacturing Strategy

Modules:
- Product Cost
- Should Cost
- CAPEX
- OPEX
- ROI
- Unit Economics
- Manufacturing Strategy
- Outsourcing Strategy
- Scaling Strategy
- Capacity Investment
- Cost of Poor Quality

## 15. Domain 13 — Regulations & Standards

Modules:
- Quality Management
- Machinery Safety
- Electrical Safety
- Functional Safety
- Product Compliance
- Environmental Compliance
- Industry-specific Standards
- Documentation Standards
- Metrology & Laboratory Standards

## 16. Domain 14 — Case Studies

Modules:
- Successful Industrialization
- Failed Industrialization
- Prototype-to-Production Failures
- Supplier Failures
- Quality Escapes
- Automation Success/Failure
- Ramp-up Case Studies
- Startup Hardware Case Studies

## 17. Domain 15 — Engineering Management

Modules:
- Technical Leadership
- Program Management
- Concurrent Engineering
- Stage Gates
- Change Management
- ECO / ECN
- Configuration Governance
- Cross-functional Ownership
- Decision Making
- Lessons Learned
- Knowledge Management

## 18. Cross-cutting Lifecycle Axis

Concept → POC → Prototype → Engineering Prototype → MVP → Alpha → Beta → EVT → DVT → PVT → Pilot → Bridge Production → Ramp-up → Serial / Mass Production → Sustainment → End of Life

## 19. Cross-cutting Evidence Axis

Normative Requirement → Verified Fact → Academic Evidence → Academic Consensus → Industrial Best Practice → Manufacturer Guidance → Expert Opinion → Project Synthesis / Heuristic

## 20. Cross-cutting Provenance Axis

AI-originated content retains `GNR` provenance permanently, even after external verification. Additional source provenance is accumulated rather than replacing origin metadata.

## 21. Cross-cutting Question Axis

Every Domain and major Module maintains `Questions Answered`. Questions are not hierarchy nodes; they are navigation and research entry points that map to Decisions, Claims and Objects.

## 22. Cross-cutting Uncertainty Axis

Uncertainty is explicitly represented using:

- Open Questions
- Engineering Assumptions
- Knowledge Conflicts

Unknown or conflicting knowledge must not be hidden inside prose.

## 23. Cross-cutting Relationship Axis

All entity-to-entity links must use controlled types from `RELATIONSHIP_MODEL.md` and include context/evidence where the relationship makes a technical, normative or causal claim.

## 24. Governance

Changes to top-level Domains, hierarchy levels or object types require an ADR. Adding new Modules or Objects inside the existing ontology does not normally require an ADR.

Knowledge OS v1.0 is the architecture baseline. Content growth should occur within this model rather than continually extending it.