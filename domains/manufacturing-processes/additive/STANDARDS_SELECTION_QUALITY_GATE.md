# 3.11.8 Standards, Process Selection & Quality Gate

status: Researching
provenance: [GNR]

## Standards/source architecture to populate
Primary families:
- ISO/ASTM 52900-series additive manufacturing terminology, design, process/feedstock, qualification and test standards
- material/process-specific ASTM/ISO specifications
- application/industry requirements for aerospace, medical, pressure/service-critical products where applicable
- NDT/metrology standards used for AM parts
- conventional material and post-processing standards when AM does not supersede them

Every standard object must retain edition/revision, scope, process/material applicability, normative role and linked claims/decisions.

## Process selection candidates
- polymer material extrusion
- vat photopolymerization
- polymer powder bed
- metal powder bed fusion
- DED
- binder jetting
- material jetting
- hybrid additive/subtractive
- conventional alternative

## Selection dimensions
- material state/properties
- geometry and build envelope
- internal features
- orientation/aniso­tropy
- supports/cleaning
- tolerance/surface
- post-processing
- inspection/detectability
- qualification
- volume/takt
- tooling/NRE
- lead time
- supply-chain capability
- total lifecycle cost

## Architecture coverage
- domain taxonomy: COMPLETE
- polymer AM: COMPLETE architecture
- metal AM: COMPLETE architecture
- DfAM: COMPLETE architecture
- orientation/supports: COMPLETE architecture
- defects/anisotropy/residual stress: COMPLETE architecture
- post-processing: COMPLETE architecture
- inspection/cleaning: COMPLETE architecture
- feedstock: COMPLETE architecture
- qualification/traceability: COMPLETE architecture
- economics/AM-vs-conventional: COMPLETE architecture
- standards/selection: COMPLETE architecture

## Open population work
- clause-level standards extraction and current revisions
- process/material quantitative capability
- fatigue and defect-property literature
- feedstock reuse evidence
- in-process monitoring validation evidence
- qualification case studies
- cost/break-even case studies
- application-specific regulatory overlays
- top questions/decisions/mistakes/myths/lessons
- GNR verification

## Integrity gates before Podcast Ready
1. Printable is not treated as production-ready.
2. Machine/material label is not treated as a qualified material condition.
3. Orientation and post-processing remain part of evidence scope.
4. Internal features include cleaning and verification strategy.
5. AM is compared against conventional/hybrid alternatives.
6. No universal break-even volume.
7. Process monitoring claims require validated relationship to quality.
8. Standards carry revision/applicability.
9. Decision objects expose assumptions/open questions.
10. GNR remains visible until verified.

## Status
Architecture: CLOSED
Knowledge population: OPEN
Evidence verification: OPEN
Podcast readiness: NOT READY

## Next domain
Proceed according to the master WBS after 3.11; do not invent or renumber the next domain without checking the existing roadmap.