# ADR-001 — Knowledge OS Architecture

- Status: Accepted
- Date: 2026-08-07

## Context

The Hardware to Production project requires a research foundation that can support dozens of podcast episodes without being repeatedly restructured during writing.

A conventional wiki or folder tree would organize pages but would not preserve enough semantic meaning between concepts.

## Decision

The Data Hub will be implemented conceptually as a Knowledge Operating System composed of stable Knowledge Objects connected by typed, directional, evidence-aware Relationships.

The podcast is the primary public product. The Knowledge OS is the single source of truth used to create it.

Knowledge architecture is independent of episode architecture.

## Consequences

- Each concept receives one stable object identity.
- Relationships are treated as claims rather than generic hyperlinks.
- Research builds the graph while evidence is collected.
- Major architectural changes require ADRs.
- Episode writing begins only after supporting objects meet Podcast Ready criteria.
- Future Toolkit and Learning Path layers may reuse the same objects without restructuring the core knowledge model.

## Alternatives Considered

### Folder-based Wiki

Rejected as the primary model because folder placement alone cannot represent cross-domain engineering dependencies.

### Episode-first Research

Rejected because it encourages duplication, missing context and repeated restructuring.

### Unstructured Source Library

Rejected because accumulating PDFs/links does not create reusable engineering knowledge.