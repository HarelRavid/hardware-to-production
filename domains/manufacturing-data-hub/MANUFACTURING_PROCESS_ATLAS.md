# 9.9 Manufacturing-Process Atlas

status: Researching
provenance: [GNR]

## Purpose
Provide a decision/navigation layer over the manufacturing knowledge domains without duplicating their underlying content.

## Atlas principle
The Atlas references authoritative Knowledge Objects, Claims, Decisions, Standards and operational evidence. It does not become a parallel encyclopedia.

## Atlas entry points
- manufacturing process family
- material family
- geometry/feature
- tolerance/surface requirement
- volume/takt
- defect/failure mode
- equipment/resource capability
- inspection/test requirement
- industry/application
- cost/lead-time objective
- question/decision

## Core Atlas views
### Process family card
- process definition
- typical materials
- geometry envelope
- tolerance/surface boundary
- tooling/NRE
- rate/volume suitability
- common defects
- inspection implications
- downstream/post-processing
- standards/source maturity
- decision links

### Cross-process comparison
Compare candidate processes across explicit dimensions rather than a single score.

### Process chain view
Show upstream/downstream effects, intermediate product states, inspection gates and sequence-dependent failure modes.

### Failure-mode view
Failure mode -> likely creation processes -> contributing conditions -> detection methods -> related claims/case studies.

### Evidence maturity view
Expose which process-selection claims are verified, bounded by standards, industrially validated or still GNR.

## Selection dimensions
- material compatibility
- part size/geometry
- feature accessibility
- tolerance/GD&T
- surface condition
- mechanical/property requirements
- annual volume/takt
- tooling/NRE
- lead time
- automation
- inspection/qualification
- supplier maturity
- environmental/EHS constraints
- lifecycle cost

## Decision objects
### D-ATLAS-PROC-001 — Candidate manufacturing process families
### D-ATLAS-COMP-001 — Compare process candidates with evidence and tradeoffs
### D-ATLAS-CHAIN-001 — Candidate end-to-end manufacturing chain
### D-ATLAS-NOT-001 — Why should a seemingly obvious process not be selected?

## Integrity rules
- no hidden universal score that masks tradeoffs;
- no process recommendation without assumptions and scope;
- Atlas summaries must link back to authoritative Objects/Claims;
- conflicting evidence remains visible;
- prototype suitability and serial-production suitability are separate dimensions.
