# Knowledge Object Model

## 1. Purpose

A Knowledge Object is the smallest durable unit of the Hardware to Production Knowledge OS. Objects are nodes in the knowledge graph. They are not merely pages or files.

Every object has a stable ID, a defined type, metadata, evidence, and typed relationships to other objects.

## 2. Object Types

Initial controlled vocabulary:

- Concept
- Principle
- Method
- Process
- Lifecycle Stage
- Deliverable
- Document
- Standard
- Regulation
- Requirement
- Machine
- Equipment
- Tool
- Software
- Material
- Manufacturing Process
- Test Method
- Measurement Method
- Formula
- KPI
- Role
- Organization
- Risk
- Failure Mode
- Case Study
- Source
- Checklist
- Template
- Podcast Episode

New object types require an ADR if they materially alter the model.

## 3. Mandatory Metadata

```yaml
id: H2P-XXXXXX
title:
aliases: []
object_type:
domain:
subdomain:
lifecycle: []
status:
summary:
tags: []
created:
last_reviewed:
```

## 4. Knowledge Status

Controlled state progression:

Idea → Mapped → Researching → Draft → Reviewed → Validated → Podcast Ready → Published

A status change should represent a real maturity increase, not editorial progress alone.

## 5. Core Content Structure

Every mature object should contain, when applicable:

1. Definition
2. Purpose
3. Problem Solved
4. Lifecycle Position
5. Typical Owner / Responsible Role
6. Inputs / Preconditions
7. Outputs / Deliverables
8. How It Works
9. Decision Criteria
10. Limitations
11. Common Mistakes
12. Standards / Regulations
13. Academic Evidence
14. Professional Books / Handbooks
15. Industrial Guidance
16. Case Studies
17. Related Objects
18. Open Questions / Evidence Gaps
19. Podcast Mapping
20. Future Toolkit Mapping — reserved, not developed yet
21. Future Learning Path Mapping — reserved, not developed yet

Not every object requires every section. Empty sections should not be padded with low-value content.

## 6. Claim Classification

Important statements should be labeled or written so their evidence class is clear:

- normative requirement;
- verified fact;
- academic finding;
- industry practice;
- expert opinion;
- project synthesis/recommendation.

## 7. Stable Identity

Object IDs do not change when titles or terminology change.

Aliases capture alternate terminology. Example: an object may retain one stable ID while recognizing multiple industry terms for a lifecycle stage.

## 8. No Orphan Objects

A mature object should normally have at least three meaningful graph relationships. Foundational objects may temporarily have fewer.

Relationships exist because of engineering meaning, not to satisfy a numerical target.

## 9. Object Granularity

Create a separate object when the concept can reasonably:

- have its own definition;
- have different lifecycle relevance;
- have different evidence;
- be independently referenced by multiple other objects;
- or support a distinct podcast discussion.

Do not fragment trivial synonyms into separate objects.

## 10. Versioning

Content evolves, identity remains stable. Material changes in meaning, taxonomy or architectural behavior should be captured in ADRs.