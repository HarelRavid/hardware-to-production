# 0.6 Standards Revision & Applicability Control

status: Researching
provenance: [GNR]

## Purpose
Prevent standards, regulations and guidance from being treated as timeless or universally applicable evidence.

## Standard / Regulation object metadata
- stable internal ID
- issuing body
- designation
- title
- edition/revision/date
- status: current / superseded / withdrawn / unknown
- normative versus informative role
- jurisdiction / industry / product / process scope
- exclusions and applicability limits
- supersedes / superseded-by relationship
- source location
- access/review date
- linked clauses/requirements
- linked claims/decisions/domains

## Clause-level requirement object
Where a specific engineering conclusion depends on a clause, retain:
- standard revision
- clause/section identifier
- requirement summary
- normative language class where relevant
- applicability context
- exceptions/conditions
- linked evidence/claim

## Applicability decision
Standard existence != applicability.

Applicability should evaluate:
1. governing contract/customer requirement;
2. jurisdiction/regulatory adoption;
3. product/process/material scope;
4. lifecycle phase;
5. edition/effectivity;
6. exclusions and special conditions;
7. whether use is normative, adopted voluntarily, or informative/analogical.

## Revision-change workflow
Revision detected -> compare affected clauses -> identify linked Claims/Decisions/Objects -> assess impact -> update applicability/evidence -> record review decision -> preserve historical revision relationships.

## Cross-industry use rule
A standard from aerospace, automotive, medical, semiconductor or another sector may provide useful engineering guidance, but must not be labeled mandatory outside its governing scope unless separately adopted by contract, law, specification or internal requirement.

## Decision objects
### D-KOS-STD-001 — Is this standard applicable, informative or irrelevant to the current engineering decision?
### D-KOS-REV-001 — Does a new revision invalidate or modify existing Claims/Decisions?

## Integrity rules
- Never cite a standard without revision when revision can affect meaning.
- Never infer applicability from title similarity alone.
- Preserve superseded standards when they governed historical product/process evidence.
- Avoid paraphrasing a recommendation as a mandatory requirement.