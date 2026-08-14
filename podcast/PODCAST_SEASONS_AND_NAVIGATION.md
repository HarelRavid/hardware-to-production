# Podcast Seasons & Navigation Architecture

status: CANONICAL EDITORIAL NAVIGATION
version: 1.0
purpose: Make the 68-episode Hardware-to-Production roadmap easy to enter, navigate and consume without requiring a strictly linear listen from Episode A1 through Episode 60.

## 1. Principle

The canonical technical roadmap remains 68 episodes:
- Opening Arc A1–A8
- Core Episodes 1–60

Listener navigation is NOT required to mirror that numbering.

The published experience should be organized as seasons and optional learning paths so that a listener can enter at the correct maturity level and still understand prerequisites.

The navigation layer must never create duplicate engineering truth. It points into the same canonical episode/research-pack system.

## 2. Primary navigation model

Use three simultaneous navigation dimensions:

### Dimension A — Season
A bounded thematic journey that feels approachable and marketable.

### Dimension B — Lifecycle stage
- DEV — development/prototype
- LVP — low-volume initial production
- SVP — serial/commercial production
- CROSS-STAGE — relevant across the lifecycle

### Dimension C — Listener path
A role/problem-based route through selected episodes.

A listener may follow a whole season or a curated path.

## 3. Proposed season architecture

### Season 1 — Building Hardware That Can Grow Up
Primary audience: founders, early developers, first hardware teams.
Primary stages: DEV → early production intent.
Canonical episodes:
- A1 — From an Idea to Engineering Requirements
- A2 — The Hardware Team Map
- A3 — System Architecture and Interfaces
- A4 — Choosing Prototype Technologies Without Trapping the Product
- A5 — Mechanical Design for the First Serious Prototype
- A6 — Electronics, PCB and Embedded Hardware for the First Serious Prototype
- A7 — Development Verification Before Production Verification
- A8 — Configuration Management from Prototype #1
- 1 — The product works. Why can’t we manufacture it?
- 2 — POC, Prototype, MVP and Production-Intent Hardware
- 3 — What NPI and Industrialization Actually Own
- 4 — Product Readiness vs Manufacturing Readiness

Promise:
Help a team avoid creating manufacturing debt before its first real production build.

Independent entry point:
A1.

Fast entry for a team that already has a working prototype:
Episode 1.

### Season 2 — Designing the Product for Production
Primary audience: development + NPI teams.
Primary stages: DEV → production intent → LVP.
Canonical episodes:
- 5 — EVT, DVT, PVT, Pilot and Ramp Without the Buzzwords
- 6 — Design for Manufacturing
- 7 — Design for Assembly and Mistake Prevention
- 8 — Design for Test, Calibration and Traceability
- 9 — Tolerance, GD&T, Variation
- 10 — Designing for Reliability, Service and Repair

Promise:
Turn a functioning design into one that can survive variation, assembly, testing, service and scale.

Required recap:
Hardware Evolution Ladder + DEV/LVP/SVP in 2–4 minutes.

### Season 3 — How Things Are Actually Made
Primary audience: designers, process/manufacturing engineers, technical founders.
Primary stages: DEV/LVP/SVP decision transitions.
Canonical episodes:
- 11 — How to Select a Manufacturing Process
- 12 — Polymer Parts
- 13 — Metal Parts
- 14 — Joining
- 15 — Composite Manufacturing
- 16 — Ceramics, Powder Processing and Sintering
- 17 — Additive Manufacturing
- 18 — Surface Engineering, Cleaning and Heat Treatment
- 19 — Manufacturing Process Chains

Promise:
Choose manufacturing routes based on function, volume, quality, tooling, supplier maturity and cost per good part rather than familiarity or prototype convenience.

Independent entry point:
Episode 11.

### Season 4 — Building the First Real Production System
Primary audience: Audience B — early production/NPI/industrialization teams.
Primary stages: production intent → LVP.
Canonical episodes:
- 20 — EBOM to MBOM and Process Flow
- 21 — Tooling, Jigs, Fixtures and Production-Intent Equipment
- 22 — Work Instructions, Standard Work and Operator Qualification
- 23 — DFMEA, PFMEA, Control Plans and Quality Gates
- 24 — Production Testing and Measurement-System Capability
- 25 — Layout, Material Flow and Ergonomics

Promise:
Build tens or hundreds of units under control before over-investing in a full serial-production factory.

Independent entry point:
Episode 20.

### Season 5 — Pilot, Ramp and the Fight for Stable Output
Primary audience: NPI, manufacturing, operations and engineering managers.
Primary stages: LVP → production validation → ramp → SVP.
Canonical episodes:
- 26 — How to Plan a Pilot Build
- 27 — What a Production Validation Build Must Prove
- 28 — Yield, Rework, Scrap and the Learning Curve
- 29 — Capacity, Bottlenecks, Takt Time and Line Balance
- 30 — Supplier Readiness and Contract-Manufacturer Management
- 31 — Engineering Changes During Ramp-Up

Promise:
Distinguish finishing a batch from proving sustainable production capability.

Independent entry point:
Episode 26; Episode 29 may also stand alone with a short takt/capacity recap.

### Season 6 — Quality, Reliability and Evidence
Primary audience: quality, test, reliability, NPI and engineering leadership.
Primary stages: LVP → SVP; cross-stage principles also apply in DEV.
Canonical episodes:
- 32 — Process Capability and SPC
- 33 — Nonconformance, MRB, CAPA and Learning from Failure
- 34 — Reliability Validation and Production Reality
- 35 — Traceability, Genealogy and Evidence Retention
- 36 — Standards, Regulatory Requirements and Applicability

Promise:
Build evidence that tells you whether the process and product are actually trustworthy.

Independent entry point:
Episode 32 or 36 depending on listener need.

### Season 7 — Suppliers as Part of the Manufacturing System
Primary audience: supply chain, supplier quality, NPI, engineering and operations.
Primary stages: production intent → LVP → SVP.
Canonical episodes:
- 37 — Make or Buy?
- 38 — Selecting a Supplier by Capability
- 39 — RFQ Technical Package and First Production Approval
- 40 — Supplier Quality, Dual Sourcing and Resilience

Promise:
Turn purchasing relationships into controlled production capability.

Independent entry point:
Episode 37.

### Season 8 — Automation, Equipment and Scale Economics
Primary audience: manufacturing/process/automation engineers, founders and operations leaders.
Primary stages: LVP → SVP.
Canonical episodes:
- 41 — When Not to Automate
- 42 — Building the Business Case for Automation
- 43 — Automation Architecture and Integration
- 44 — Qualifying Production Equipment
- 45 — OEE, Downtime and Loss Analysis
- 46 — Maintenance, Recovery and Sustained Automation Performance

Promise:
Automate the real constraint only after process, safety, recovery and economics evidence justify it.

Independent entry point:
Episode 41.

### Season 9 — Manufacturing Data, Digital Thread and OT Security
Primary audience: manufacturing-data engineers, operations, quality, automation and technical leadership.
Primary stages: LVP → SVP; lightweight principles begin in DEV.
Canonical episodes:
- 47 — What Manufacturing Data Should Actually Exist?
- 48 — Product, Process, Equipment and Execution Identity
- 49 — Digital Thread and Genealogy
- 50 — MES, ERP, PLM, QMS and System-of-Record Boundaries
- 51 — Semantic Integration / ISA-95 / OPC UA
- 52 — OT/ICS Cybersecurity and Secure Manufacturing Operations

Promise:
Preserve manufacturing truth as the organization scales without turning a five-person startup into an enterprise-software project prematurely.

Independent entry point:
Episode 47.

### Season 10 — Failure, Scale and Real-World Lessons
Primary audience: both core audiences plus experienced practitioners.
Primary stages: CROSS-STAGE.
Canonical episodes:
- 53–60 — Cross-industry case studies and synthesis

Case selection should exercise:
- supplier/process failure;
- field evidence and recall;
- capacity/ramp failure;
- automation decisions;
- configuration/system interaction;
- OT/cyber recovery;
- quality-system corrective-action effectiveness;
- cross-domain failure propagation.

Promise:
Stress-test the frameworks against documented industrial reality rather than tidy textbook examples.

Independent entry point:
Episode 53 with a compact framework refresher.

## 4. Listener paths

Seasons are the public catalog structure. Listener paths are shortcuts.

### Path A — “I have an idea / early prototype and don’t know what comes next”
A1 → A2 → A3 → A4 → A7 → A8 → 1 → 3 → 6 → 8 → 20 → 23 → 26

Goal:
Create an end-to-end mental model without requiring all 68 episodes.

### Path B — “Our first prototype works; now we need to build 50–500”
1 → 2 → 3 → 5 → 6 → 7 → 8 → 20 → 21 → 22 → 23 → 24 → 26 → 28 → 29 → 30 → 31 → 35

Primary audience:
Audience B.

### Path C — “I’m building the quality system”
8 → 23 → 24 → 28 → 32 → 33 → 34 → 35 → 36 → 39 → 40

### Path D — “We need to scale capacity and automate”
21 → 25 → 27 → 28 → 29 → 41 → 42 → 43 → 44 → 45 → 46

### Path E — “I manage suppliers / contract manufacturing”
3 → 20 → 23 → 26 → 30 → 31 → 35 → 37 → 38 → 39 → 40

### Path F — “I need a manufacturing data/digital thread architecture”
A8 → 8 → 20 → 24 → 31 → 35 → 47 → 48 → 49 → 50 → 51 → 52

### Path G — “Founder executive crash course”
A1 → A2 → A4 → 1 → 3 → 4 → 11 → 20 → 23 → 26 → 29 → 30 → 37 → 41 → 42 → 47 → 53

Goal:
Understand the major decisions, risks and maturity transitions without learning every specialist technique first.

## 5. Navigation metadata required in every episode pack

Every episode research pack must include:

- Season ID and title
- Canonical Episode ID
- Primary listener path(s)
- Primary audience A/B/both
- Lifecycle stage DEV/LVP/SVP/cross-stage
- Entry-point status:
  - INDEPENDENT
  - RECAP REQUIRED
  - PREREQUISITE REQUIRED
- Required prior concepts, not merely prior episode numbers
- Suggested prior episode(s)
- Suggested next episode(s)
- “Skip to this episode if…” note
- “Go back first if…” note
- 2–5 minute recap package if RECAP REQUIRED

## 6. Recap architecture

A listener entering mid-series should not be punished for not hearing every prior episode.

Maintain reusable micro-recaps for:

1. Hardware Evolution Ladder
2. DEV / LVP / SVP
3. Claim → Evidence → Applicability
4. Configuration / Effectivity
5. CTQ → Control → Measurement
6. Takt / Constraint / Accepted Throughput
7. Supplier Evidence Envelope
8. Digital Thread / Genealogy

Episode packs should reference a recap object rather than rewrite inconsistent explanations.

## 7. Season trailer contract

Each season should receive a short trailer/intro of approximately 3–7 minutes containing:

- Who this season is for
- What problem it solves
- Where it sits in the hardware lifecycle
- What the listener should already know
- Which framework(s) will recur
- What the listener should be able to decide/do by the end
- Alternative entry path for experienced listeners

A trailer is navigation/editorial content, not a new technical episode and does not alter the canonical 68-episode count.

## 8. Public catalog rule

Do not present the public catalog as:

“Episode 1 of 68, Episode 2 of 68…”

Prefer:

Season → episode title → stage tags → role/problem tags.

Canonical episode numbers remain visible for cross-reference, but should not create the impression that every listener must consume all preceding material.

Example display concept:

Season 5 — Pilot, Ramp and Stable Output
Episode 29 — Capacity, Bottlenecks, Takt Time and Line Balance
Tags: [LVP] [SVP] [NPI] [Operations] [Can start here]

## 9. Content duplication rule

Navigation may repeat a recap but must not duplicate technical ownership.

If Season 8 needs capability/yield logic from Season 6:
- reference the canonical quality framework;
- provide a short recap;
- do not create a new conflicting definition.

## 10. Relationship to Episode Packaging Contract

This document extends `podcast/EPISODE_PACKAGING_CONTRACT.md`.

The Episode Packaging Contract controls technical/evidence readiness.
This document controls listener navigation and discoverability.

An episode is not publication-ready until both are satisfied.

## 11. Pilot Batch mapping

The first five research packs should test the navigation architecture as well as technical packaging:

- A1 — Season 1 / independent founder entry
- A4 — Season 1 / DEV process-choice entry
- Episode 1 — Season 1 / working-prototype independent entry
- Episode 23 — Season 4 / standards/quality-heavy mid-series entry with recap
- Episode 29 — Season 5 / quantitative practitioner mid-series entry with recap

Pilot success criteria:
1. A listener can understand why the episode is relevant before listening.
2. Mid-series entry does not require listening to dozens of prior episodes.
3. Reusable recap objects are sufficient.
4. Audience and lifecycle advice remains explicit.
5. No technical truth is duplicated or contradicted across navigation paths.

## 12. Status

Season/navigation architecture: DEFINED.

Recommended next action:
Open Pilot Batch 1 and build the five Episode Research Packs under this navigation model and the canonical Episode Packaging Contract.
