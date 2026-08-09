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
Source: NASA Systems Engineering Handbook (current web edition; handbook lineage includes NASA/SP-2016-6105 Rev2).
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

### NPR 7123.1D / endorsed standards list
Use for standards discovery only at this breadth stage, including systems life-cycle, V&V and configuration-management standards. Clause-level applicability remains Pass-2 work.

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
status: STRONG CONCEPTUAL SUPPORT
Evidence basis: NASA describes CM as maintaining true product representation, distinguishing versions, controlling changes and keeping product/documentation consistent across design, fabrication, test, integration and operation.
Podcast use: A8.

### C-EHD-006 — Early prototype technology choices can create downstream manufacturing debt
status: GNR SYNTHESIS
Rationale: highly plausible and central to podcast thesis, but needs broader empirical/industrial evidence before being presented as a general factual claim.
Podcast use: A4–A6.

### C-EHD-007 — Hardware teams should plan verification approach while defining requirements
status: STRONG
Evidence basis: NASA V&V guidance explicitly recommends identifying verification approach while developing requirements and uses requirement-verification matrices.
Podcast use: A1, A3, A7.

### C-EHD-008 — System interfaces deserve explicit ownership and verification
status: MODERATE/STRONG CONCEPTUAL SUPPORT
Evidence basis: NASA SE identifies interface definition/assessment as a core systems-engineering responsibility; broader industrial corroboration still needed for startup-oriented prescriptive guidance.
Podcast use: A2–A3.

## Evidence gaps for Pass 1
1. Commercial/startup hardware development references outside aerospace.
2. Electronics/PCB/embedded development and transition-to-production evidence.
3. Mechanical prototype-to-production transition case studies.
4. Empirical evidence around late requirement/interface changes and rework cost.
5. Practical configuration-management patterns appropriate to teams of 2–20 people.
6. Prototype fidelity/representativeness literature beyond aerospace.
7. Regulatory/product-safety discovery timing by product class.

## Editorial boundary
The Opening Arc should teach minimum useful engineering discipline, not transplant a large-enterprise stage-gate bureaucracy into a startup. Every practice should be presented with a scaling question: what is the lightest implementation that preserves the engineering intent at DEV, LVP and SVP?