# Hardware to Production — Project Brain

**Knowledge OS Baseline: v1.0**

## 1. Mission

Build a rigorous, practical podcast about the transition from hardware development to scalable manufacturing.

The podcast is the primary public product. The Knowledge OS / Data Hub is the research engine, memory system, decision-support layer, and single source of truth that makes the podcast reliable, consistent, and expandable.

## 2. Product Order

1. Knowledge OS / Data Hub
2. Podcast
3. Engineering Toolkit
4. Learning Paths
5. Manufacturing Atlas / interactive navigation layers (Post-v1)

The Toolkit, Learning Paths, Manufacturing Atlas and interactive Decision Engine are intentionally deferred until the Data Hub and podcast knowledge base are mature.

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

The Knowledge OS must give a listener enough depth to continue learning after an episode without requiring new ad-hoc foundational research.

It must provide:

- clear definitions;
- engineering meaning and decision impact;
- lifecycle context;
- standards and regulations;
- academic and professional literature;
- industrial best practices;
- books, courses and technical guides;
- case studies;
- methods, machines, materials and software;
- common mistakes, myths and limitations;
- engineering decisions and decision logic;
- evidence-bearing engineering claims;
- open questions and unresolved uncertainty;
- engineering assumptions;
- knowledge conflicts;
- relationships to other objects;
- stable podcast tags for listener navigation.

## 6. Stable Knowledge Hierarchy

The organizational hierarchy is:

**Knowledge Layer → Domain → Module → Knowledge Object**

Knowledge Objects are durable graph nodes with stable IDs. A Domain may contain multiple Modules; a Module groups related Objects without changing Object identity.

The evidence and reasoning hierarchy is:

**Engineering Question → Engineering Decision → Engineering Claim → Knowledge Object → Source**

Objects organize knowledge. Claims assert knowledge. Sources support claims. Decisions consume claims. Questions define the user need the system must answer.

The system is a knowledge-and-decision graph, not a folder-based wiki.

## 7. Object Types — v1.0

The controlled top-level object vocabulary is:

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

New object types require an ADR. New Objects inside existing types do not normally require an ADR.

## 8. Major Domains

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

## 9. Lifecycle Axis

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
- Bridge Production
- Ramp-up
- Serial / Mass Production
- Sustainment
- End of Life

Lifecycle terminology varies by industry. The Knowledge OS must distinguish formal standards from common industry shorthand.

## 10. Object Status

Knowledge Objects use the following work-state model:

`Draft → Researching → Verified → Referenced → Podcast Ready → Published → Archived`

`Verified` means the important factual content has been checked against suitable evidence. `Referenced` means the evidence is traceable in the Object/Claims. `Podcast Ready` is governed by `DEFINITION_OF_DONE.md`.

## 11. Evidence Classification

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

## 12. Evidence Maturity

Evidence maturity is recorded separately from workflow status:

- L0 — Concept / unverified working knowledge
- L1 — supported by at least one suitable external source
- L2 — supported by multiple independent suitable sources
- L3 — supported or bounded by applicable standards / normative guidance where such guidance exists
- L4 — externally validated in relevant industrial practice or strong case evidence
- L5 — mature, widely accepted engineering principle within its stated scope

Maturity is not a quality score and must not be inflated merely by source count.

## 13. Provenance and GNR

Every AI-originated Object, Claim, Decision, Relationship or synthesis must preserve `GNR` in its provenance metadata.

`GNR` means **Generated**. It records origin, not truth value.

External evidence may be added alongside it, for example:

`provenance: [GNR, STD, PPR, GOV]`

The `GNR` marker is never removed simply because the content was later verified. A Claim supported only by `GNR` cannot be treated as Podcast Ready evidence.

Detailed provenance rules are governed by ADR-003.

## 14. Source Priority

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

## 15. Project Principles

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
15. The Data Hub must remain understandable independently of the podcast.
16. Every significant engineering recommendation should be traceable to Claims and evidence.
17. Numerical values must retain their material, process, test and environmental context.
18. Decision logic must distinguish evidence-backed rules from Project Heuristics.
19. Questions drive research; Domains organize the resulting knowledge.
20. Unknowns are explicit knowledge: Open Questions are preserved rather than hidden.
21. Assumptions must never be presented as facts.
22. Conflicting evidence must be preserved as Knowledge Conflicts until scope or evidence resolves it.

## 16. Research Rule

Do not collect information into an undefined bucket.

Before research begins, define target Objects, Engineering Questions and research questions. New discoveries may create new Objects, Claims, Open Questions, Assumptions or Knowledge Conflicts, but they must immediately be classified and linked.

For every meaningful source, ask:

1. Which Engineering Claims does it support?
2. Which existing Claims does it refine, limit or contradict?
3. Under what conditions are those Claims valid?
4. Which engineering decisions can use those Claims?
5. Which Open Questions does it resolve or create?

A source is an evidence input, not the final knowledge output.

## 17. Question-Driven Rule

Every Domain and major Module maintains a `Questions Answered` section.

Questions should reflect real engineering work, for example:

- When should this process be selected?
- Which material or process is appropriate under these constraints?
- Why did this failure occur?
- Which validation is needed before the next lifecycle gate?
- What changes when moving from prototype to serial production?

Questions are navigation and research drivers; they do not replace the stable Domain/Module/Object hierarchy.

## 18. Open Questions

Open Questions are first-class records. They must contain, where applicable:

- question;
- status;
- current evidence;
- confidence in the current working answer;
- related Objects/Claims/Decisions;
- research gap;
- resolution when closed.

A known unknown is preferable to an unsupported answer.

## 19. Engineering Assumptions

Engineering Assumptions are explicit statements used when required information is unavailable or intentionally fixed for analysis.

Examples include forecast volume, service life, environment, duty cycle or target cost.

Assumptions must be linked to the Decisions, Claims or calculations that depend on them and must be invalidated/reviewed when their underlying condition changes.

## 20. Knowledge Conflicts

Credible conflicting guidance is preserved rather than collapsed into one answer.

A Knowledge Conflict records:

- competing Claims;
- source/evidence for each position;
- applicability context;
- likely reason for disagreement;
- current resolution or `Unresolved` status.

When possible, resolve conflicts by narrowing scope rather than declaring one universal winner.

## 21. Claim Rule

Engineering Claims are the atomic evidence-bearing units of the Knowledge OS.

Each validated Claim must preserve:

- a clear statement;
- classification;
- confidence;
- evidence maturity;
- provenance (including GNR when applicable);
- applicable context;
- limitations and exceptions where known;
- related Objects;
- evidence;
- decision relevance where applicable.

Contradictory Claims are preserved rather than silently merged.

## 22. Relationship Rule

A relationship is not merely a hyperlink. It is a claim about the relationship between entities.

Every relationship must have:

- a predefined relationship type;
- direction;
- target object/entity;
- short reason;
- evidence/source where appropriate;
- confidence;
- strength/importance;
- provenance, including GNR when AI-originated.

Whenever possible, an inverse relationship should be defined automatically or explicitly.

## 23. Engineering Decision Rule

The Knowledge OS must answer `Given my situation, what should I do?`, not only `What is X?`.

Decision Objects shall define inputs, assumptions, constraints, candidate options, tradeoffs, supporting Claims, exceptions and escalation paths.

Decision-tree branches must be traceable to Claims or explicitly marked Project Heuristics.

Detailed rules are maintained in `ENGINEERING_DECISION_MODEL.md`.

## 24. Definition of Podcast Readiness

A topic is not ready because enough links were collected. It becomes Podcast Ready only after it has sufficient evidence, context, Claims, relationships and practical decision understanding to support a strong episode without substantial new foundational research.

Detailed criteria are maintained in `DEFINITION_OF_DONE.md`.

## 25. Listener Navigation

Every podcast episode will reference stable Knowledge OS tags, Objects or question/decision entry points. Navigation must therefore be designed for long-term listener use and not merely episode-specific organization.

## 26. Quality Gates

Before a major Domain/Section is considered complete, perform a Knowledge Integrity Review covering:

- duplicate concepts;
- orphan Objects;
- unsupported Claims;
- Decision branches without evidence or explicit heuristic labels;
- unresolved Knowledge Conflicts;
- hidden assumptions;
- missing lifecycle links;
- missing listener questions/tags;
- substantial foundational research gaps.

## 27. Post-v1 Backlog

Deferred until the full Data Hub and podcast knowledge base are complete:

- Manufacturing Atlas
- Engineering Toolkit
- Learning Paths / role-based roadmaps
- Interactive Decision Engine
- audience-specific navigation maps

These layers consume the Data Hub; they do not redefine it.

## 28. Change Governance / Architecture Freeze

This file is the project constitution.

Knowledge OS v1.0 is the stable baseline. Routine content work must not modify the architecture.

A future architectural change requires an ADR describing the problem, alternatives, reason and migration impact before changing the baseline.

ADR-002 established Engineering Claims as the atomic evidence-bearing knowledge unit. ADR-003 established GNR provenance and AI traceability. The v1.0 baseline freezes the hierarchy, core object types, provenance policy, uncertainty/conflict handling and readiness model.