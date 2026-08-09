# Early Hardware Development — Evidence Source Map

status: IN PROGRESS
campaign: A0 / Opening Arc A1–A8
podcast_leverage: Opening Arc + Episodes 1–10
provenance: primary-source-first

## Purpose
Build the evidence backbone for the new podcast opening arc: Idea -> Requirements -> Architecture -> POC -> Integrated Prototype -> Engineering Prototype -> Production Intent.

The objective is not to impose aerospace process on startups. NASA material is used here as a strong primary reference for engineering concepts; applicability to commercial/startup hardware must be stated explicitly and supplemented with broader industrial evidence.

## Primary source backbone captured

### NASA Systems Engineering Handbook
Use for:
- stakeholder needs and technical requirements
- system architecture
- interface definition
- design tradeoffs
- product verification and validation
- technical management across lifecycle
Applicability: strong conceptual systems-engineering reference; NASA-specific implementation details are not automatically startup requirements.

### NASA SE Handbook — Appendix / V&V material
Use for:
- requirements verification matrix
- validation planning
- verification methods: analysis, inspection, demonstration, test
- test-article pedigree
- developmental/engineering-unit evaluation versus formal verification/qualification/acceptance
Key relevance: test article type/pedigree and intended inference should be explicit.

### NASA TRL definitions
Use for:
- POC/prototype maturity distinctions
- relevant/operational environment progression
- demonstrating why functional prototype maturity alone does not define manufacturing maturity
Applicability boundary: TRL is technology maturity, not a complete product-development or manufacturing-readiness model.

### NASA Configuration Management guidance
Use for:
- configuration identification
- baseline/change control
- distinguishing versions
- keeping product and product information consistent
Key relevance to opening arc: configuration discipline should begin before production; waiting until industrialization loses learning and makes prototype comparisons unreliable.

### Espressif Hardware Design Guidelines
Source family: official ESP Hardware Design Guidelines and reference designs.
Use for:
- schematic/PCB design discipline
- power, grounding, RF, crystal and layout constraints
- reference-design use
- end-product RF verification
- design-specific checklist thinking
Applicability: device/vendor specific, but strong commercial evidence that serious embedded product development requires structured schematic/layout review and end-product verification rather than only functional bring-up.

### Texas Instruments custom-board design/checklist guidance
Source family: TI official custom-board schematic/design guidelines and review checklists for Sitara/SimpleLink families.
Use for:
- structured schematic self-review before layout/build
- companion use of datasheet, TRM, errata and application notes
- reducing design errors that increase bring-up/test time
- review evidence and checklist-based discipline
Applicability: processor-family specific; transferable principle is that vendor guidance, design review and pre-build checklist activity are part of robust commercial hardware development.

### Microchip Hardware Design Checklists
Source family: official Microchip hardware-design considerations/checklists and reference design resources.
Use for:
- schematic and layout checklists
- power sequencing/decoupling
- grounding/stack-up/high-speed constraints
- manufacturing constraints
- design-review service/reference designs
Applicability: device/application specific; strong corroboration for early design review and manufacture-aware PCB decisions.

## Opening Arc claim register

### C-EHD-001 — Requirements and architecture should precede uncontrolled component-level optimization
status: STRONG CONCEPTUAL SUPPORT / applicability expansion needed
Evidence basis: NASA SE assigns system engineers responsibility for architecture, requirements allocation, interfaces and tradeoffs as the system evolves from concept to product.
Podcast use: A1–A3.

### C-EHD-002 — Verification and validation are different engineering questions
status: STRONG
Verification establishes compliance with specified requirements; validation establishes that the system satisfies stakeholder/customer expectations in intended use/context.
Podcast use: A1, A7 and later DVT/PVT discussion.

### C-EHD-003 — Test-article pedigree determines what evidence can legitimately be inferred
status: STRONG
Evidence basis: NASA V&V planning distinguishes breadboards, prototypes, engineering units, qualification units and operational/final units and asks what activities apply to each.
Podcast use: A4–A7 and Prototype Representativeness framework.

### C-EHD-004 — A functional prototype is not equivalent to a production-ready product
status: STRONG when combined with existing Product Readiness evidence package
Evidence basis: TRL prototype progression addresses technology demonstration; production-readiness evidence requires additional manufacturing/process/supply/test controls.
Podcast use: bridge from A8 to Episode 1.

### C-EHD-005 — Configuration management has value before production
status: STRONG CONCEPTUAL SUPPORT
Evidence basis: NASA describes CM as maintaining true product representation, distinguishing versions, controlling changes and keeping product/documentation consistent across design, fabrication, test, integration and operation.
Podcast use: A8.

### C-EHD-006 — Early prototype technology choices can create downstream manufacturing debt
status: GNR SYNTHESIS
Rationale: highly plausible and central to podcast thesis, but needs broader empirical/industrial evidence before being presented as a general factual claim.
Podcast use: A4–A6.

### C-EHD-007 — Hardware teams should plan verification approach while defining requirements
status: STRONG
Evidence basis: NASA V&V guidance recommends identifying verification approach while developing requirements and uses requirement-verification matrices.
Podcast use: A1, A3, A7.

### C-EHD-008 — System interfaces deserve explicit ownership and verification
status: MODERATE/STRONG CONCEPTUAL SUPPORT
Evidence basis: NASA SE identifies interface definition/assessment as a core systems-engineering responsibility; broader industrial corroboration still needed for startup-oriented prescriptive guidance.
Podcast use: A2–A3.

### C-EHD-009 — Commercial embedded-hardware development benefits from pre-build schematic/layout review against vendor constraints
status: STRONG, product-family-scoped
Evidence basis: Espressif, TI and Microchip all publish official design guides, schematic/layout checklists, reference designs and/or review workflows intended to reduce design errors and improve successful product integration.
Podcast use: A6.
Applicability boundary: evidence supports the principle of disciplined board review; exact checklist items are component/vendor specific.

### C-EHD-010 — A development board/reference design does not remove the need to verify the final end-product implementation
status: STRONG, product-family-scoped
Evidence basis: Espressif explicitly requires consideration/testing of the final product context for RF/antenna behavior; vendor reference designs are implementation aids, not blanket proof of the final enclosure/PCB/system performance.
Podcast use: A4, A6, A7.

### C-EHD-011 — PCB manufacturing constraints belong in design review, not only after layout is complete
status: MODERATE/STRONG
Evidence basis: Microchip hardware design considerations explicitly include manufacturing constraints in layout/design checklists; commercial semiconductor vendors commonly embed layout, stack-up, via, grounding and assembly-sensitive constraints in design guidance.
Podcast use: A6 and bridge to DFM.

## DEV / LVP / SVP interpretation for Opening Arc
### DEV
- lightweight requirements and interface ownership
- explicit prototype purpose
- capture BOM/firmware/mechanical revision per build
- schematic/layout checklist before fabrication
- test plan tied to critical requirements

### LVP
- move from ad-hoc prototype build to released repeatable configuration
- controlled component alternates
- board fabrication/assembly constraints and test access become explicit
- serial/lot identity and failure history become valuable
- fixture/test repeatability matters even if assembly is manual

### SVP
- approved production component sources/alternates
- controlled PCB fab/assembly specification
- manufacturing test coverage and measurement capability
- configuration/effectivity discipline
- regulatory, reliability and supplier evidence as required by product class

## Evidence gaps for Pass 1
1. Commercial/startup hardware development references that address team/process scaling directly.
2. Lightweight configuration-management patterns appropriate to teams of 2–20 people.
3. Mechanical prototype-to-production transition case studies.
4. Empirical evidence around late requirement/interface changes and rework cost.
5. Prototype fidelity/representativeness literature beyond aerospace.
6. Regulatory/product-safety discovery timing by product class.
7. Embedded firmware release/configuration evidence linked to physical hardware revisions.

## Pass-2 depth targets
- quantify evidence for late changes/rework and manufacturing debt
- investigate electronics DFM/DFT and PCB assembly standards/guidance
- build a practical minimum configuration package for prototype teams
- obtain case studies where prototype assumptions failed at low-volume build
- separate vendor-specific layout rules from transferable engineering principles

## Editorial boundary
The Opening Arc should teach minimum useful engineering discipline, not transplant a large-enterprise stage-gate bureaucracy into a startup. Every practice should be presented with a scaling question: what is the lightest implementation that preserves the engineering intent at DEV, LVP and SVP?