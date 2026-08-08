# 3.13.3 Cleanliness Verification & Acceptance

status: Researching
provenance: [GNR]

## Verification objects
- visual inspection
- particle extraction
- particle count/size distribution
- gravimetric residue
- nonvolatile residue
- ionic contamination/conductivity extraction boundary
- surface-energy/contact-angle boundary
- fluorescence/UV inspection boundary
- microscopy
- chemical analysis
- rinse-water/end-point monitoring
- functional verification

## Requirement model
Cleanliness requirement -> contaminant class -> critical surface/volume -> extraction/sampling method -> measurement method -> acceptance limit -> frequency -> reaction plan -> preservation method.

## Engineering principle
A measurement result is meaningful only if the sampling/extraction method can recover the contamination of concern from the relevant geometry with adequate repeatability.

## Questions
1. Are we measuring the contaminant that actually creates the failure mode?
2. Does the extraction method reach internal channels and crevices?
3. Is the measurement sensitive enough for the acceptance limit?
4. Does the verification process itself contaminate or damage the part?
5. Is cleanliness verified at the right point in the manufacturing sequence?

## Decision objects
### D-CLEAN-VER-001 — Verification method
### D-CLEAN-SAMP-001 — Sampling/extraction strategy
### D-CLEAN-FREQ-001 — 100%, batch/sample, process-monitoring or hybrid verification?

## Cross-links
Cleanliness verification <-> MSA
Acceptance <-> control plan
Particle data <-> failure analysis
Extraction method <-> geometry
Verification <-> traceability

No acceptance limit is universalized across applications.