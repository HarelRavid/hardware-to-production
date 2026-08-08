# 3.12.3 Plating, Conversion Coatings, Passivation & Anodizing

status: Researching
provenance: [GNR]

## Process families
### Electroplating
- zinc
- nickel
- copper
- chromium boundary
- tin/silver/gold boundary
- multilayer systems

### Electroless deposition
- electroless nickel and other applicable systems

### Conversion/passivation
- phosphate
- chromate/non-chromate conversion families
- stainless passivation
- black oxide boundary

### Anodizing
- sulfuric anodizing
- hard anodizing
- coloring/sealing boundary

## Core process objects
- substrate
- pretreatment
- bath chemistry
- temperature
- current/current density where applicable
- time
- agitation/flow
- anode/cathode geometry
- rack/contact point
- throwing power / coverage boundary
- thickness distribution
- post-treatment/sealing
- hydrogen embrittlement risk boundary

## DFM questions
1. How will coating thickness affect threads, bores, press fits and seal lands?
2. Which surfaces need masking or electrical contact?
3. Can recesses/internal features achieve required coverage?
4. Does substrate metallurgy/heat treatment create process risk?
5. Is post-bake or other embrittlement-control action required by the applicable specification?
6. Is the finish functional, cosmetic, or both?

## Failure modes
- poor adhesion
- blistering/peeling
- burning/pitting
- nonuniform thickness
- uncoated recesses
- rack/contact marks
- corrosion staining
- hydrogen-related cracking boundary
- sealing/post-treatment failure
- dimensional interference after coating

## Decision objects
### D-SURF-PLATE-001 — Plating/electroless vs conversion/anodize vs coating alternative
### D-SURF-MASK-001 — Masking and contact strategy
### D-SURF-ALLOW-001 — Required dimensional allowance for coating

## Integrity rule
Nominal coating family does not establish corrosion performance, thickness capability or embrittlement control without substrate, specification, process and test scope.