# Wave 06B Internal Technical Review — EP12

status: PASS TO SCRIPT OUTLINE WITH MATERIAL/PROCESS GUARDRAILS
review_date: 2026-09-19
reviewer_type: internal technical/editorial review; independent external human review not claimed

inputs:
- SOURCE_LOCK_WAVE_06B_POLYMERS_REGISTER.md
- W6B_EP12_CLAIM_LOCK.md
- EP12 Production Blueprint
- polymer-forming/elastomer domain maps
- Wave 06A process-selection package
- Wave 01 representativeness
- Wave 02 measurement/quality
- Wave 03 economics

## Decision

EP12 can advance to script outline using current public standards scope and scoped technical guidance without generic DFM folklore.

## Technical findings

### Current standards status
PASS.
ISO 20457:2026 correctly replaces ISO 20457:2018.
ISO 294-1:2017, ISO 294-4:2018 and ISO 62:2008 remain current/confirmed at the checked date.

### Moulded tolerance framing
PASS.
Use plastics-specific tolerance/process behavior; do not imply ISO 20457 gives one simple tolerance table applicable without material/process context.

### Shrinkage
PASS.
Directional/material/process dependency is directly supported.
Do not present one scalar shrink factor as engineering truth.

### Warpage
PASS.
Differential cooling/shrinkage/orientation explanation is technically coherent.
Do not say one mechanism always dominates.

### Sink/voids
PASS.
Mechanism linked to thick/local geometry and packing/cooling/material.
Do not include common online rib-percentage rules.

### Weld/meld lines
PASS.
Location/process/material consequence remains conditional.
Do not present every weld line as structural failure.

### Moisture/conditioning
PASS.
Keep material-specific.
BASF examples demonstrate variability among grades; they do not create a family-wide rule.

### Tooling/gating/cooling/ejection
PASS.
Treat as product/process architecture.
No supplier-guide numeric design dimensions.

### Alternate routes
PASS at high level.
EP12 may introduce extrusion/blow/thermoforming/rotomoulding/compression/transfer/reactive routes as candidates without pretending to teach their full process physics.

### Bridge route
PASS.
Reuse 06A instead of inventing new volume break-even thresholds.

## Required script guards

1. no generic wall thickness;
2. no generic draft angle;
3. no generic rib/boss ratio;
4. no generic shrinkage percentage;
5. no generic drying recipe;
6. no generic tolerance table spoken from memory;
7. exact grade and conditioned state visible when property examples are used;
8. CNC/AM prototype evidence transferred claim-by-claim;
9. simulation is decision support, not release qualification;
10. injection moulding is an anchor process, not automatically the preferred SVP route.

## Boundary with other episodes

EP11 owns route-selection method.
EP12 owns polymer route/material/process physics at practitioner level.
EP17 owns additive depth.
EP18 owns surface/cleaning/thermal-state depth.
EP19 owns full process-chain sequence.

Result: PASS — no merge or architecture change required.

**WAVE 06B INTERNAL TECHNICAL REVIEW: PASS**
