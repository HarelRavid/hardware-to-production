# Hardware to Production — Project Brain

## 1. Mission

Build a rigorous, practical podcast about the transition from hardware development to scalable manufacturing.

The podcast is the primary product. The Knowledge OS / Data Hub is the research engine, memory system, and single source of truth that makes the podcast reliable, consistent, and expandable.

## 2. Product Order

1. Knowledge OS / Data Hub
2. Podcast
3. Engineering Toolkit
4. Learning Paths

The Toolkit and Learning Paths are intentionally deferred until the podcast and its supporting knowledge base are mature.

## 3. Core Principle

**The podcast is derived from the Knowledge OS. The Knowledge OS is never reshaped merely to fit an episode.**

Every episode must be supportable from existing, validated Knowledge OS objects before it is written.

## 4. Podcast Scope

The first season is expected to contain roughly 30–40 practical episodes organized into three major internal sections:

1. Prototype Workshop — building and operating in-house development manufacturing capability.
2. Designing Products for Manufacturing — DFM/DFX and product maturation toward production.
3. NPI & Industrialization — complete transition from mature design through pilot, ramp-up, automation and stable production.

The final episode count may change only after the Knowledge OS shows the true natural boundaries between topics.

## 5. Knowledge OS Purpose

The Knowledge OS must give a listener enough depth to continue learning after an episode without requiring new ad-hoc research.

It must provide:

- clear definitions;
- lifecycle context;
- standards and regulations;
- academic and professional literature;
- industrial best practices;
- books, courses and technical guides;
- case studies;
- methods, machines, materials and software;
- common mistakes and limitations;
- relationships to other objects;
- stable podcast tags for listener navigation.

## 6. Knowledge Architecture

Knowledge is structured as:

**Domain → Subdomain → Topic → Knowledge Object**

Each Knowledge Object is a durable node with a stable ID and typed relationships to other nodes.

The system is a knowledge graph, not a folder-based wiki.

## 7. Major Domains

1. Product Development
2. Prototype Workshop
3. Manufacturing Processes
4. Materials Engineering
5. Design for X
6. Manufacturing Engineering
7. Quality Engineering
8. NPI & Industrialization
9. Factory Design
10. Automation
11. Supply Chain
12. Business & Manufacturing Strategy
13. Regulations & Standards
14. Case Studies
15. Engineering Management

## 8. Lifecycle Tags

Objects may be associated with one or more lifecycle stages:

- Concept
- POC
- Prototype
- Engineering Prototype
- MVP
- Alpha
- Beta
- EVT
- DVT
- PVT
- Pilot
- Ramp-up
- Mass Production
- Sustainment
- End of Life

Lifecycle terminology varies by industry. The Knowledge OS must distinguish formal standards from common industry shorthand.

## 9. Evidence Classification

Every important claim should be identifiable as one of:

- Standard / Regulation
- Verified Fact
- Academic Evidence / Consensus
- Industrial Best Practice
- Expert Opinion
- Project Synthesis / Recommendation

These categories must not be silently mixed.

## 10. Source Priority

Preferred source hierarchy:

1. Standards, regulations and normative bodies
2. Government and research institutes
3. Universities and academic institutions
4. Peer-reviewed literature
5. Authoritative professional books and handbooks
6. Industry associations and high-quality manufacturer technical literature
7. Courses, conference material and expert lectures
8. Professional experience, specialist blogs and forums

Lower-tier sources may be extremely useful, but they do not override higher-authority evidence without explicit justification.

## 11. Project Principles

1. Knowledge before content.
2. Structure before research.
3. Evidence before opinion.
4. One authoritative home for each concept.
5. No orphan knowledge objects.
6. Prefer systems thinking over isolated facts.
7. Explain where every topic sits in the product lifecycle.
8. Separate what is mandatory from what is recommended.
9. Preserve contradictions and disagreements when evidence conflicts.
10. Optimize for correctness, clarity and maintainability rather than speed.
11. Keep IDs and relationships stable even when wording evolves.
12. Every listener must be able to discover where to continue learning.
13. Every significant architectural decision must be documented.
14. The Knowledge OS should outlive the first podcast season.
15. The Data Hub should remain understandable independently of the podcast.

## 12. Research Rule

Do not collect information into an undefined bucket.

Before research begins, define the target objects and research questions. New discoveries may create new objects, but those objects must immediately be classified and linked.

## 13. Relationship Rule

A relationship is not merely a hyperlink. It is a claim.

Every relationship must have:

- a predefined relationship type;
- direction;
- target object;
- short reason;
- evidence/source where appropriate;
- confidence;
- strength/importance.

Whenever possible, an inverse relationship should be defined automatically or explicitly.

## 14. Definition of Podcast Readiness

A topic is not ready because enough links were collected. It becomes Podcast Ready only after it has sufficient evidence, context, relationships and practical understanding to support a strong episode without substantial new foundational research.

Detailed criteria are maintained in `DEFINITION_OF_DONE.md`.

## 15. Listener Navigation

Every podcast episode will reference stable Knowledge OS tags or object IDs. Tags must therefore be designed for long-term listener navigation and not merely episode-specific organization.

## 16. Prototype Workshop Priority

The first deep research domain is the Prototype Workshop because it supports the earliest section of the podcast and bridges development engineering with manufacturing capability.

It includes in-house rapid manufacturing, workshop design, additive manufacturing, CNC, turning, laser cutting, sheet metal, electronics prototyping, cable/harness work, joining, measurement, fixtures, workshop management, and make-vs-buy decisions.

## 17. Change Governance

This file is the project constitution. It should change rarely.

When a major architectural choice changes, create an Architecture Decision Record (ADR) describing the decision, reason, alternatives and consequences before altering the system.