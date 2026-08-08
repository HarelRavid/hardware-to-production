# ADR-004 — Knowledge OS v1.0 Architecture Baseline

## Status
Accepted

## Context

The Hardware to Production project has accumulated enough real research across Prototype Workshop, manufacturing processes, Claims, Decisions, Relationships and provenance to validate the core Knowledge OS architecture.

Continually extending the architecture during content research would increase refactoring risk and distract from the primary objective: completing the Data Hub so it can support the podcast.

A final architecture review identified four important concepts that needed explicit representation before freezing the model:

1. Questions Answered / Open Questions
2. Engineering Assumptions
3. Knowledge Conflicts
4. Clear separation between workflow status, evidence maturity and provenance

## Decision

Knowledge OS v1.0 is adopted as the stable architecture baseline.

The stable organizational hierarchy is:

`Knowledge Layer → Domain → Module → Knowledge Object`

The reasoning/evidence flow is:

`Engineering Question → Engineering Decision → Engineering Claim → Knowledge Object → Source`

Engineering Claims remain the atomic evidence-bearing units.

The following are first-class controlled entity types in v1.0:

- Domain
- Module
- Knowledge Object
- Engineering Decision
- Engineering Claim
- Engineering Pattern
- Engineering Principle
- Failure Mode
- Standard / Regulation
- Book / Handbook
- Paper / Academic Source
- Template / Checklist
- Case Study
- Open Question
- Engineering Assumption
- Knowledge Conflict

AI-originated content retains `GNR` provenance permanently.

Workflow status and Evidence Maturity are independent dimensions.

Questions drive research/navigation but do not replace the stable hierarchy.

Unknowns, assumptions and credible conflicts must be explicit rather than hidden in prose.

## Consequences

### Positive

- Content research can proceed without continual architecture redesign.
- Decisions remain traceable to evidence and assumptions.
- Conflicting knowledge is preserved transparently.
- AI-generated origin remains auditable after verification.
- The system can scale without changing Object identity.
- Podcast production can use explicit readiness gates.

### Costs

- Existing legacy Objects may not yet contain every v1.0 metadata field.
- Migration will be gradual as Objects are revisited; no mass rewrite is required unless it provides research value.
- Researchers must explicitly manage Questions, Assumptions and Conflicts when material.

## Migration Rule

Do not stop content research to retrofit every existing file immediately.

New or materially updated Objects should use the v1.0 model. Older Objects should be upgraded opportunistically during normal research and Quality Gates.

## Architecture Freeze Rule

Routine content additions, new Modules, new Claims and new Relationships should fit inside v1.0.

Future changes to hierarchy levels, top-level object types, provenance semantics, evidence-maturity semantics or core graph behavior require a new ADR with migration impact analysis.

## Deferred Layers

The following remain Post-v1 consumers of the Data Hub and are not part of this architecture baseline:

- Manufacturing Atlas
- Engineering Toolkit
- Learning Paths / role-based roadmaps
- Interactive Decision Engine

## Rationale

The architecture is now sufficiently expressive for the project’s stated goal. Further architectural ideation has lower expected value than expanding, verifying and connecting the engineering knowledge needed by the podcast.