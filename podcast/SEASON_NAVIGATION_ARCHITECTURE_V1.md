# Season & Listener Navigation Architecture V1

status: BASELINED FOR EPISODE PACKAGING
purpose: Convert the 68-episode canonical roadmap into approachable listener-facing seasons and navigation paths without duplicating or fragmenting the technical backbone.

## 1. Principle

The canonical roadmap remains 68 episodes, but listeners should never be required to experience it as one 68-step linear course.

Navigation is built on two simultaneous dimensions:

1. **Season / topic journey** — a coherent learning arc that can be marketed and consumed independently.
2. **Lifecycle / audience journey** — DEV → LVP → SVP, allowing a listener to enter at the maturity level closest to the problem they currently have.

Every season must have a short orientation/trailer that explains required frameworks and points to prerequisite material instead of forcing full-series listening.

## 2. Primary listener routes

### Route A — Founder / early hardware developer
Start: Opening Arc A1.
Goal: understand what must be designed, documented and learned now so a successful prototype does not become manufacturing debt.
Default journey: DEV-heavy opening → product/architecture/DFX → prototype-to-production transition → selected quality/supplier/process episodes.

### Route B — Team with a working prototype
Start: Episode 1 or the season containing prototype-to-production transition.
Goal: identify prototype shortcuts, their expiration conditions, and the controls/evidence required for tens/hundreds of units.
Default journey: LVP transition → configuration → quality → process → supplier → pilot/ramp.

### Route C — New NPI / industrialization / production team
Start: NPI/industrialization season orientation.
Goal: establish controlled initial production, upgrade prototype solutions into industrial solutions and prepare scalable production evidence.
Default journey: configuration/change → quality chain → process qualification → supplier → capacity/ramp → automation/data.

### Route D — Specialist / problem-driven listener
Start directly at the relevant season/episode.
Goal: solve a current problem without consuming the entire curriculum.
Requirement: every specialist entry point gets a concise prerequisite recap and links to foundational frameworks.

## 3. Listener-facing season model

Exact episode IDs may be editorially adjusted during packaging; the technical mappings remain canonical.

### Season 1 — From Idea to Manufacturable Hardware
Primary audience: A
Lifecycle: DEV
Question: What should we do while developing the product so manufacturing does not become a late surprise?
Includes the Opening Arc and early product/readiness foundations.
Exit capability: listener can distinguish proof-of-concept success from product/manufacturing readiness and identify the manufacturing debt being created.

### Season 2 — Prototype to Controlled Production
Primary audience: A + B
Lifecycle: DEV → LVP
Question: The prototype works; what changes before we build tens or hundreds?
Focus: configuration, BOM/revisions, DFX, process definition, CTQs, test strategy, initial supplier and quality controls.
Exit capability: listener can define the minimum controlled production system for LVP.

### Season 3 — Manufacturing Processes & Industrial Methods
Primary audience: B + specialist
Lifecycle: DEV/LVP/SVP depending process
Question: How do manufacturing processes actually work, what do they control, and when should each be selected?
Focus: process families, materials, tooling, special processes, electronics manufacturing and process-specific standards.
Exit capability: listener can ask the correct process-selection, capability, qualification and supplier questions.

### Season 4 — Quality, Reliability & Evidence
Primary audience: A + B
Lifecycle: LVP → SVP
Question: How do we prove that the product and process are consistently good rather than merely seeing good units?
Focus: CTQ, PFMEA, Control Plan, MSA, SPC, capability, reliability/qualification, NCR/CAPA, field evidence and effectiveness.
Exit capability: listener can build an evidence chain from risk/requirement to production and field learning.

### Season 5 — Suppliers, NPI & Production Ramp
Primary audience: B
Lifecycle: LVP → SVP
Question: How do we move from a capable prototype supply chain to repeatable commercial production?
Focus: supplier industrialization, FAI/PPAP where applicable, sub-tier control, pilot/PVT, Run-at-Rate, bottlenecks, WIP, accepted throughput and ramp exit.
Exit capability: listener can distinguish supplier approval, process approval and sustainable system capacity.

### Season 6 — Automation & Manufacturing Economics
Primary audience: B + founders making scale decisions
Lifecycle: LVP → SVP
Question: What should we automate, when, and does the investment actually improve the production system?
Focus: automation ladder, qualification/recovery, machine safety, OEE/losses, CapEx/NRE, break-even, NPV, staged investment and moving constraints.
Exit capability: listener can evaluate automation as an engineering/economic intervention rather than a maturity badge.

### Season 7 — Digital Factory, Traceability & OT Security
Primary audience: B + operations/data/automation specialists
Lifecycle: LVP → SVP
Question: What manufacturing truth must be reconstructable, and how do we protect the connected production system?
Focus: Minimum Viable Manufacturing Atlas, genealogy, MES/ERP/PLM/QMS boundaries, ISA-95/IEC 62264, OPC UA context, OT/ICS architecture, IEC 62443, backup/recovery and remote access.
Exit capability: listener can define the minimum digital thread and security controls appropriate to manufacturing maturity.

### Season 8 — Scaling, Failures & Real-World Lessons
Primary audience: A + B
Lifecycle: cross-stage
Question: What breaks when real products and factories scale, and how do we learn without copying the wrong lesson?
Focus: cross-industry cases, field evidence loop, interaction claims, degraded production modes, corrective-action effectiveness, signal aggregation and system-level lessons.
Exit capability: listener can analyze industrial failures using the canonical frameworks and distinguish facts from transferred lessons.

## 4. Navigation tags on every episode

Every Episode Research Pack must expose listener-facing tags in addition to technical metadata:

- **Audience:** Founder/Developer | NPI/Production | Specialist | All
- **Stage:** DEV | LVP | SVP | Cross-stage
- **Track:** Product | Process | Quality | Supplier | Reliability | Automation | Economics | Data | OT Security | Case Study
- **Depth:** Foundation | Practitioner | Advanced
- **Entry point:** YES/NO
- **Prerequisite recap required:** YES/NO
- **Next recommended:** 1–3 episodes/routes

These tags are navigation metadata, not new technical taxonomy.

## 5. Season trailer/orientation contract

Each season gets a short orientation asset (target ~5 minutes, editorially adjustable) that:

1. states who the season is for;
2. states the production/lifecycle problem it solves;
3. explains where it sits in DEV/LVP/SVP;
4. introduces only the canonical frameworks required for that season;
5. gives a fast prerequisite recap;
6. explains which listeners may skip or enter midway;
7. gives 2–4 recommended entry points by listener situation;
8. previews the season's practical outputs/checklists.

A season trailer does not create new normative claims unless those claims enter the normal Claim Register.

## 6. Non-linear consumption rule

No episode may rely on “you had to listen to episode X” for a concept necessary to understand a consequential recommendation.

Instead:
- give a concise definition/recap;
- link the foundational episode for depth;
- state the prerequisite explicitly in the research pack;
- avoid repeating the full lesson.

This allows the series to function both as a narrative podcast and as a searchable manufacturing reference library.

## 7. DEV/LVP/SVP navigation inside episodes

Where relevant, show chapter markers or show-note navigation for:

- **DEV — Do now / learn now**
- **Prototype shortcut — acceptable temporarily**
- **Expiration trigger — when the shortcut stops being acceptable**
- **LVP — control required for tens/hundreds**
- **SVP — evidence/system required for commercial scale**

This structure should be visible enough that listeners can jump to their maturity stage without losing the episode's core logic.

## 8. Cross-season framework reuse

Canonical frameworks remain shared infrastructure. Seasons must not create local substitutes for:

- Hardware Evolution Ladder
- DEV/LVP/SVP Lens
- QUALITY CHAIN 8
- CHANGE 9
- RATE 8 / RAMP 10
- ECON 10
- SUPPLIER 10
- AUTOMATE 10 / LOSS 8 / RELEASE 12
- TRACE 10 / ATLAS 10 / RECONSTRUCT 8
- SECURITY 12 / SECURE RELEASE 12
- CASE 12

A trailer may recap a framework in simplified language but must retain its canonical mapping.

## 9. Pilot packaging implication

The first five Episode Research Packs should deliberately test different navigation paths:

- **A1** — Season 1 / Founder entry point / DEV.
- **A4** — Season 1 / early-team foundation / DEV.
- **Episode 1** — Season 2 / working-prototype entry point / DEV→LVP.
- **Episode 23** — Quality/process specialist entry / LVP→SVP / standards-heavy test.
- **Episode 29** — quantitative/production decision entry / LVP→SVP.

For each pilot pack, verify both technical contract compliance and navigation usability.

## 10. Success test

The navigation architecture passes if a listener can answer:

1. Where should I start given my role and product maturity?
2. Which season solves my current problem?
3. Can I enter without listening to dozens of prior episodes?
4. What prerequisite knowledge do I actually need?
5. What should I do differently in DEV, LVP and SVP?
6. Where do I go next if I need deeper quality/process/supplier/automation/data knowledge?

If these answers are not obvious from episode/season metadata and show notes, packaging has failed even if the technical content is correct.

## 11. Relationship to Knowledge Backbone V1 freeze

This document does not reopen the frozen technical backbone. It is listener/navigation architecture built on top of the baseline.

Allowed editorial evolution:
- season names;
- exact episode grouping;
- trailers;
- navigation tags;
- recommended routes;
- episode order where technical dependencies remain intact.

Structural technical changes still follow the post-freeze change-control rule.

## 12. Next action

Build the five Pilot Episode Research Packs using both:
- `podcast/EPISODE_PACKAGING_CONTRACT.md`
- this Season & Listener Navigation Architecture.

Use the pilot to validate the production workflow before opening the remaining episode packs in waves.
