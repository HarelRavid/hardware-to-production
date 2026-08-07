# ADR-002 — Engineering Claims as Atomic Evidence-Bearing Knowledge

Status: Accepted

Date: 2026-08-07

## Context

The Knowledge OS was originally structured primarily around durable Knowledge Objects connected by typed relationships. During early Prototype Workshop research, it became clear that an Object such as `FDM / FFF Printing` contains many independent engineering assertions with different evidence, scope, confidence, limitations and decision relevance.

Treating the whole Object as one evidence-bearing unit would make contradictions, manufacturer-specific limits, context-dependent numerical data and decision support difficult to manage.

## Decision

Knowledge Objects remain the durable organizational nodes of the graph, but **Engineering Claims become the atomic evidence-bearing knowledge units**.

The system shall use the following reasoning stack:

`Engineering Question → Decision → Engineering Claims → Knowledge Objects → Sources`

Sources are evidence inputs. They are not themselves the final knowledge product.

## Consequences

1. Each important engineering assertion may receive a stable Claim ID.
2. Claims can be independently supported, contradicted, refined, limited or superseded.
3. Claims preserve application context and exceptions.
4. Decision trees can cite explicit Claims rather than relying on prose pages.
5. Numerical values must retain test/process/material context.
6. Knowledge Objects become containers and relationship hubs rather than monolithic evidence units.
7. Existing Object content remains valid; it will progressively be decomposed into claims during research, not rewritten all at once.
8. Podcast scripts should ultimately be traceable through claims to sources.

## Alternatives Considered

### Objects only
Rejected because independent assertions inside an Object may have different evidence quality or scope.

### Source-centered database
Rejected because the project goal is engineering understanding and decisions, not bibliography management.

### Free-form notes
Rejected because they cannot reliably support graph reasoning, contradictions, updates or listener navigation.

## Governance

The canonical models are maintained in:

- `ENGINEERING_CLAIM_MODEL.md`
- `ENGINEERING_DECISION_MODEL.md`
- `RELATIONSHIP_MODEL.md`
- `RESEARCH_WORKFLOW.md`

Major changes to Claim semantics require a new ADR.
