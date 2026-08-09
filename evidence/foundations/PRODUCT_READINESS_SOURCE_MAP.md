# Product Development / NPI / Production Readiness — Source Map

status: Evidence Population — Pass 1 Breadth
started_on: 2026-08-09
maps_to: MASTER_WBS 1.1–1.6, 5.2, 5.10; PODCAST_MAP Episodes 1–5

## Purpose
Establish a high-authority evidence backbone for the first podcast arc: why functional hardware is not automatically production-ready, how development maturity differs from manufacturing maturity, and what production-readiness evidence should cover.

## Source families identified

### S-PR-001 — NASA Technology Readiness Levels
Authority: primary government framework
Use: technology maturity / prototype maturity boundary
Key evidence:
- TRL is a technology-maturity scale.
- TRL 3 includes analytical/experimental proof of concept.
- TRL 6 includes a fully functional prototype/representational model.
- higher TRLs move toward qualification and operational proof.
Applicability note: TRL measures technology maturity; it should not be treated as a complete manufacturing-readiness model.
URL: https://www.nasa.gov/directorates/somd/space-communications-navigation-program/technology-readiness-levels/

### S-PR-002 — NASA Production Readiness Review, NPR 7123.1D Appendix G
Authority: primary NASA systems-engineering requirement
Use: production-readiness evidence dimensions
Key evidence identified:
- significant production engineering problems/nonconformances should be resolved;
- design documentation needed for production should be available;
- production plans, process controls/procedures and production-enabling products should be ready;
- materials, resources, BOM, inspections/tests, risks, cost/schedule and personnel are part of readiness;
- success criteria include confidence in final production configuration and incorporation of DFM considerations.
Applicability note: NASA/aerospace framework; use as a strong production-readiness archetype, not as a universal mandatory gate for commercial hardware.
URL: https://nodis3.gsfc.nasa.gov/displayDir.cfm?Internal_ID=N_PR_7123_001D_&page_name=AppendixG

### S-PR-003 — NASA Manufacturing Readiness Levels (MRL) reference, NASA/TM-20220018403
Authority: primary government technical memorandum reproducing/using MRL framework
Use: distinguish manufacturing maturity from technology maturity and show progression from manufacturing concept to production-relevant capability.
Key evidence identified:
- early MRLs address manufacturing implications/concepts/proof of concept;
- MRL 4 includes capability to produce technology in a laboratory environment;
- MRL 5 includes prototype components in a production-relevant environment;
- manufacturing strategy, industrial base, tooling/test equipment, personnel skills, producibility and cost models become explicit maturity dimensions.
Applicability note: MRL framework is acquisition-oriented; use concepts and evidence dimensions carefully outside defense/aerospace.
URL: https://ntrs.nasa.gov/api/citations/20220018403/downloads/TM-20220018403.pdf

### S-PR-004 — NIST: Challenges in Setting up a Production Line during NPI
Authority: primary U.S. government research publication
Use: evidence that production-system creation is a distinct NPI workstream, not merely product-design completion.
Key evidence identified:
- setting up a production line/factory is described as a subset of the broader NPI process;
- activities include production targets, equipment/manpower capacity, capital procurement, manufacturing methods/technology, and verification of production/inspection equipment/processes.
URL: https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=932687

### S-PR-005 — Instrumental EVT/DVT/PVT guide
Authority: experienced industry practitioner / secondary industry source
Use: terminology comparison and evidence of nomenclature variation in hardware industry.
Key evidence identified:
- EVT/DVT/PVT/MP terminology is widely used in hardware/electronics;
- companies and even teams vary in how the stages are defined;
- therefore these labels should not be presented as universal standards without local exit criteria.
Applicability note: useful industry synthesis, not a normative standard.
URL: https://instrumental.com/build-better-handbook/evt-dvt-pvt

## Initial claim register

### C-PR-001
Claim: A functional proof of concept/prototype does not by itself demonstrate manufacturing readiness.
Evidence direction: S-PR-001 + S-PR-003 + S-PR-002.
Status: STRONG — verification/detail extraction still open.

### C-PR-002
Claim: Technology maturity and manufacturing maturity are related but distinct dimensions.
Evidence direction: compare TRL framework with MRL framework.
Status: STRONG.

### C-PR-003
Claim: Production readiness is multidimensional and includes documentation, processes, resources, materials, tooling/enabling products, quality/test planning, risk and production configuration — not only product function.
Evidence direction: S-PR-002.
Status: STRONG within NASA applicability; cross-industry corroboration open.

### C-PR-004
Claim: EVT/DVT/PVT labels do not have one universally standardized cross-industry meaning.
Evidence direction: S-PR-005 plus search for additional independent industry frameworks.
Status: MODERATE; needs corroboration before Podcast Ready.

### C-PR-005
Claim: Production-intent should be treated as multidimensional rather than a single yes/no state.
Evidence direction: synthesis from production-readiness dimensions, MRL progression, prototype representativeness and configuration evidence.
Status: GNR synthesis — high priority for verification/bounding.

### C-PR-006
Claim: One successful build provides weak evidence of repeatability/capability unless the process, inputs, measurement system and production conditions are representative and variation is assessed.
Evidence direction: bridge to MSA/SPC/capability, MRL and PVT evidence.
Status: GNR synthesis — high priority.

## Episode-critical questions still open
1. Is there a high-authority source that formally defines EVT/DVT/PVT, or should the podcast explicitly state they are industry conventions?
2. What are the strongest cross-industry production-readiness frameworks outside aerospace/defense?
3. How should MRL concepts be translated for startups without importing acquisition bureaucracy?
4. Which evidence best supports the term/manufacturing-debt concept?
5. What quantitative evidence demonstrates the danger of extrapolating from one/few prototype builds?

## Pass-2 targets
- clause/table extraction from NASA PRR and MRL sources;
- independent source for EVT/DVT/PVT variability;
- ISO/APQP/industry readiness analogues where applicable;
- capability/statistical evidence for repeatability claim;
- case study for functional prototype -> production failure;
- convert high-confidence claims into Knowledge OS Claim Objects with applicability and evidence links.

## Readiness
Source map: STARTED
Critical claims identified: YES
Primary-source backbone: YES
Conflicts/applicability visible: YES
Podcast Ready: NO