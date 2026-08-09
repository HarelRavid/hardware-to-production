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
Key relevance: provides evidence that test article type/pedigree and intended inference should be explicit.

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

### KiCad official documentation — project files and Git integration
Sources:
- https://docs.kicad.org/9.0/en/getting_started_in_kicad/getting_started_in_kicad.html
- https://docs.kicad.org/9.0/en/kicad/kicad.html
Use for:
- showing that even mainstream electronics design tooling treats the project as a multi-file controlled object
- identifying project/schematic/PCB/manufacturing-output artifacts
- practical version-control implementation using Git
- lightweight prototype-team configuration history
Applicability: tooling guidance, not a normative engineering-management standard.

### GitHub official documentation — tags and releases
Sources:
- https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases
- https://docs.github.com/en/repositories/releasing-projects-on-github/viewing-your-repositorys-releases-and-tags
Use for:
- lightweight implementation pattern for identifying known-good software/firmware/configuration states
- showing that tags can identify a specific point in repository history
Applicability: software configuration mechanism; when used for hardware programs it must be linked to hardware/BOM/PCB/mechanical configuration rather than treated as complete product CM by itself.

### NISTIR 7922 — Engineering Change Management Concepts for Systems Modeling
Source:
- https://www.nist.gov/publications/engineering-change-management-concepts-systems-modeling
Use for:
- engineering-change management rationale
- cost and complexity created when system specifications change after build/delivery
- revisiting previously completed engineering decisions/tasks after change
Applicability: strong cross-industry systems/manufacturing reference; not a quantitative universal late-change cost curve.

### Commercial embedded-hardware design guidance
Source families captured in A0 research:
- Espressif hardware design guidelines
- Texas Instruments schematic/layout/reference-design guidance
- Microchip hardware design/checklist/reference-design guidance
Use for:
- schematic review before fabrication
- PCB layout constraints
- power/decoupling/clock/reset/RF implementation guidance
- use and limits of reference designs
- DRC/review before manufacturing release
Applicability: component/vendor-specific guidance; useful as commercial corroboration, not universal rules across all electronics.

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
Evidence basis: NASA V&V planning explicitly distinguishes breadboards, prototypes, engineering units, qualification units and operational/final units and asks what activities apply to each.
Podcast use: A4–A7 and Prototype Representativeness framework.

### C-EHD-004 — A functional prototype is not equivalent to a production-ready product
status: STRONG when combined with existing Product Readiness evidence package
Evidence basis: TRL prototype progression addresses technology demonstration; production-readiness evidence requires additional manufacturing/process/supply/test controls.
Podcast use: bridge from A8 to Episode 1.

### C-EHD-005 — Configuration management has value before production
status: STRONG CONCEPTUAL SUPPORT + COMMERCIAL IMPLEMENTATION SUPPORT
Evidence basis: NASA describes CM as maintaining true product representation, distinguishing versions, controlling changes and keeping product/documentation consistent across design, fabrication, test, integration and operation. KiCad 9 includes Git integration for tracking design changes, while Git/GitHub tagging can identify known points in firmware/software history.
Podcast use: A8.

### C-EHD-006 — Early prototype technology choices can create downstream manufacturing debt
status: GNR SYNTHESIS
Rationale: central podcast thesis but still needs broader empirical/industrial evidence tying prototype-route decisions to later redesign, tooling, qualification, supply or cost consequences.
Podcast use: A4–A6.

### C-EHD-007 — Hardware teams should plan verification approach while defining requirements
status: STRONG
Evidence basis: NASA V&V guidance explicitly recommends identifying verification approach while developing requirements and uses requirement-verification matrices.
Podcast use: A1, A3, A7.

### C-EHD-008 — System interfaces deserve explicit ownership and verification
status: MODERATE/STRONG CONCEPTUAL SUPPORT
Evidence basis: NASA SE identifies interface definition/assessment as a core systems-engineering responsibility; broader industrial corroboration still needed for startup-oriented prescriptive guidance.
Podcast use: A2–A3.

### C-EHD-009 — Lightweight version control is practical for small electronics/firmware teams
status: STRONG IMPLEMENTATION SUPPORT / not a universal process prescription
Evidence basis: KiCad 9 integrates Git directly into the project manager and supports commits, branches, push/pull and repository creation for electronics projects. GitHub tags/releases identify specific repository states.
Podcast use: A8.
Practical translation:
- DEV: controlled project repository + meaningful commits + build/revision notes
- LVP: tagged released hardware/firmware states linked to BOM/PCB/mechanical revision and test evidence
- SVP: PLM/controlled product configuration and formal effectivity, while Git remains an engineering source/history system where appropriate

### C-EHD-010 — Firmware revision should be part of physical-unit configuration when product behavior depends on it
status: STRONG SYNTHESIS / needs more product-specific primary evidence in Pass 2
Evidence basis: configuration-control logic plus tagged software/firmware history implies that the hardware serial alone is insufficient when firmware changes function, calibration, safety or test behavior.
Podcast use: A6, A8 and later genealogy episodes.

### C-EHD-011 — Engineering changes can force previously completed decisions and work to be revisited
status: STRONG
Evidence basis: NISTIR 7922 describes engineering change as revisiting decisions/tasks considered completed and notes significant manufactured-system cost can arise from changing specifications after systems have been built and delivered.
Podcast use: A1, A3, A8 and Episode 31.
Important boundary: this supports change cost/complexity qualitatively; it does not establish a universal “10x/100x cost of late change” curve.

### C-EHD-012 — A schematic/PCB project is a controlled multi-artifact configuration, not just a PCB file
status: STRONG IMPLEMENTATION SUPPORT
Evidence basis: KiCad project documentation identifies project, schematic, PCB, libraries/settings and manufacturing-output files and warns that project-level design information can be lost when artifacts are separated from the project context.
Podcast use: A6, A8.

## Lightweight configuration-management pattern for teams of 2–20
This is a GNR-derived implementation pattern backed by the CM principles and tooling evidence above; it is not presented as a standard.

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

SVP extension:
- formal PLM/MES/QMS/effectivity model where justified
- supplier and production-process revisions
- serialized/lot genealogy
- controlled software deployment/calibration configuration

## Evidence gaps remaining before A0 Breadth Complete
1. Mechanical prototype-to-production commercial case studies.
2. Broader prototype-fidelity/representativeness literature outside aerospace.
3. Stronger primary evidence for firmware/hardware co-configuration in commercial products.
4. Regulatory/product-safety discovery timing by product class.
5. More empirical evidence tying early prototype choices to downstream manufacturing debt.

## Pass-2 depth targets already identified
- quantify/document engineering-change propagation and cost without relying on folklore multipliers;
- collect mechanical examples where prototype process masked serial-process failure modes;
- build PCB/PCBA production-transition source pack: DFM, panelization, assembly, test, component lifecycle and change control;
- define practical product-configuration object linking hardware revision, BOM, firmware, calibration and test evidence;
- compare lightweight Git-based DEV configuration control with PLM-level LVP/SVP needs.

## Editorial boundary
The Opening Arc should teach minimum useful engineering discipline, not transplant a large-enterprise stage-gate bureaucracy into a startup. Every practice should be presented with a scaling question: what is the lightest implementation that preserves the engineering intent at DEV, LVP and SVP?