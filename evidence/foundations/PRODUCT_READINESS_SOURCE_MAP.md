# Product Development / NPI / Production Readiness — Source Map

status: BREADTH COMPLETE
campaign: A1
started_on: 2026-08-09
maps_to: MASTER_WBS 1.1–1.6, 5.2, 5.10; PODCAST_MAP Episodes 1–5
provenance: primary-source-first

## Purpose
Establish the evidence backbone for why functional hardware is not automatically production-ready, how technology/product/manufacturing maturity differ, and what evidence should exist before low-volume and serial production.

## Source families captured

### S-PR-001 — NASA Technology Readiness Levels
Authority: primary government framework
Use: technology maturity / prototype maturity boundary.
Key evidence:
- TRL is a technology-maturity scale.
- TRL 3 includes proof of concept.
- TRL 6 includes a fully functional prototype/representational model.
Applicability: TRL is not a complete manufacturing-readiness model.
URL: https://www.nasa.gov/directorates/somd/space-communications-navigation-program/technology-readiness-levels/

### S-PR-002 — NASA Production Readiness Review, NPR 7123.1D Appendix G
Authority: primary NASA systems-engineering requirement
Use: production-readiness evidence dimensions.
Evidence dimensions include production documentation, process controls/procedures, production-enabling products, materials/resources, BOM, inspection/test, risks, cost/schedule, personnel and confidence in final production configuration.
Applicability: aerospace archetype, not universal commercial gate.
URL: https://nodis3.gsfc.nasa.gov/displayDir.cfm?Internal_ID=N_PR_7123_001D_&page_name=AppendixG

### S-PR-003 — Manufacturing Readiness Levels / NASA and NIST references
Authority: government technical sources
Use: distinguish manufacturing maturity from technology maturity and show progression toward production-relevant/representative environments and rate.
Key evidence:
- MRL progression separates laboratory production, production-relevant prototypes, production-representative capability, pilot/low-rate production and full-rate production.
- MRLs include multiple manufacturing threads rather than one binary readiness state.
URLs:
- https://ntrs.nasa.gov/api/citations/20220018403/downloads/TM-20220018403.pdf
- NIST Quantitative Benchmark for Time to Market framework (MRL summary)

### S-PR-004 — NIST: Challenges in Setting up a Production Line during NPI
Authority: primary U.S. government research publication
Use: production-system creation as a distinct NPI workstream.
Evidence includes production targets, equipment/manpower capacity, capital procurement, manufacturing methods/technology and verification of production/inspection equipment/processes.
URL: https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=932687

### S-PR-005 — AIAG Advanced Product Quality Planning / Control Plan / PPAP ecosystem
Authority: major automotive industry body
Use: cross-industry corroboration that launch readiness is planned across product/process development, sourcing, risk, controls, traceability and production approval rather than inferred from product function.
Key evidence:
- APQP 3rd edition addresses sourcing, change management, metrics, risk mitigation and gated management.
- AIAG Core Tools connect APQP, FMEA, MSA, SPC, Control Plan and PPAP to new-product launch and ongoing manufacturing.
- PPAP is used to demonstrate/approve production-process readiness in its intended automotive context.
Applicability: automotive-specific requirements must not be presented as universal requirements; the planning logic is broadly useful.
URLs:
- https://www.aiag.org/training-and-resources/manuals/details/APQP-3
- https://www.aiag.org/expertise-areas/quality/quality-core-tools
- https://go.aiag.org/apqp-cp

### S-PR-006 — Commercial semiconductor NPI maturity example captured through NIST Baldrige material
Authority: NIST-hosted industrial case material
Use: commercial corroboration of a staged prototype -> high-volume-manufacturing compatibility -> qualification -> production progression.
Key evidence: the documented NPI process separates a fully functional prototype milestone from a later phase reviewing compatibility with high-volume manufacturing, followed by qualification/documentation before production release.
Applicability: company-specific case, valuable as an example rather than a universal lifecycle.
Source: NIST-hosted ST Application Summary.

### S-PR-007 — Industry EVT/DVT/PVT terminology
Authority: industry practitioner/secondary sources
Use: terminology and workflow comparison.
Current evidence indicates EVT/DVT/PVT terminology is common in electronics/hardware but definitions vary by organization/team.
Applicability: treat as useful industry shorthand, not a universal normative maturity scale.
Example source: https://instrumental.com/build-better-handbook/evt-dvt-pvt

## Claim register

### C-PR-001 — Functional prototype != manufacturing readiness
status: STRONG
Evidence: TRL + MRL + PRR + commercial NPI case.
Podcast use: Episode 1.

### C-PR-002 — Technology maturity and manufacturing maturity are related but distinct
status: STRONG
Evidence: TRL versus MRL frameworks.
Podcast use: Episodes 1–2.

### C-PR-003 — Production readiness is multidimensional
status: STRONG
Evidence: NASA PRR/MRL + AIAG APQP/Core Tools + NIST NPI.
Dimensions include product configuration, process, resources, materials/supply, tooling, measurement/test, quality controls, people, documentation, capacity/rate and risk.
Podcast use: Episodes 1–5.

### C-PR-004 — EVT/DVT/PVT labels do not have one universally standardized cross-industry meaning
status: MODERATE / sufficient for Breadth, Pass-2 corroboration required
Podcast rule: define the meaning used in this series and focus on exit evidence rather than stage labels.

### C-PR-005 — Production-intent is better modeled as multidimensional than binary
status: STRONG SYNTHESIS, not a quoted standard
Evidence basis: PRR readiness dimensions + MRL threads/progression + APQP launch planning + prototype representativeness model.
Podcast use: Episode 3.

### C-PR-006 — One successful build is weak evidence of repeatability/capability
status: STRONG ENGINEERING SYNTHESIS; quantitative/statistical depth deferred to A4/A5
Evidence direction: MRL production-relevant/representative progression + APQP/PPAP/SPC/MSA logic.
Podcast use: Episodes 1, 4, 5.

### C-PR-007 — Production-system development is a parallel engineering workstream
status: STRONG
Evidence: NIST NPI production-line work + PRR + APQP.
Podcast use: Episodes 2–5.

### C-PR-008 — A fully functional prototype may precede a separate high-volume-manufacturing compatibility review
status: STRONG AS CASE EXAMPLE, not universal stage model
Evidence: NIST-hosted commercial semiconductor NPI case.
Podcast use: Episode 1 opening example.

## DEV / LVP / SVP translation
### DEV
Goal: prove requirements, architecture and key technical risks while capturing configuration and manufacturing implications.
Do not pretend prototype tooling/process/supplier evidence is production evidence.

### LVP — tens/hundreds
Goal: produce controlled, repeatable units with explicit BOM/revision, routings/work instructions, test/inspection, approved materials/suppliers, basic genealogy and visible rework/deviation.
Manual/semi-automated production is acceptable when capable and controlled.

### SVP — serial/commercial production
Goal: demonstrated process capability/rate, scalable supply, production tooling/equipment, controlled change/effectivity, mature quality/test system, maintenance and stable operational ownership.

## Applicability conflicts / cautions
1. NASA PRR/MRL and automotive APQP/PPAP are powerful evidence frameworks but carry sector-specific bureaucracy and terminology.
2. Podcast guidance should extract engineering intent and scale implementation to team size, product risk and volume.
3. EVT/DVT/PVT should be presented as a practical hardware-industry vocabulary, not as an ISO-like universal standard.
4. Production-intent multidimensionality is our synthesis and must be labeled as such.
5. Capability thresholds and statistical proof belong in A4/A5 rather than being invented here.

## Pass-2 depth targets
- clause/table extraction from NASA PRR and MRL sources;
- stronger independent corroboration of EVT/DVT/PVT terminology variation;
- detailed APQP/PPAP applicability and evidence-object mapping;
- statistical evidence for repeatability/capability claims;
- industrial case studies where functional prototypes failed at production transition;
- convert high-confidence claims into Knowledge OS Claim Objects with applicability/evidence links.

## Breadth promotion check
1. authoritative source families: YES
2. episode-critical claims: YES
3. weak/GNR claims visible: YES
4. applicability conflicts visible: YES
5. Pass-2 depth targets: YES

## Readiness
Source map: BREADTH COMPLETE
Primary-source backbone: YES
Cross-industry corroboration: YES — aerospace/government + automotive + commercial industrial example
Podcast Ready: NO — depth/verification/case population remains open