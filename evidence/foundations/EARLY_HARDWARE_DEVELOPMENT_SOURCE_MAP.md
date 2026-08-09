# Early Hardware Development — Evidence Source Map

status: BREADTH COMPLETE
campaign: A0 / Opening Arc A1–A8
podcast_leverage: Opening Arc + Episodes 1–10
provenance: primary-source-first

## Purpose
Build the evidence backbone for the podcast opening arc: Idea -> Requirements -> Architecture -> POC -> Integrated Prototype -> Engineering Prototype -> Production Intent.

The objective is not to impose aerospace process on startups. NASA material is used as a strong primary reference for engineering concepts; commercial, regulatory and open-source hardware evidence is used to test applicability and provide lightweight implementation patterns.

## Primary source backbone captured

### NASA Systems Engineering Handbook / V&V / TRL / Configuration Management
Use for:
- stakeholder needs and technical requirements
- system architecture and interfaces
- design tradeoffs
- verification versus validation
- verification planning while requirements are written
- test-article pedigree
- prototype/technology maturity boundaries
- configuration identification, baselines and change control
Applicability: strong conceptual systems-engineering references; NASA-specific implementation details are not automatically startup requirements.

### KiCad official documentation — project files and Git integration
Use for:
- showing a hardware-design project as a controlled multi-file object
- practical version control for schematic/PCB projects
- lightweight prototype-team history and rollback
Applicability: tooling guidance, not a normative engineering-management standard.

### GitHub official documentation — tags and releases
Use for:
- immutable/identified software and firmware states
- lightweight released-state markers
Applicability: software configuration mechanism; complete product configuration must also bind hardware/BOM/mechanical/calibration state.

### NISTIR 7922 — Engineering Change Management Concepts for Systems Modeling
Use for:
- engineering-change propagation
- revisiting previously completed decisions/tasks
- qualitative cost and complexity of late changes
Applicability: strong cross-industry systems/manufacturing reference; does not justify universal 10x/100x cost-of-change folklore.

### NIST — Conceptual Process Planning
Source: NIST publication "Conceptual Process Planning - A Definition and Functional Decomposition".
Use for:
- evaluating manufacturability and manufacturing cost during early design
- integrating conceptual design with conceptual process planning
Key relevance: direct support for introducing manufacturing thinking before design is frozen, rather than waiting for formal industrialization.

### NIST — Product Design and Development / MEP case material
Use for:
- commercial examples of idea -> prototype -> production transition
- practical manufacturing-extension support for small and medium manufacturers
Applicability: case/example evidence, not a universal lifecycle model.

### NIST — Rapid prototyping / high-speed machining literature
Use for:
- prototype process choice as an engineering decision
- distinction between prototype objectives and serial-process evidence
- rapid fabrication of functional mechanical prototypes
Applicability: some sources are older; useful for foundational distinctions, while specific technology economics require current sources.

### Commercial embedded-hardware design guidance
Source families:
- Espressif hardware design guidelines
- Texas Instruments schematic/layout/reference-design guidance
- Microchip hardware design/checklist/reference-design guidance
Use for:
- schematic review before fabrication
- PCB layout constraints
- power/decoupling/clock/reset/RF implementation
- use and limits of reference designs
- review/DRC before manufacturing release
Applicability: vendor/device-specific guidance used as commercial corroboration, not universal electronics rules.

### Zephyr Project — board revision support
Source: Zephyr board-porting documentation.
Use for:
- explicit hardware board revision identity
- revision-specific devicetree/Kconfig configuration
- software build behavior tied to board revision
Key relevance: direct primary evidence that firmware build configuration may legitimately vary by hardware revision.

### Espressif — chip revision compatibility
Use for:
- hardware revision and firmware compatibility constraints
- binary metadata defining supported hardware revisions
Key relevance: direct commercial evidence that software compatibility can depend on hardware revision and should be represented in configuration control.

### UK HSE / OPSS / GOV.UK product-safety guidance
Use for:
- applicable safety requirements affecting product design and manufacture
- conformity assessment involving design, manufacturing controls, technical documentation and testing
- traceability/labeling/instructions obligations before market placement
- evidence that regulatory/product-safety discovery can affect design choices and therefore should not be deferred until the end
Applicability: UK-specific legal implementation; podcast must translate the principle and then identify jurisdiction/product-specific requirements.

### UK product-safety policy guidance — design-stage conformity
Use for:
- explicit evidence that some product regimes require conformity-assessment activity at design stage and further verification at manufacturing stage
Key relevance: supports early regulatory discovery as an engineering planning activity, especially in higher-risk product classes.

## Opening Arc claim register

### C-EHD-001 — Requirements and architecture should precede uncontrolled component-level optimization
status: STRONG CONCEPTUAL SUPPORT
Evidence basis: NASA SE assigns architecture, requirement allocation, interfaces and tradeoffs before/while detailed design evolves.
Podcast use: A1–A3.

### C-EHD-002 — Verification and validation are different engineering questions
status: STRONG
Verification establishes compliance with specified requirements; validation establishes suitability for stakeholder/customer intended use/context.
Podcast use: A1, A7 and later DVT/PVT discussion.

### C-EHD-003 — Test-article pedigree determines what evidence can legitimately be inferred
status: STRONG
Evidence basis: NASA V&V distinguishes breadboards, prototypes, engineering units, qualification units and final/operational units.
Podcast use: A4–A7 and Prototype Representativeness framework.

### C-EHD-004 — A functional prototype is not equivalent to a production-ready product
status: STRONG
Evidence basis: technology/prototype maturity and production readiness require different evidence; existing A1 package adds manufacturing/process/supply/test readiness evidence.
Podcast use: bridge from A8 to Episode 1.

### C-EHD-005 — Configuration management has value before production
status: STRONG CONCEPTUAL + PRACTICAL SUPPORT
Evidence basis: NASA CM principles plus KiCad/Git/GitHub implementation patterns.
Podcast use: A8.

### C-EHD-006 — Early prototype technology choices can create downstream manufacturing debt
status: MODERATE SYNTHESIS — PASS-2 DEPTH TARGET
Evidence basis now includes NIST conceptual process-planning work showing manufacturability/cost should be assessed early and prototype-process literature demonstrating that prototype technologies are selected for different objectives. Direct empirical attribution of downstream redesign/cost to a specific prototype-route choice still needs stronger case evidence.
Podcast use: A4–A6.
Editorial boundary: present as a risk/mechanism with examples, not as a universal quantitative law.

### C-EHD-007 — Hardware teams should plan verification approach while defining requirements
status: STRONG
Evidence basis: NASA V&V guidance and requirement-verification matrix practices.
Podcast use: A1, A3, A7.

### C-EHD-008 — System interfaces deserve explicit ownership and verification
status: STRONG CONCEPTUAL SUPPORT
Evidence basis: NASA systems-engineering responsibility for interface definition/assessment.
Podcast use: A2–A3.

### C-EHD-009 — Lightweight version control is practical for small electronics/firmware teams
status: STRONG IMPLEMENTATION SUPPORT
Evidence basis: KiCad Git integration and GitHub identified states.
Podcast use: A8.

### C-EHD-010 — Firmware revision can be part of physical-product configuration
status: STRONG
Evidence basis: Zephyr explicitly supports board-revision-specific software configuration; Espressif binaries encode supported hardware/chip revisions and compatibility boundaries.
Podcast use: A6, A8 and later genealogy episodes.

### C-EHD-011 — Engineering changes can force previously completed decisions/work to be revisited
status: STRONG
Evidence basis: NISTIR 7922.
Podcast use: A1, A3, A8 and Episode 31.
Boundary: no universal late-change multiplier asserted.

### C-EHD-012 — A schematic/PCB project is a controlled multi-artifact configuration, not just a PCB file
status: STRONG IMPLEMENTATION SUPPORT
Evidence basis: KiCad project structure and manufacturing-output context.
Podcast use: A6, A8.

### C-EHD-013 — Manufacturing planning should begin while the product is still being designed
status: STRONG
Evidence basis: NIST conceptual process planning explicitly evaluates manufacturability and manufacturing cost in the early design stage and integrates process planning with conceptual design.
Podcast use: A3–A6 and bridge to Episode 6.

### C-EHD-014 — Regulatory/product-safety applicability should be discovered before design freeze when it can affect design, testing or documentation
status: STRONG PRINCIPLE / JURISDICTION-SPECIFIC IMPLEMENTATION
Evidence basis: UK HSE/OPSS guidance requires applicable safety requirements to be met through design/manufacture and conformity assessment may include product design, manufacturing controls, documentation and testing; some regimes explicitly include design-stage conformity assessment.
Podcast use: A1–A3 and Episode 36.

### C-EHD-015 — Hardware and firmware revision compatibility may require explicit co-configuration
status: STRONG
Evidence basis: Zephyr board-revision-specific configuration and Espressif chip-revision compatibility metadata provide direct examples.
Podcast use: A6, A8, Episodes 35/48.

## Lightweight configuration-management pattern for teams of 2–20
This is a GNR-derived implementation pattern backed by CM principles and tooling evidence; it is not presented as a standard.

Minimum DEV baseline:
1. one controlled repository/location for mechanical, electronics and firmware artifacts or explicit linked repositories;
2. unique prototype/build ID;
3. BOM/critical-component snapshot;
4. schematic/PCB/mechanical revision identity;
5. firmware commit/tag or immutable build identifier;
6. short build/change log: what changed and why;
7. test result linked to the exact unit/configuration tested.

LVP extension:
- released baseline/tag
- controlled approved substitutions
- unit/lot genealogy at risk-appropriate granularity
- rework/deviation record
- manufacturing/test files tied to release revision
- explicit hardware/firmware compatibility matrix where required

SVP extension:
- formal PLM/MES/QMS/effectivity model where justified
- supplier and production-process revisions
- serialized/lot genealogy
- controlled software deployment/calibration configuration

## Prototype representativeness synthesis
Prototype evidence should be classified by what it actually represents:
- geometry
- material
- manufacturing process
- surface/finish
- joining/assembly
- electronics/PCB implementation
- firmware/hardware compatibility
- environment/load
- variation
- supplier/tooling
- production rate

Evidence from NASA test-article pedigree plus NIST rapid-prototyping/process-planning sources supports treating representativeness as multidimensional rather than binary. The exact representativeness vector remains an internal framework and should be labeled as synthesis.

## A0 Breadth Completion Assessment
The campaign has now captured:
1. authoritative source families — YES;
2. episode-critical claims — YES;
3. weak/GNR claims — YES, especially prototype-route -> manufacturing-debt causality;
4. applicability conflicts/boundaries — YES, including NASA versus startup and UK regulation versus other jurisdictions;
5. Pass-2 depth targets — YES.

Status: BREADTH COMPLETE.

## Pass-2 depth targets
- collect stronger commercial mechanical case studies where prototype process masked serial-process constraints;
- quantify/document engineering-change propagation and cost without folklore multipliers;
- build PCB/PCBA transition pack: DFM, panelization, assembly, test, component lifecycle and change control;
- define product-configuration object linking hardware revision, BOM, firmware, calibration and test evidence;
- compare lightweight Git-based DEV configuration control with PLM-level LVP/SVP needs;
- build jurisdiction/product-class regulatory discovery matrix for common startup hardware categories.

## Editorial boundary
The Opening Arc should teach minimum useful engineering discipline, not transplant a large-enterprise stage-gate bureaucracy into a startup. Every practice should be presented with a scaling question: what is the lightest implementation that preserves the engineering intent at DEV, LVP and SVP?