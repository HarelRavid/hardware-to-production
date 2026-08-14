# Hardware-to-Production Podcast — Season & Listener Navigation Architecture

status: CANONICAL EDITORIAL NAVIGATION
version: 1.0
baseline: Knowledge Backbone V1
purpose: Divide the 68-episode roadmap into listener-friendly seasons and entry paths without changing the frozen technical backbone.

## 1. Principle

The podcast must not be presented as one undifferentiated list of 68 episodes.

The technical backbone remains continuous from DEV → LVP → SVP, but the listener-facing product is divided into seasons that:
- have a clear promise;
- serve a recognizable audience/stage;
- can be entered independently with a short prerequisite recap;
- make it easy to navigate by problem rather than chronology;
- preserve cross-links to the canonical episode numbering.

Season architecture is editorial packaging, not a new technical ontology.

## 2. Listener entry paths

### Path A — I am starting a hardware company/product
Start: Opening A1.
Goal: understand the disciplines, architecture and prototype decisions that determine future manufacturability.
Primary seasons: S1 → S2 → S3.

### Path B — I have a working prototype and need to manufacture 10–500 units
Start: Episode 1 or Episode 3.
Goal: convert prototype truth into controlled LVP production without over-automating or locking in manufacturing debt.
Primary seasons: S2 → S4 → S5 → S6.

### Path C — I am an NPI / manufacturing / quality engineer
Start: Episode 20, with a compact recap of Episodes 1–10.
Goal: production system, quality, pilot/ramp, supplier and scale.
Primary seasons: S4 → S5 → S6 → S7.

### Path D — I need one technical topic
Use topic navigation:
- DFM / DFA / DFT → S2
- manufacturing processes → S3
- MBOM / tooling / WI → S4
- pilot / yield / capacity → S5
- quality / reliability / compliance → S6
- suppliers → S7
- automation → S8
- manufacturing data / OT security / scale intelligence → S9
- real-world case studies / synthesis → S10

Every season opener must state whether prior seasons are required or merely recommended.

## 3. Season structure

### Season 1 — Build Hardware That Can Grow Up
Audience: founders / early development teams
Lifecycle: Idea → DEV / first serious prototypes
Canonical episodes:
- A1 From an Idea to Engineering Requirements
- A2 The Hardware Team Map
- A3 System Architecture and Interfaces
- A4 Choosing Prototype Technologies Without Trapping the Product
- A5 Mechanical Design for the First Serious Prototype
- A6 Electronics, PCB and Embedded Hardware for the First Serious Prototype
- A7 Development Verification Before Production Verification
- A8 Configuration Management from Prototype #1

Promise:
> Build the first serious version of the product without creating avoidable manufacturing debt.

Exit state:
Listener understands what a serious DEV system must preserve before industrialization starts.

### Season 2 — From Working Prototype to Production-Intent Product
Audience: founders + NPI + engineering teams
Lifecycle: late DEV → production intent
Canonical episodes:
- 1 The product works. Why can’t we manufacture it?
- 2 POC, Prototype, MVP and Production-Intent Hardware
- 3 What NPI and Industrialization Actually Own
- 4 Product Readiness vs Manufacturing Readiness
- 5 EVT, DVT, PVT, Pilot and Ramp Without the Buzzwords
- 6 DFM
- 7 DFA / mistake prevention
- 8 DFT / calibration / traceability
- 9 Tolerance / GD&T / variation
- 10 Reliability / service / repair

Promise:
> Learn what must change when “it works” has to become “we can build it repeatedly.”

### Season 3 — Manufacturing Process Decisions
Audience: product engineers + manufacturing engineers + founders making make/process decisions
Lifecycle: DEV → LVP → SVP process migration
Canonical episodes:
- 11 Process selection
- 12 Polymer parts
- 13 Metal parts
- 14 Joining
- 15 Composites
- 16 Ceramics / powder / sintering
- 17 Additive manufacturing
- 18 Surface engineering / cleaning / heat treatment
- 19 Manufacturing process chains

Promise:
> Choose how the product should actually be made, and know when the prototype route must expire.

Mandatory navigation rule:
Every process episode includes Prototype Route / LVP Route / SVP Route / Trigger to Change.

### Season 4 — Build the Minimum Viable Production System
Audience: teams entering tens/hundreds of units
Lifecycle: production-intent → LVP
Canonical episodes:
- 20 EBOM → MBOM / process flow
- 21 Tooling / fixtures / production-intent equipment
- 22 Work instructions / standard work / operator qualification
- 23 DFMEA / PFMEA / Control Plan / quality gates
- 24 Production testing / MSA
- 25 Layout / material flow / ergonomics

Promise:
> Build a controlled production system for tens or hundreds without pretending you already run a mature factory.

This season is a major standalone entry point for Audience B.

### Season 5 — Pilot, Yield, Capacity and Ramp
Audience: NPI / manufacturing / operations / quality
Lifecycle: LVP → production validation → ramp
Canonical episodes:
- 26 Pilot build planning
- 27 Production validation build
- 28 Yield / rework / scrap / learning curve
- 29 Capacity / bottlenecks / takt / balance
- 30 Supplier readiness / CM management
- 31 Engineering changes during ramp

Promise:
> Prove that the production system works under representative conditions before scaling the commitment.

### Season 6 — Quality, Reliability and Evidence
Audience: quality / reliability / manufacturing / engineering leadership
Lifecycle: cross-stage, strongest at LVP/SVP
Canonical episodes:
- 32 Process capability / SPC
- 33 Nonconformance / MRB / CAPA
- 34 Reliability validation and production reality
- 35 Traceability / genealogy / evidence retention
- 36 Standards / regulatory requirements / applicability

Promise:
> Know whether the product and process are actually under control—and what evidence supports that claim.

Required cross-link:
FIELD EVIDENCE LOOP must be visible here, especially Episodes 33–35.

### Season 7 — Supplier Industrialization and Supply Chain
Audience: supply chain / NPI / quality / founders outsourcing production
Lifecycle: production-intent → LVP → SVP
Canonical episodes:
- 37 Make or Buy?
- 38 Selecting a supplier by capability
- 39 RFQ technical package / first production approval
- 40 Supplier quality / dual sourcing / resilience

Promise:
> Turn “a supplier can make a sample” into “a supplier can support controlled production.”

Required cross-link:
Industrialization Supplier concept includes tooling/equipment/test-system suppliers where relevant.

### Season 8 — Automation and Scaling Decisions
Audience: manufacturing / automation / operations / founders considering CapEx
Lifecycle: LVP → SVP
Canonical episode range:
- 41–46, using the canonical Podcast Map titles and mappings

Core promise:
> Automate the right problem at the right maturity, then prove the integrated system can run safely and recoverably.

Mandatory frameworks:
AUTOMATE 10, LOSS 8, RELEASE 12, OEE guardrails, economics link.

### Season 9 — Manufacturing Data, Digital Thread and OT Security
Audience: manufacturing systems / operations / engineering leadership / smart-factory teams
Lifecycle: LVP → SVP and scale
Canonical episode range:
- 47–52, using canonical Podcast Map titles and mappings

Core promise:
> Preserve manufacturing truth as the factory becomes connected, data-rich and cyber-dependent.

Mandatory concepts:
Manufacturing Atlas, Definition vs Execution, genealogy, evidence/applicability, minimum controlled production mode, OT zones/conduits, recovery.

### Season 10 — What Real Manufacturing Failures Teach Us
Audience: all audiences; best after at least one earlier season
Lifecycle: cross-stage synthesis
Canonical episodes:
- 53–60

Core promise:
> Stress-test the frameworks against documented real-world failures, ramps, recalls and recoveries.

Case-study packaging rule:
FACT → SOURCE INTERPRETATION → OUR FRAMEWORK LESSON.

This season may grow editorially with additional cases without changing the frozen backbone.

## 4. Season opener contract

Each season gets a short 3–7 minute opener/trailer or opening segment containing:
1. Who this season is for.
2. Where the listener is in DEV/LVP/SVP.
3. What they should already know.
4. What they will be able to decide/do by the end.
5. The 2–4 canonical frameworks used repeatedly.
6. Where to start instead if this is not their current problem.

This avoids requiring sequential listening of the entire catalogue.

## 5. Episode navigation metadata

Every Episode Research Pack must add:
- Season ID
- Primary entry path(s): A/B/C/D
- Can-start-here: YES / WITH RECAP / NO
- Required prerequisites
- Recommended prior episodes
- Next logical episodes
- Topic tags
- DEV / LVP / SVP relevance score: Primary / Secondary / Context

## 6. Topic-tag taxonomy

Use stable listener-facing tags, not repository jargon:
- Requirements
- Systems Architecture
- Mechanical
- Electronics / PCB
- Embedded / Firmware
- Verification / Test
- DFM / DFA / DFT
- Process Selection
- Tooling / Fixtures
- Assembly
- Quality
- Metrology
- Reliability
- Pilot / Ramp
- Capacity / Flow
- Economics
- Supplier / Supply Chain
- Automation
- Safety
- Standards / Compliance
- Traceability / Digital Thread
- MES / Manufacturing Data
- OT Cybersecurity
- Field / CAPA / Recall
- Leadership / Decision Making

## 7. Navigation UX rule

Do not expose the listener primarily to internal IDs such as P2.04 or WBS numbers.

Listener-facing hierarchy:
Season → Episode → Problem / Stage → Related episodes.

Research-facing metadata retains:
Episode → P2 → WBS → Claims → Evidence.

This preserves technical traceability without making the podcast feel like a standards database.

## 8. Pilot Batch placement

The first five Episode Research Packs are deliberately distributed across the navigation architecture:

| Pilot | Season | Why selected |
|---|---|---|
| A1 — From an Idea to Engineering Requirements | S1 | tests founder/DEV entry point |
| A4 — Choosing Prototype Technologies Without Trapping the Product | S1/S3 bridge | tests prototype-shortcut expiration and process migration |
| 1 — The product works. Why can’t we manufacture it? | S2 | tests main industrialization entry point |
| 23 — DFMEA/PFMEA/Control Plan/Quality Gates | S4/S6 bridge | tests standards-heavy quality packaging |
| 29 — Capacity/Bottlenecks/Takt/Line Balance | S5 | tests quantitative worked-evidence packaging |

If these five pass the Episode Packaging Contract, they become reference templates for the rest of the catalogue.

## 9. Freeze compatibility

This architecture does not reopen Knowledge Backbone V1.
It changes listener-facing organization only.

A season move or title change is editorial refinement unless it changes:
- technical claim ownership;
- canonical framework meaning;
- audience mission;
- DEV/LVP/SVP lifecycle logic;
- backbone/global invariants.

## 10. Result

The podcast should be marketed and navigated as a set of focused learning journeys, not as “68 episodes you must finish.”

Canonical listener proposition:

> Start where your hardware team is today, understand what you need now, and see what production will demand next.
