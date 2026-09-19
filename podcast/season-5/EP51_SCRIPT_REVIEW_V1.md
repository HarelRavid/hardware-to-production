# EP51 Script Review V1 — OPC UA, ISA-95 and Semantic Integration Without the Buzzwords

status: PASS TO SOURCE NOTES
review_date: 2026-09-19
script_reviewed: EP51_SCRIPT_DRAFT_V1.md
source_lock: evidence/source-lock/wave-05/
reviewer_type: internal technical/editorial review; independent external human review not claimed

## Decision
The script correctly separates connectivity, syntax and semantics and keeps ISA-95/OPC UA inside their public source boundaries.

PASS TO SOURCE-NOTE PACKAGING.

## Technical findings
- connectivity/syntax/semantics distinction: PASS.
- ISA-95 2025 context: PASS.
- ISA-95 not mandatory stack: PASS.
- OPC UA infrastructure/information-model layer: PASS.
- Companion Specification framing: PASS.
- durable identity mapping: PASS.
- NodeId/tag/database-key nuance: PASS.
- event/state/time-series distinction: PASS as synthesis.
- semantic-model version/effectivity: PASS.
- protocol security vs OT security boundary: PASS.

## Recording-lock guards
- ISA-95 levels are not presented as Purdue/security zones;
- NodeId is not declared inherently unstable/inadequate;
- Companion Specification use is recommendation where applicable, not universal mandate;
- OPC UA security does not replace OT security program.

**EP51 SCRIPT REVIEW V1: PASS TO SOURCE NOTES**
