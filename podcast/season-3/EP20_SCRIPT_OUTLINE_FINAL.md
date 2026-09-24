# EP20 Final Script Outline — From EBOM to MBOM and Process Flow

status: FINAL SCRIPT OUTLINE COMPLETE — SEASON CONTINUITY PENDING
season: Season 3 — Build the Factory Before You Need the Factory
audience: NPI / manufacturing / design / operations / quality
lifecycle: LVP → Production Validation → Ramp
source_lock: evidence/source-lock/season-3/S3A_EP20_CLAIM_LOCK.md
technical_review: evidence/source-lock/season-3/S3A_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-3/EP20_PRODUCTION_BLUEPRINT.md

## Listener transformation

Before:
“The engineering BOM is released, so production has the product definition it needs.”

After:
“I can translate released product definition into an executable manufacturing structure with operations, material/consumable inputs, resources, CTQs, traceability and controlled alternate/rework routes.”

## Two-character opportunity

Rona:
“Why can’t production just build from the engineering BOM?”

Oz:
Because the EBOM says what the product is; manufacturing also needs to know how material and operations transform it into the released unit.

## Cold open

[ILLUSTRATIVE]
Engineering releases a clean BOM. Production still asks:
which subassembly first, when firmware is loaded, where adhesive/labels/packaging live, which station owns inspection, and what happens if rework is needed.

## Beat 1 — Product definition vs executable process definition

Claims: EP20-C01/C02.

Use NIST process-plan premise:
task + resource + constraint + sequence.

## Beat 2 — EBOM / MBOM are useful models, not universal taxonomies

Claim: EP20-C03.

Guard:
do not imply one ERP/PLM/MES architecture.

## Beat 3 — Manufacturing decomposition

Claim: EP20-C04.

Examples:
subassemblies / kits / consumables / programming / packaging / process materials.

## Beat 4 — Operation as state transformation

Claim: EP20-C05.

For each operation:
input state
→ task
→ resource/tool
→ output state
→ CTQ/evidence
→ next dependency.

## Beat 5 — Routing and sequence

Claims: EP20-C02/C08.

Sequence matters because later operations may depend on previous state, access, datum, cleanliness or configuration.

## Beat 6 — Configuration and effectivity

Claim: EP20-C06.

Callback to A8 / EP19.

## Beat 7 — Alternate and rework routes

Claim: EP20-C07.

Rework adds history; do not silently create an undocumented alternate route.

## Listener tool — Product-to-Process Translation Map

Released product definition
→ manufacturing breakdown
→ operation sequence
→ material/consumable inputs
→ equipment/tooling
→ CTQ/test
→ output state
→ traceability
→ next operation.

## DEV / LVP / SVP

DEV:
build notes can be lightweight if identity/history survive.

LVP:
explicit routing/operation ownership becomes necessary.

SVP:
effectivity, alternates, rework and execution records must scale.

## Misconceptions

- EBOM copied to ERP = manufacturing definition;
- routing is only an ERP transaction;
- consumables/labels/programming are secondary details;
- rework can happen informally if final unit passes;
- operation sequence is obvious to experienced builders.

## Closing action

Take one released product and create the first version of a Product-to-Process Translation Map.

## Handoff

EP20 defines what production must execute.
EP21 asks how fixtures, tools and equipment make that execution repeatable.
