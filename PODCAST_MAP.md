# Podcast Map

status: CANONICAL PODCAST ROADMAP
version: 2.0
aligned_with: MASTER_WBS.md v1.0
editorial_model: Hardware Evolution Journey

## 1. Purpose

The podcast is the primary published product built from the Hardware-to-Production Data Hub.

The Data Hub is the research and evidence system.
The Podcast Map is the editorial/learning sequence.
The MASTER_WBS is the canonical knowledge-development roadmap and numbering authority.

These three structures are related but are not required to share the same numbering.

The podcast is intended to guide a hardware team across the full journey from early development to commercial production, not only explain industrialization after a prototype already works.

## 2. Audience and mission

### Primary audience A — Founders and early hardware development teams
Teams that may still be defining architecture, building first prototypes or deciding how mechanical, electronics, embedded, test and manufacturing choices fit together.

The podcast should help them understand:
- which engineering disciplines and responsibilities are needed;
- what should be solved now versus deferred;
- which prototype shortcuts are legitimate;
- which shortcuts create manufacturing debt;
- what must change before producing tens or hundreds of units;
- what commercial production will eventually require so they can avoid designing themselves into a corner.

### Primary audience B — Early production / industrialization teams
Teams that have a first working prototype and are now:
- upgrading prototype components into industrial/production-intent components;
- moving from bench assembly into repeatable low-volume production;
- building tens or hundreds of units manually or semi-automatically;
- introducing suppliers, tooling, test, quality, documentation and traceability;
- preparing for scalable commercial production.

### Secondary audience
- NPI and industrialization engineers
- manufacturing and process engineers
- quality, reliability and test engineers
- technical founders and engineering managers
- supply-chain and operations teams
- product managers working with physical products
- automation and manufacturing-data engineers
- students transitioning into industrial hardware roles

## 3. Working premise

A working hardware product is not yet a production-ready product.

More importantly, decisions made before the first prototype can determine whether the product will later be manufacturable, testable, serviceable and economically scalable.

The podcast therefore follows the product through three practical production contexts:

### DEV — Development / Prototype
Goal: learn, prove function, reduce technical uncertainty and expose integration problems quickly.

### LVP — Low-Volume Production
Typical context: tens to hundreds of units, often manual or semi-automated, with increasing process discipline but limited justification for full automation or high-NRE tooling.

### SVP — Serial / Commercial Production
Goal: repeatable, capable, traceable, economically sustainable production at commercial scale with controlled suppliers, process, quality, change and lifecycle support.

DEV / LVP / SVP are internal podcast lenses, not claimed industry-standard lifecycle terms.

## 4. Hardware Evolution Ladder

The recurring journey framework is:

`Idea → Requirements → Architecture → POC → Integrated Prototype → Engineering Prototype → Production-Intent Hardware → LVP → Production Validation → Ramp → SVP`

At every major transition the podcast evaluates at least:
- design/configuration maturity;
- material and component maturity;
- BOM and supplier maturity;
- manufacturing process maturity;
- tooling/fixture/equipment maturity;
- assembly method;
- test/calibration strategy;
- quality controls and measurement capability;
- documentation/configuration control;
- traceability/genealogy;
- reliability/serviceability;
- cost/volume economics;
- exit evidence required to justify the next step.

## 5. Recurring five-question lens

Every technical episode should explicitly answer, where relevant:

1. What should the team do now during DEV?
2. What is acceptable as a prototype shortcut but dangerous to carry forward?
3. What changes when producing tens or hundreds of units in LVP?
4. What must change before SVP / commercial serial production?
5. What should be designed or documented today to avoid manufacturing debt later?

This lens is mandatory editorial structure, not optional commentary.

## 6. Editorial rules

1. Episode order is optimized for the hardware journey, not Data Hub domain numbering.
2. Every episode must map back to one or more MASTER_WBS domains or explicitly identify a knowledge gap.
3. Podcast claims must come from verified Data Hub claims or be visibly identified as unresolved/GNR during research.
4. Architecture-complete Data Hub domains are not automatically Podcast Ready.
5. Podcast Ready requires evidence verification, standards/applicability review and editorial synthesis.
6. Manufacturing processes should be explained through decisions, trade-offs and failure modes rather than encyclopedic process lists.
7. Cross-domain concepts should reuse the authoritative Data Hub object rather than create duplicate podcast-specific engineering truth.
8. DEV/LVP/SVP distinctions must be used when advice changes materially with production maturity.
9. Prototype shortcuts should be presented with an explicit expiration condition or risk where practical.
10. Episodes should tell the listener not only what exists, but what they will need next and why.

# 7. Opening Arc — Before the Product Works

The Opening Arc is deliberately placed before the original industrialization journey. It closes the gap for founders and early development teams without renumbering the original 60-episode roadmap.

## Opening Episode A1 — From an Idea to Engineering Requirements
Maps primarily to: 1, 2 and requirements interfaces across the WBS.

Core questions:
- What problem are we solving and what must the hardware actually do?
- Which requirements are functional, environmental, safety, regulatory, manufacturing or service related?
- Which assumptions should be made explicit before CAD or PCB work accelerates?
- What does “good enough for the first prototype” actually mean?

DEV focus: build the smallest useful requirement set that prevents random engineering.
LVP horizon: identify requirements that will later affect suppliers, inspection and process control.
SVP horizon: recognize requirements that will become CTQs, compliance evidence or production limits.

## Opening Episode A2 — The Hardware Team Map: Who Owns What?
Maps to: 1.3 plus cross-domain ownership throughout 2–9.

Coverage:
- systems/product engineering
- mechanical
- electronics/PCB
- embedded/firmware/software boundary
- test
- manufacturing/NPI
- quality/reliability
- supply chain
- regulatory/safety boundary

Core question: which responsibilities can one startup engineer temporarily combine, and which responsibilities must never disappear?

## Opening Episode A3 — System Architecture and Interfaces Before Detailed Design
Maps to: 2 and cross-domain architecture decisions.

Coverage:
- subsystem boundaries
- mechanical/electrical/fluid/thermal/software interfaces
- connector and service interfaces
- power/data paths
- load paths
- environmental boundaries
- interface ownership

Key lesson: integration failures often originate at interfaces owned by nobody.

## Opening Episode A4 — Choosing Prototype Technologies Without Trapping the Product
Maps to: 1.1, 1.6, 2.7, 3.0, Prototype Workshop knowledge.

Coverage:
- COTS versus custom
- breadboards/dev boards
- 3D printing
- CNC prototype parts
- soft/bridge tooling
- temporary wiring/connectors
- lab fixtures
- outsourced prototype fabrication
- knowing what evidence transfers to production and what does not

Anchor framework: Prototype-to-Production Representativeness Check.

## Opening Episode A5 — Mechanical Design for the First Serious Prototype
Maps to: 2.1, 2.2, 2.4, 2.5, 2.6 and relevant Section 3 process domains.

Coverage:
- architecture before detail
- loads and interfaces
- materials
- fastening/joining choices
- tolerances
- access
- thermal/environmental considerations
- what can be crude in DEV and what should already reflect intended production logic

## Opening Episode A6 — Electronics, PCB and Embedded Hardware for the First Serious Prototype
Maps to: DFT/traceability/configuration aspects of Sections 2, 4, 6 and 9; detailed electronics-manufacturing expansion may require future Data Hub enrichment.

Coverage:
- dev board versus custom PCB
- power architecture
- connectors and harnesses
- sensors/actuators
- programming/debug access
- test points
- component lifecycle/availability
- firmware/configuration identity
- what changes for tens/hundreds and then serial production

Editorial note: if evidence population reveals insufficient electronics-manufacturing depth in MASTER_WBS V1.0, create a controlled V1.x gap decision rather than inventing unsupported coverage.

## Opening Episode A7 — Development Verification Before Production Verification
Maps to: 1, 2.3, 2.6, 4.8, 6.6.

Coverage:
- proving function
- abuse/boundary testing
- environmental and load testing
- debugging instrumentation
- test fixtures during development
- separating engineering validation from production acceptance testing
- learning what should eventually become automated or controlled

## Opening Episode A8 — Configuration Management from Prototype #1
Maps to: 1.6, 6.7, 9.4–9.7.

Coverage:
- prototype IDs
- BOM revision
- PCB/firmware/mechanical revision
- test result linkage
- supplier/component substitution
- build notes
- why “we know what changed” stops working surprisingly early

Key lesson: lightweight configuration discipline in DEV is cheaper than reconstructing history after failures appear.

---

# 8. Core Journey — From Working Product to Commercial Production

## Part I — Understanding the Gap

### Episode 1 — The product works. Why can’t we manufacture it?
Maps to MASTER_WBS: 1.1, 1.4, 1.5

Core questions:
- What separates a functional prototype from a production-ready product?
- Why can one successful build prove very little about manufacturing readiness?
- What is manufacturing debt?
- Which problems become visible only when one build becomes fifty or five thousand?

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

This part is intentionally decision-oriented. For every process family the episode must distinguish DEV, LVP and SVP routes and explain when a bridge process should be abandoned.

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
- machining/AM/urethane or bridge-process alternatives where applicable
- when low-volume economics justify staying with an alternate route
- what eventually forces the shift to serial tooling/process control

## Episode 13 — Metal Parts: Casting, Forming or Machining?
Maps to: 3.3, 3.4, 3.6

Coverage:
- casting families
- forging/forming/extrusion
- machining/material removal
- near-net + finish machining
- prototype versus low-volume versus serial route

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
- manual joining in LVP versus process qualification/automation in SVP

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

This part marks the transition from “we can build it” to “we can build it repeatedly.” LVP examples should receive explicit emphasis before SVP systems are introduced.

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

Episode 60 should explicitly replay the Hardware Evolution Ladder and show how the same product would be treated differently in DEV, LVP and SVP.

# 9. Episode Research Brief

Every episode should eventually contain:

1. Practical problem
2. Listener stage / Hardware Evolution Ladder position
3. Representative failure scenario
4. Definitions and boundaries
5. DEV approach
6. Prototype shortcuts and their expiration conditions
7. LVP approach for tens/hundreds
8. SVP / commercial-production approach
9. What should be prepared early to avoid manufacturing debt
10. Roles and ownership
11. Required deliverables
12. Decision criteria
13. Applicable standards and evidence
14. Common failure modes
15. Practical checklist
16. Decision objects / frameworks
17. Open questions and knowledge conflicts
18. Guest profile and interview questions
19. Sources for show notes
20. Cross-links to other episodes

# 10. Podcast Readiness Gate

An episode is not Podcast Ready until:

- relevant Data Hub domains are identified;
- target listener stage is explicit;
- DEV/LVP/SVP distinctions are included wherever engineering advice materially changes;
- prototype shortcuts have limits/risks where relevant;
- core Claims are evidence-linked;
- standards carry revision and applicability;
- unresolved conflicts are visible;
- GNR synthesis is identified and verified or intentionally retained as hypothesis;
- practical decisions and trade-offs are represented;
- representative case studies are available;
- common mistakes/myths are supported or clearly labeled;
- source pack is complete enough for show notes and technical review.

# 11. Research-to-Episode Workflow

`Audience/Stage → Question → Data Hub Objects → Claims → Evidence → Standards/Conflicts → DEV/LVP/SVP Comparison → Decision Framework → Case Study → Episode Research Pack → Technical Review → Script/Recording → Show Notes`

# 12. Anchor Frameworks

The podcast will progressively build and reuse the following cross-episode frameworks:

1. Hardware Evolution Ladder
2. DEV / LVP / SVP Lens
3. Hardware Manufacturing Readiness Matrix
4. Manufacturing Process Selection Framework
5. Prototype-to-Production Representativeness Check
6. Joint/Assembly Selection Framework
7. Control Plan / Process Qualification Logic
8. Pilot & Production Validation Exit Criteria
9. Supplier Capability Assessment Framework
10. Automation Business-Case Framework
11. Manufacturing Data / Genealogy Model
12. Manufacturing Atlas decision layer

# 13. Audience coverage test

Before approving a Part/episode sequence, verify that it serves at least one of the two primary audiences and does not accidentally require knowledge the target listener has not yet been given.

### Audience A test — Founder / early development team
Can the listener understand:
- what disciplines and decisions are needed now;
- what a credible next prototype should prove;
- what future manufacturing constraints should influence today's choices;
- how the design should evolve before tens/hundreds and commercial production?

### Audience B test — First-prototype / early production team
Can the listener understand:
- which prototype components/processes should be industrialized first;
- how to establish repeatable low-volume production;
- what documentation/tooling/test/quality/supplier systems are required next;
- what evidence is needed before commercial scale?

If either intended audience is assumed to know a critical concept that has not yet appeared, add a cross-reference, prelude or episode gap rather than silently assuming it.

# 14. Governance

1. MASTER_WBS.md is the canonical knowledge-development and numbering roadmap.
2. PODCAST_MAP.md is the canonical editorial roadmap.
3. Changes to Data Hub numbering happen in MASTER_WBS first.
4. Changes to episode sequence happen here and do not automatically renumber the Data Hub.
5. Opening Arc uses A1–A8 so the established 1–60 episode numbering remains stable.
6. Every new episode must map to existing MASTER_WBS domains or explicitly identify a WBS gap before publication.
7. Deep process content lives in the Data Hub; podcast episodes synthesize and teach decisions rather than duplicate the encyclopedia.
8. DEV/LVP/SVP are editorial maturity lenses, not claimed industry-standard lifecycle names.
9. If the Opening Arc exposes a genuine Data Hub coverage gap, record it through Knowledge OS governance before expanding MASTER_WBS V1.x.
