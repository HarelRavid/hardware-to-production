# 3.14.8 Standards, Process Selection & Quality Gate

status: Researching
provenance: [GNR]

## Standards/source architecture to populate
Primary families to research and scope:
- alloy/material heat-treatment specifications and product standards
- AMS 2750 pyrometry requirements and current revision/applicability boundary
- AIAG CQI-9 Heat Treat System Assessment and automotive applicability boundary
- ASTM/ISO hardness, tensile, metallography, grain-size, case-depth and decarburization methods where relevant
- aerospace, automotive, medical, pressure-equipment and other application-specific requirements
- customer/supplier special-process approval requirements

A special-process standard from one industry is not automatically normative for another. Informative use must be labeled accordingly.

## Master process-selection dimensions
- alloy/material and incoming condition
- target microstructure/properties
- through vs surface/local treatment
- geometry/section thickness
- distortion sensitivity
- oxidation/decarburization sensitivity
- atmosphere/vacuum need
- quench/cooling need
- upstream/downstream sequence
- machining allowance
- production volume/load strategy
- inspection/property verification
- traceability/qualification
- supplier capability
- total cost per good part

## Architecture coverage
- domain taxonomy: COMPLETE
- annealing/stress relief: COMPLETE architecture
- hardening/tempering: COMPLETE architecture
- solution treatment/aging: COMPLETE architecture
- case/local hardening: COMPLETE architecture
- furnace/atmosphere/vacuum: COMPLETE architecture
- quench/cooling: COMPLETE architecture
- distortion/residual stress: COMPLETE architecture
- furnace/load qualification: COMPLETE architecture
- metallurgy/property verification: COMPLETE architecture
- traceability/automation/economics: COMPLETE architecture
- standards/process selection: COMPLETE architecture

## Open population work
- current standards/revisions and clause-level extraction
- alloy-specific heat-treatment evidence
- TUS/SAT/instrumentation requirements by application
- quench and distortion literature
- furnace-load scale-up case studies
- hardness/microstructure/property correlation limits
- special-process supplier qualification examples
- industrial failure case studies
- top questions/decisions/mistakes/myths/lessons
- GNR verification

## Integrity gates before Podcast Ready
1. Furnace setpoint is not treated as part thermal history.
2. Alloy/material condition is attached to every thermal recipe/property claim.
3. Production-load configuration is represented where it affects thermal response.
4. Quench/transfer/cooling is part of the thermal process where applicable.
5. Distortion is integrated with machining and GD&T strategy.
6. Hardness is not treated as universal proof of microstructure/properties.
7. Special-process standards retain industry/applicability boundaries.
8. Standards carry revision and applicability.
9. Decision objects expose assumptions/open questions.
10. GNR remains visible until verified.

## Status
Architecture: CLOSED
Knowledge population: OPEN
Evidence verification: OPEN
Podcast readiness: NOT READY

## Next domain
3.15 Manufacturing Process Integration, per MASTER_WBS.md.