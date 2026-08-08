# Knowledge Object Model

**Baseline: v1.0**

## 1. Purpose

A Knowledge Object is the smallest durable organizational unit of the Hardware to Production Knowledge OS. Objects are nodes in the knowledge graph; they are not merely pages or files.

Engineering Claims remain the atomic evidence-bearing units. Objects organize those Claims and connect them to Decisions, Questions, lifecycle context and Sources.

## 2. Stable Hierarchy

**Knowledge Layer → Domain → Module → Knowledge Object**

The hierarchy organizes navigation. Stable Object IDs preserve identity even when a Module or navigation path changes.

## 3. Controlled Top-Level Object Types

Knowledge OS v1.0 recognizes:

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

A Knowledge Object may use a more specific semantic subtype in metadata (for example Process, Material, Machine, Tool, Method, KPI, Role, Software, Test Method), but new top-level architectural object types require an ADR.

## 4. Mandatory Metadata

```yaml
id: H2P-XXXXXX
title:
aliases: []
object_type: Knowledge Object
semantic_type:
domain:
module:
knowledge_path:
lifecycle: []
status: Draft
evidence_maturity: L0
provenance: [GNR]
summary:
tags: []
questions_answered: []
related_decisions: []
open_questions: []
assumptions: []
knowledge_conflicts: []
created:
last_reviewed:
```

`GNR` must remain in provenance for AI-originated content even after validation.

## 5. Knowledge Status

Controlled work-state progression:

`Draft → Researching → Verified → Referenced → Podcast Ready → Published → Archived`

Status describes workflow/maturity of the Object as a usable knowledge artifact. Evidence Maturity is a separate field and must not be inferred from status.

## 6. Evidence Maturity

- L0 — concept / unverified working knowledge
- L1 — supported by at least one suitable external source
- L2 — multiple independent suitable sources
- L3 — supported or bounded by applicable standards / normative guidance where such guidance exists
- L4 — relevant industrial validation or strong case evidence
- L5 — mature, widely accepted engineering principle within its stated scope

## 7. Core Content Structure

Every mature Object should contain, when applicable:

1. Definition
2. Engineering Meaning
3. Decision Impact
4. Purpose / Problem Solved
5. Lifecycle Position
6. Typical Owner / Responsible Role
7. Inputs / Preconditions
8. Outputs / Deliverables
9. How It Works
10. Decision Criteria / Tradeoffs
11. Limitations / Applicability
12. Failure Modes / Common Mistakes
13. Standards / Regulations
14. Academic Evidence
15. Professional Books / Handbooks
16. Industrial Guidance
17. Case Studies
18. Engineering Claims
19. Typed Relationships
20. Questions Answered
21. Open Questions / Evidence Gaps
22. Engineering Assumptions
23. Knowledge Conflicts
24. Listener Tags / Podcast Mapping
25. Future Toolkit Mapping — reserved, not developed in v1
26. Future Learning Path / Atlas Mapping — reserved, not developed in v1

Not every Object requires every section. `Not applicable` is preferable to padding with low-value content.

## 8. Questions Answered

Every mature Object should identify the real engineering questions it helps answer. Questions are navigation/research entry points and do not replace the stable hierarchy.

Examples:

- When should this process be selected?
- What causes this failure mode?
- Which design constraints control this decision?
- What must be validated before scale-up?

## 9. Open Questions

Known unknowns should be explicit rather than hidden in prose. Open Questions should link to relevant Claims, Sources and Decisions and record the evidence gap that prevents closure.

## 10. Engineering Assumptions

Assumptions such as annual volume, service life, duty cycle, environmental exposure or target cost must be represented explicitly when they materially affect an Object or Decision.

An assumption changing should trigger reevaluation of dependent Decisions/Claims.

## 11. Knowledge Conflicts

When credible Sources or Claims disagree, preserve the conflict. A mature Object should link to a Knowledge Conflict record rather than silently select one position without explaining context.

## 12. Stable Identity

Object IDs do not change when titles, navigation paths or terminology change.

Aliases capture alternate terminology. `knowledge_path` is navigational and may change; `id` is identity and must remain stable.

## 13. No Orphan Objects

A mature Object should normally have multiple meaningful graph relationships. Foundational Objects may temporarily have fewer.

Relationships exist because of engineering meaning, not to satisfy a numerical target.

## 14. Object Granularity

Create a separate Object when the concept can reasonably:

- have its own definition;
- have different lifecycle relevance;
- have different evidence;
- be independently referenced by multiple other Objects;
- support a distinct Decision;
- or support a distinct podcast discussion.

Do not fragment trivial synonyms into separate Objects.

## 15. Provenance Rule

All AI-originated Objects include `GNR`. External verification adds provenance codes; it does not erase origin.

Object prose may summarize external evidence, but episode-critical engineering assertions should be expressed as Claims with traceable evidence.

## 16. Versioning and Architecture Freeze

Content evolves; identity remains stable.

Knowledge OS v1.0 freezes the hierarchy, core object types, status model, provenance policy and explicit representation of Questions, Assumptions and Conflicts. Future architectural changes require an ADR.