# 3.15.2 Sequence Effects & Datum Migration

status: Researching
provenance: [GNR]

## Sequence-effect objects
- material condition entering operation
- residual stress entering operation
- surface condition entering operation
- cleanliness entering operation
- coating/oxide entering operation
- dimensional stock/allowance
- heat-input history
- joining-induced distortion
- post-process accessibility

## Sequence questions
- Does heat treatment occur before or after precision machining?
- Is coating applied before or after final assembly?
- Should cleaning occur before joining, coating, test, or packaging?
- Does welding destroy a previously machined datum relationship?
- Does blasting/polishing alter an edge or sealing surface?
- Does finishing block electrical grounding/contact requirements?

## Datum migration model
Design datum -> raw/near-net reference -> fixture datum -> intermediate machined datum -> thermal/process-distorted state -> finish-machined datum -> assembly datum -> inspection datum.

Each transition must record whether the datum is preserved, recreated, transferred or lost.

## Decision objects
### D-INT-SEQ-001 — Operation sequence selection
### D-INT-DAT-001 — Datum preservation/recreation strategy
### D-INT-ACCESS-001 — Which operations must occur before accessibility is lost?

## Failure modes
- final tolerance impossible after downstream distortion
- inspection datum differs from manufacturing datum without defined transform
- coating/heat treatment changes a previously accepted fit
- inaccessible surface cannot be cleaned/coated/inspected after assembly
- rework requires destructive disassembly

No sequence is universal; the functional chain drives selection.