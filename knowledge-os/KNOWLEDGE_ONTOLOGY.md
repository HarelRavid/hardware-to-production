# Hardware to Production Knowledge Ontology

## Purpose

This ontology defines the stable high-level knowledge architecture used by the Knowledge OS. It is intentionally broader than the podcast episode list.

## Domain 01 — Product Development

Subdomains:
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

## Domain 02 — Prototype Workshop

Subdomains:
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

## Domain 03 — Manufacturing Processes

Subdomains:
- Machining
- Casting
- Injection Molding
- Extrusion
- Blow Molding
- Thermoforming / Vacuum Forming
- Additive Manufacturing
- Sheet Metal Forming
- Welding & Joining
- Adhesive Bonding
- Heat Treatment
- Surface Treatment
- Coating & Finishing
- Electronics Manufacturing
- Cable/Harness Manufacturing

## Domain 04 — Materials Engineering

Subdomains:
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

## Domain 05 — Design for X

Subdomains:
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

## Domain 06 — Manufacturing Engineering

Subdomains:
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

## Domain 07 — Quality Engineering

Subdomains:
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

## Domain 08 — NPI & Industrialization

Subdomains:
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

## Domain 09 — Factory Design

Subdomains:
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

## Domain 10 — Automation

Subdomains:
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

## Domain 11 — Supply Chain

Subdomains:
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

## Domain 12 — Business & Manufacturing Strategy

Subdomains:
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

## Domain 13 — Regulations & Standards

Subdomains:
- Quality Management
- Machinery Safety
- Electrical Safety
- Functional Safety
- Product Compliance
- Environmental Compliance
- Industry-specific Standards
- Documentation Standards
- Metrology & Laboratory Standards

## Domain 14 — Case Studies

Subdomains:
- Successful Industrialization
- Failed Industrialization
- Prototype-to-Production Failures
- Supplier Failures
- Quality Escapes
- Automation Success/Failure
- Ramp-up Case Studies
- Startup Hardware Case Studies

## Domain 15 — Engineering Management

Subdomains:
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

## Cross-cutting Lifecycle Axis

Concept → POC → Prototype → Engineering Prototype → MVP → Alpha → Beta → EVT → DVT → PVT → Pilot → Ramp-up → Mass Production → Sustainment → End of Life

## Cross-cutting Evidence Axis

Normative Requirement → Verified Fact → Academic Evidence → Industrial Best Practice → Expert Opinion → Project Synthesis

## Cross-cutting Relationship Axis

All object-to-object links must use controlled types from `RELATIONSHIP_MODEL.md`.

## Governance

Changes to top-level Domains or the fundamental ontology require an ADR. Adding new Topics or Objects inside an existing Subdomain does not normally require an ADR.