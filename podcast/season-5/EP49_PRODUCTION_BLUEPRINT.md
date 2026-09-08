# Episode 49 Production Blueprint — Standards, Claims and Evidence as a Manufacturing Knowledge Graph

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
lifecycle: CROSS-STAGE
maps_to: MASTER_WBS 9.8

## Listener transformation
Before: stores standards, reports and engineering knowledge mainly as documents and search results.
After: models requirement/standard applicability, engineering claims, evidence, configuration and decisions as linked objects whose provenance and validity can be inspected.

## Narrative hook
An engineer finds a PDF proving a material test passed. Months later nobody can tell which requirement the test addressed, which product revision it covered or whether a supplier/process change invalidated it. The document exists; the engineering claim has lost its context.

## Teaching flow
1. Documents are sources/containers, not engineering truth by themselves.
2. Question → decision → claim → evidence → source chain.
3. Applicability and configuration envelope are mandatory context.
4. Separate source says from engineering conclusion/synthesis.
5. Link standards/regulations/customer requirements to controlled claims.
6. Evidence can support multiple claims but only within valid scope.
7. Changes trigger dependency-based impact review, not universal evidence deletion.
8. Contradictions and unresolved uncertainty should be first-class objects.
9. Provenance, maturity and review status prevent GNR from becoming invisible truth.
10. Search/retrieval should return the decision context and evidence path, not only documents.

## Core framework — Claim–Evidence Knowledge Graph
`Question → decision → claim → applicability/configuration → evidence → source/location → maturity/reviewer → related object → change dependency`.

## Listener tools
- Claim Evidence Card.
- Evidence Impact Query: what claim does this evidence support, for which configuration/envelope, what depends on it, and what change would require reassessment?

## DEV / LVP / SVP
DEV: lightweight claim/evidence capture prevents reconstruction debt. LVP: supplier/process/test evidence becomes graph-linked to configuration. SVP: governance, access, review maturity and change impact support scalable decision integrity.

## Common mistakes
- PDF repository called a knowledge base;
- search relevance mistaken for evidence strength;
- standard citation without edition/scope/location;
- AI synthesis stored as verified fact;
- source and conclusion merged;
- change causes blanket requalification or, worse, no reassessment at all.

## Standards/applicability gate
Normative claims require authoritative designation, edition/status, exact support location where needed and explicit applicability. Controlled standards content must respect licensing; secondary summaries assist discovery but do not silently replace authoritative P0 evidence.

## Closing handoff
Episode 50 turns this graph from a memory system into a decision system: the Manufacturing Atlas.
