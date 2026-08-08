# Podcast Map

status: CANONICAL PODCAST ROADMAP
version: 1.1
aligned_with: MASTER_WBS.md v1.0

## 1. Purpose

The podcast is the primary published product built from the Hardware-to-Production Data Hub.

The Data Hub is the research and evidence system.
The Podcast Map is the editorial/learning sequence.
The MASTER_WBS is the canonical knowledge-development roadmap and numbering authority.

These three structures are related but are not required to share the same numbering.

## 2. Working premise

A working hardware product is not yet a production-ready product.

The podcast explains the engineering, manufacturing, quality, supply-chain, operational, data and organizational changes required to move from development hardware to repeatable, scalable production.

## 3. Audience

### Primary
- Hardware development engineers
- NPI and industrialization engineers
- Manufacturing and process engineers
- Technical founders and engineering managers

### Secondary
- Quality, reliability and test engineers
- Supply-chain and operations teams
- Product managers working with physical products
- Automation and manufacturing-data engineers
- Students transitioning into industrial hardware roles

## 4. Editorial rules

1. Episode order is optimized for understanding, not for Data Hub domain numbering.
2. Every episode must map back to one or more MASTER_WBS domains.
3. Podcast claims must come from verified Data Hub claims or be visibly identified as unresolved/GNR during research.
4. Architecture-complete Data Hub domains are not automatically Podcast Ready.
5. Podcast Ready requires evidence verification, standards/applicability review and editorial synthesis.
6. Manufacturing processes should be explained through decisions, trade-offs and failure modes rather than encyclopedic process lists.
7. Cross-domain concepts should reuse the authoritative Data Hub object rather than create duplicate podcast-specific engineering truth.

# 5. Proposed Season Architecture

## Part I — Understanding the Gap

### Episode 1 — The product works. Why can’t we manufacture it?
Maps to MASTER_WBS: 1.1, 1.4, 1.5

Core questions:
- What separates a functional prototype from a production-ready product?
- Why can one successful build prove very little about manufacturing readiness?
- What is manufacturing debt?

### Episode 2 — POC, Prototype, MVP and Production-Intent Hardware
Maps to: 1.1, 1.6, 2.7

### Episode 3 — What NPI and Industrialization Actually Own
Maps to: 1.3, 4, 5

### Episode 4 — Product Readiness vs Manufacturing Readiness
Maps to: 1.4, 1.5, 1.6

Anchor framework introduced:
**Hardware Manufacturing Readiness Matrix**

---

## Part II — Designing for Production

### Episode 5 — EVT, DVT, PVT, Pilot and Ramp Without the Buzzwords
Maps to: 1.2, 5

### Episode 6 — Design for Manufacturing: Designing for a Process, Not a CAD Model
Maps to: 2.1, 2.5, 2.7, 3.0

This episode introduces the manufacturing-process decision framework rather than teaching every process in one episode.

### Episode 7 — Design for Assembly and Mistake Prevention
Maps to: 2.2, 3.5, 4.3, 4.4, 4.11

### Episode 8 — Design for Test, Calibration and Traceability
Maps to: 2.3, 4.8, 6.7, 9.4–9.8

### Episode 9 — Tolerance, GD&T, Variation and Why One Good Prototype Proves Little
Maps to: 2.4, 3.0.4, 4.9, 6.3, 6.4

### Episode 10 — Designing for Reliability, Service and Repair
Maps to: 2.6, 6.6

---

# Part III — Manufacturing Processes: How the Part Should Actually Be Made

This part is intentionally decision-oriented. The Data Hub contains the deep process encyclopedia; the podcast teaches how to choose and reason about the processes.

## Episode 11 — How to Select a Manufacturing Process
Maps to: 3.0, 3.1

Decision dimensions:
- function
- material
- geometry
- tolerance
- surface
- volume
- tooling/NRE
- process capability/yield
- inspection/qualification
- automation
- supplier maturity
- cost per good part

## Episode 12 — Polymer Parts: Injection Molding and the Alternatives
Maps to: 3.2, 3.7, 3.9 boundary where relevant

Coverage:
- injection molding
- extrusion
- blow molding
- thermoforming
- rotational molding
- compression/transfer/RIM
- when machining or AM may still be better

## Episode 13 — Metal Parts: Casting, Forming or Machining?
Maps to: 3.3, 3.4, 3.6

Coverage:
- casting families
- forging/forming/extrusion
- machining/material removal
- near-net + finish machining

## Episode 14 — Joining: Welding, Adhesives, Brazing, Soldering and Fasteners
Maps to: 3.5

Coverage:
- joint requirements
- serviceability
- load path
- inspection
- qualification
- process monitoring
- repair

## Episode 15 — Composite Manufacturing
Maps to: 3.8

## Episode 16 — Ceramics, Powder Processing and Sintering
Maps to: 3.10

## Episode 17 — Additive Manufacturing: When It Creates Value and When It Does Not
Maps to: 3.11

Includes explicit decision object:
**When should we NOT use additive manufacturing?**

## Episode 18 — Surface Engineering, Cleaning and Heat Treatment
Maps to: 3.12, 3.13, 3.14

Coverage:
- finishing/coatings
- corrosion protection
- cleanliness/contamination
- thermal processing
- surface/material state as part of production definition

## Episode 19 — Manufacturing Process Chains: The Sequence Is Part of the Design
Maps to: 3.15

Coverage:
- near-net + machining
- forming + heat treatment + machining
- joining + coating
- cleaning before joining/coating
- AM + post-processing
- datum migration
- cumulative distortion
- process-chain yield and economics

---

# Part IV — Building the Production System

## Episode 20 — From EBOM to MBOM and Process Flow
Maps to: 4.1, 4.2

## Episode 21 — Tooling, Jigs, Fixtures and Production-Intent Equipment
Maps to: 4.3

## Episode 22 — Work Instructions, Standard Work and Operator Qualification
Maps to: 4.4, 4.5, 4.6

## Episode 23 — DFMEA, PFMEA, Control Plans and Quality Gates
Maps to: 4.7, 6.1

## Episode 24 — Production Testing and Measurement-System Capability
Maps to: 4.8, 4.9, 6.2, 6.3

## Episode 25 — Layout, Material Flow and Ergonomics
Maps to: 4.10, 4.11

---

# Part V — Pilot and Ramp

## Episode 26 — How to Plan a Pilot Build
Maps to: 5.1

## Episode 27 — What a Production Validation Build Must Prove
Maps to: 5.2, 5.10

## Episode 28 — Yield, Rework, Scrap and the Learning Curve
Maps to: 5.3, 5.4, 5.5

## Episode 29 — Capacity, Bottlenecks, Takt Time and Line Balance
Maps to: 5.6, 5.7

## Episode 30 — Supplier Readiness and Contract-Manufacturer Management
Maps to: 5.8, 7

## Episode 31 — Engineering Changes During Ramp-Up
Maps to: 5.9, 7.9

---

# Part VI — Quality, Reliability and Compliance

## Episode 32 — Process Capability, SPC and Knowing Whether Production Is Stable
Maps to: 6.3, 6.4

## Episode 33 — Nonconformance, MRB, CAPA and Learning from Failure
Maps to: 6.5

## Episode 34 — Reliability Validation and Production Reality
Maps to: 6.6

## Episode 35 — Traceability, Genealogy and Evidence Retention
Maps to: 6.7, 6.9, 9.4–9.8

## Episode 36 — Standards, Regulatory Requirements and Applicability
Maps to: 6.8 and Knowledge OS evidence model

---

# Part VII — Supply Chain and Supplier Industrialization

## Episode 37 — Make or Buy?
Maps to: 7.1

## Episode 38 — Selecting a Supplier by Capability, Not by Sales Deck
Maps to: 7.2, 7.3

## Episode 39 — Building the RFQ Technical Package and Approving First Production
Maps to: 7.4, 7.5

## Episode 40 — Supplier Quality, Dual Sourcing and Resilience
Maps to: 7.6, 7.8

---

# Part VIII — Automation and Scale

## Episode 41 — When Not to Automate
Maps to: 8.1

## Episode 42 — Building the Business Case for Automation
Maps to: 8.2

## Episode 43 — Semi-Automation, Robotics and Machine Vision
Maps to: 8.3, 8.4, 8.5

## Episode 44 — Automated Inspection and End-of-Line Test
Maps to: 8.6, 8.7

## Episode 45 — Automation Qualification, OEE and Maintenance
Maps to: 8.8, 8.9

## Episode 46 — Scaling Without Automating Defects
Maps to: 8.10

---

# Part IX — Manufacturing Data and the Digital Thread

## Episode 47 — What PLM, ERP, MES, QMS, SCADA and Historians Actually Do
Maps to: 9.11

## Episode 48 — Product Genealogy, Recipes, Parameters and Measurements
Maps to: 9.3–9.7

## Episode 49 — Standards, Claims and Evidence as a Manufacturing Knowledge Graph
Maps to: 9.8

## Episode 50 — The Manufacturing Atlas: Turning Knowledge into Decisions
Maps to: 9.9, 9.10

## Episode 51 — OPC UA, ISA-95 and Semantic Integration Without the Buzzwords
Maps to: 9.2, 9.12

## Episode 52 — Manufacturing Data Engineers Can Actually Use
Maps to: 9.13, 9.14, 9.15

---

# Part X — Case Studies and Synthesis

## Episode 53 — Hardware Launch Failures and What Was Missed
Maps to: 10.1

## Episode 54 — Successful Industrialization Patterns
Maps to: 10.2

## Episode 55 — Startup Constraints: Speed Without Manufacturing Debt
Maps to: 10.3

## Episode 56 — Lessons from Automotive Manufacturing
Maps to: 10.4

## Episode 57 — Lessons from Medical-Device Manufacturing
Maps to: 10.5

## Episode 58 — Lessons from Aerospace Manufacturing
Maps to: 10.6

## Episode 59 — Lessons from Industrial Equipment
Maps to: 10.7

## Episode 60 — From Prototype to Production: The Full Decision Story
Maps to: 10.8 and cross-domain synthesis

# 6. Episode Research Brief

Every episode should eventually contain:

1. Practical problem
2. Representative failure scenario
3. Definitions and boundaries
4. What changes between development and production
5. Roles and ownership
6. Required deliverables
7. Decision criteria
8. Applicable standards and evidence
9. Common failure modes
10. Practical checklist
11. Decision objects / frameworks
12. Open questions and knowledge conflicts
13. Guest profile and interview questions
14. Sources for show notes
15. Cross-links to other episodes

# 7. Podcast Readiness Gate

An episode is not Podcast Ready until:

- relevant Data Hub domains are identified;
- core Claims are evidence-linked;
- standards carry revision and applicability;
- unresolved conflicts are visible;
- GNR synthesis is identified and verified or intentionally retained as hypothesis;
- practical decisions and trade-offs are represented;
- representative case studies are available;
- common mistakes/myths are supported or clearly labeled;
- source pack is complete enough for show notes and technical review.

# 8. Research-to-Episode Workflow

`Question → Data Hub Objects → Claims → Evidence → Standards/Conflicts → Decision Framework → Case Study → Episode Research Pack → Technical Review → Script/Recording → Show Notes`

# 9. Anchor Frameworks

The podcast will progressively build and reuse the following cross-episode frameworks:

1. Hardware Manufacturing Readiness Matrix
2. Manufacturing Process Selection Framework
3. Prototype-to-Production Representativeness Check
4. Joint/Assembly Selection Framework
5. Control Plan / Process Qualification Logic
6. Pilot & Production Validation Exit Criteria
7. Supplier Capability Assessment Framework
8. Automation Business-Case Framework
9. Manufacturing Data / Genealogy Model
10. Manufacturing Atlas decision layer

# 10. Governance

1. MASTER_WBS.md is the canonical knowledge-development and numbering roadmap.
2. PODCAST_MAP.md is the canonical editorial roadmap.
3. Changes to Data Hub numbering happen in MASTER_WBS first.
4. Changes to episode sequence happen here and do not automatically renumber the Data Hub.
5. Every new episode must map to existing MASTER_WBS domains or explicitly identify a WBS gap before publication.
6. Deep process content lives in the Data Hub; podcast episodes synthesize and teach decisions rather than duplicate the encyclopedia.
