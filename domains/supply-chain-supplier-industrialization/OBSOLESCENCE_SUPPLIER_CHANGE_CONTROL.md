# 7.9 Obsolescence & Supplier Change Control

status: Researching
provenance: [GNR]

## Obsolescence objects
- component/material lifecycle status
- end-of-life notification
- last-time-buy boundary
- alternate qualification
- redesign trigger
- inventory exposure
- shelf-life/storage risk
- tool/process obsolescence
- software/firmware compatibility boundary

## Supplier-change objects
- site change
- sub-tier change
- raw material source change
- formulation/grade change
- manufacturing-process change
- tooling/equipment change
- inspection/test-method change
- packaging/logistics change
- ownership/M&A boundary

## Engineering principle
A supplier-side change can be technically significant even when the purchased part number and drawing remain unchanged.

## Questions
1. Which supplier changes require notification versus prior approval?
2. Can the change alter fit, function, reliability, cleanliness, surface state or process capability without changing nominal dimensions?
3. What inventory/WIP exists across old/new states?
4. Is bridging stock needed during requalification?
5. Does obsolescence create a redesign, alternate-source or lifetime-buy decision?
6. Are old/new supplier/process states traceable after cut-in?

## Decision objects
### D-SUP-CHG-001 — Supplier change impact and approval scope
### D-SUP-OBS-001 — Obsolescence response strategy
### D-SUP-LTB-001 — Last-time-buy versus redesign/alternate qualification
### D-SUP-EFF-001 — Effectivity and genealogy for supplier/process changes

## Cross-links
Supplier change <-> Section 6 change/revalidation
Obsolescence <-> product lifecycle
Alternate <-> dual sourcing
Effectivity <-> genealogy
Supplier process change <-> reliability

## Integrity rule
Unchanged drawing revision does not prove unchanged supplied-product risk.