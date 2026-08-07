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

Every episode must be supportable from existing, validated Knowledge OS content before it is written.

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
- engineering decisions and decision logic;
- evidence-bearing engineering claims;
- relationships to other objects;
- stable podcast tags for listener navigation.

## 6. Knowledge Architecture

The organizational hierarchy is:

**Domain → Subdomain → Topic → Knowledge Object**

Knowledge Objects are durable graph nodes with stable IDs.

The evidence and reasoning hierarchy is:

**Engineering Question → Engineering Decision → Engineering Claim → Knowledge Object → Source**

Objects organize knowledge. Claims assert knowledge. Sources support claims. Decisions consume claims.

The system is a knowledge-and-decision graph, not a folder-based wiki.

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

Objects, Claims and Decisions may be associated with one or more lifecycle stages:

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

Every important Claim should be identifiable as one of:

- Normative Requirement
- Verified Fact
- Academic Evidence
- Academic Consensus
- Industrial Best Practice
- Manufacturer-Specific Guidance
- Expert Opinion
- Project Synthesis
- Project Heuristic

These categories must not be silently mixed.

Detailed rules are maintained in `ENGINEERING_CLAIM_MODEL.md`.

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
5. No orphan Knowledge Objects.
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
16. Every significant engineering recommendation should be traceable to Claims and evidence.
17. Numerical values must retain their material, process, test and environmental context.
18. Decision logic must distinguish evidence-backed rules from Project Heuristics.

## 12. Research Rule

Do not collect information into an undefined bucket.

Before research begins, define target Objects, Engineering Questions and research questions. New discoveries may create new Objects or Claims, but they must immediately be classified and linked.

For every meaningful source, ask:

1. Which Engineering Claims does it support?
2. Which existing Claims does it refine, limit or contradict?
3. Under what conditions are those Claims valid?
4. Which engineering decisions can use those Claims?

A source is an evidence input, not the final knowledge output.

## 13. Claim Rule

Engineering Claims are the atomic evidence-bearing units of the Knowledge OS.

Each validated Claim must preserve:

- a clear statement;
- classification;
- confidence;
- applicable context;
- limitations and exceptions where known;
- related Objects;
- evidence;
- decision relevance where applicable.

Contradictory Claims are preserved rather than silently merged.

## 14. Relationship Rule

A relationship is not merely a hyperlink. It is a claim about the relationship between entities.

Every relationship must have:

- a predefined relationship type;
- direction;
- target object/entity;
- short reason;
- evidence/source where appropriate;
- confidence;
- strength/importance.

Whenever possible, an inverse relationship should be defined automatically or explicitly.

## 15. Engineering Decision Rule

The Knowledge OS must answer `Given my situation, what should I do?`, not only `What is X?`.

Decision Objects shall define inputs, constraints, candidate options, tradeoffs, supporting Claims, exceptions and escalation paths.

Decision-tree branches must be traceable to Claims or explicitly marked Project Heuristics.

Detailed rules are maintained in `ENGINEERING_DECISION_MODEL.md`.

## 16. Definition of Podcast Readiness

A topic is not ready because enough links were collected. It becomes Podcast Ready only after it has sufficient evidence, context, Claims, relationships and practical decision understanding to support a strong episode without substantial new foundational research.

Detailed criteria are maintained in `DEFINITION_OF_DONE.md`.

## 17. Listener Navigation

Every podcast episode will reference stable Knowledge OS tags, Objects or question/decision entry points. Navigation must therefore be designed for long-term listener use and not merely episode-specific organization.

## 18. Prototype Workshop Priority

The first deep research domain is the Prototype Workshop because it supports the earliest section of the podcast and bridges development engineering with manufacturing capability.

It includes in-house rapid manufacturing, workshop design, additive manufacturing, CNC, turning, laser cutting, sheet metal, electronics prototyping, cable/harness work, joining, measurement, fixtures, workshop management, and make-vs-buy decisions.

## 19. Change Governance

This file is the project constitution. It should change rarely.

When a major architectural choice changes, create an Architecture Decision Record (ADR) describing the decision, reason, alternatives and consequences before altering the system.

ADR-002 established Engineering Claims as the atomic evidence-bearing knowledge unit while preserving Knowledge Objects as durable organizational nodes.