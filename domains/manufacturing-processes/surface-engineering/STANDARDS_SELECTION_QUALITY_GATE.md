# 3.12.8 Standards, Process Selection & Quality Gate

status: Researching
provenance: [GNR]

## Standards/source families to populate
Primary-source families include:
- ISO surface preparation standards
- ISO/ASTM coating thickness and adhesion test methods
- ISO/ASTM corrosion/environmental test methods
- plating/electroless and conversion/passivation specifications
- anodizing specifications
- paint/powder-coating system standards
- PVD/CVD/thermal-spray process and coating standards where applicable
- application-specific aerospace, automotive, medical, food/pharma, electrical or pressure-equipment requirements where relevant

Every Standard Object must retain edition/revision, substrate/process/application scope, test conditions, normative role and linked claims/decisions.

## Master decision object
### D-SURF-MASTER-001 — Which surface engineering system should be used?
Inputs:
- substrate/material condition
- required function
- corrosion/environment
- wear/friction
- electrical/thermal function
- cosmetic requirement
- geometry/access
- tolerance/GD&T
- masking/contact restrictions
- joining sequence
- service temperature
- volume/takt
- reworkability
- regulation/standards
- supplier capability
- total lifecycle cost

Candidate routes may include:
- no coating / controlled bare surface
- mechanical finish only
- passivation/conversion treatment
- anodizing
- electro/electroless plating
- paint/liquid coating
- powder coating
- PVD/CVD
- thermal spray
- surface-hardening route boundary
- alternate material/substrate choice

## Process-selection principle
Select a surface system, not merely a named coating. Substrate preparation + pretreatment + coating/deposition + cure/post-treatment + inspection + handling/packaging jointly define the production route.

## Architecture coverage
- domain taxonomy: COMPLETE
- preparation/cleanliness boundary: COMPLETE architecture
- mechanical finishing: COMPLETE architecture
- plating/electroless: COMPLETE architecture
- conversion/passivation: COMPLETE architecture
- anodizing: COMPLETE architecture
- paint/powder: COMPLETE architecture
- PVD/CVD/thermal-spray boundaries: COMPLETE architecture
- masking/fixturing/racking: COMPLETE architecture
- dimensional/coating-thickness integration: COMPLETE architecture
- corrosion/environmental validation: COMPLETE architecture
- inspection/testing: COMPLETE architecture
- rework/stripping: COMPLETE architecture
- automation/economics: COMPLETE architecture
- standards/process-selection: COMPLETE architecture

## Open population work
- current clause-level standards extraction
- substrate/process-specific preparation evidence
- quantitative thickness/capability data
- adhesion/porosity test applicability
- corrosion/service correlation evidence
- hydrogen-embrittlement controls for relevant process/material combinations
- coating compatibility with joining/adhesives/seals
- industrial case studies
- supplier capability/process-control examples
- top questions/decisions/mistakes/myths/lessons
- GNR verification

## Integrity gates before Podcast Ready
1. Coating is included in dimensional design.
2. Surface preparation is part of the coating system.
3. Masking/contact/racking requirements are represented.
4. Internal/recessed geometry includes coverage and drainage/access analysis.
5. Accelerated test duration is not treated as direct service life without validated correlation.
6. Rework/stripping effects on substrate and qualification are assessed.
7. Finish selection is compared with alternate substrate/material choices where appropriate.
8. Standards carry revision and applicability.
9. Decisions expose assumptions/open questions.
10. GNR remains visible until verified.

## Status
Architecture: CLOSED
Knowledge population: OPEN
Evidence verification: OPEN
Podcast readiness: NOT READY

## Next domain
3.13 Cleaning, Contamination Control & Clean Manufacturing, per MASTER_WBS.md.