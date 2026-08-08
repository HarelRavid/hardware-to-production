# 4.1 EBOM -> MBOM

status: Researching
provenance: [GNR]

## 4.1.1 Definitions
### EBOM
Engineering representation of the product as designed/released.

### MBOM
Manufacturing representation of the product as it must be built, supplied, staged, assembled, tested and recorded.

The relationship is not assumed to be one-to-one.

## 4.1.2 Transformation objects
- engineering part
- manufacturing part
- purchased part
- fabricated part
- consumable
- bulk material
- adhesive/sealant/chemical
- packaging material
- kit
- phantom assembly
- manufacturing subassembly
- alternate/substitute
- quantity / UOM
- scrap/yield factor boundary
- effectivity
- revision
- make/buy
- supplier source boundary

## 4.1.3 Common EBOM -> MBOM transformations
- regroup parts by actual assembly sequence
- create manufacturing subassemblies not explicit in CAD/product architecture
- add consumables and process materials
- add packaging/protection items where controlled by manufacturing
- represent purchased assemblies differently from engineering decomposition
- define kits/staging groups
- assign alternates/substitutes under controlled rules
- map parts to operations/work centers

## 4.1.4 Engineering questions
1. Does every physically consumed item exist in the manufacturing definition?
2. Are adhesives, lubricants, solvents, gases, labels and packaging treated as controlled materials where required?
3. Are assembly groupings aligned with how production actually builds and tests the product?
4. Can a manufacturing change be made without silently changing the engineering product definition?
5. Are effectivity and revision rules explicit for both EBOM and MBOM?
6. Is the same item represented with consistent units of measure and conversion rules?

## 4.1.5 Failure modes
- missing consumables
- duplicate part identities
- uncontrolled substitutions
- wrong revision/effectivity
- engineering assembly structure unusable for production staging
- kitting errors
- BOM quantity/UOM mismatch
- production uses tribal-knowledge items absent from MBOM
- packaging/service items mixed ambiguously with production material

## 4.1.6 Decision objects
### D-BOM-001 — Does this item belong in EBOM, MBOM, both, or another controlled structure?
### D-BOM-002 — Create manufacturing subassembly/phantom/kit?
### D-BOM-003 — How should alternates/substitutes be controlled?
### D-BOM-004 — What change/effectivity event requires BOM reconciliation?

## 4.1.7 Reconciliation model
Engineering revision -> EBOM delta -> manufacturing impact assessment -> MBOM/routing/WI/test/tooling update -> validation -> effectivity/release.

## Integrity principle
EBOM and MBOM may differ structurally, but they must remain reconciled to the same released product intent and configuration state.