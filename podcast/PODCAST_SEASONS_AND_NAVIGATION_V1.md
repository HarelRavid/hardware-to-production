# Podcast Seasons & Listener Navigation V1

status: POST-FREEZE EDITORIAL ARCHITECTURE
version: 1.0
backbone_change: NO — editorial/navigation layer over frozen Knowledge Backbone V1

## 1. Purpose

The canonical roadmap contains 68 episodes (A1–A8 + 1–60), but listeners should not experience the product as one compulsory 68-episode sequence.

This document defines a listener-facing season and navigation architecture that:
- reduces entry friction;
- allows different hardware roles and maturity stages to enter at useful points;
- preserves the DEV → LVP → SVP learning journey;
- avoids duplicating technical truth;
- supports both primary audiences;
- keeps the frozen Knowledge Backbone and canonical episode IDs intact.

Principle:

> One knowledge backbone; multiple useful paths through it.

## 2. Two navigation dimensions

Every episode will be navigable in two independent ways.

### Dimension A — Season / subject journey
A listener can follow a coherent season from beginning to end.

### Dimension B — Role / maturity path
A listener can select a path such as:
- Founder / early hardware team;
- Prototype → first production team;
- NPI / manufacturing engineer;
- Quality / reliability;
- Supply chain / supplier quality;
- Automation / operations;
- Manufacturing data / OT.

Episodes remain canonical objects. A path points to episodes; it does not create duplicate episode versions.

## 3. Proposed season architecture

Exact final episode-to-season assignment will be validated during Episode Research Pack planning. The season boundaries below are editorial containers, not new technical domains.

### Season 1 — Build the Right Hardware Before You Scale It
Primary audience: founders, developers, early multidisciplinary hardware teams.
Primary maturity: Idea → DEV → serious integrated prototype.

Anchor content:
- A1 requirements;
- A2 team/ownership;
- A3 architecture/interfaces;
- A4 prototype technologies;
- A5 mechanical prototype design;
- A6 electronics/PCB/embedded hardware;
- A7 development verification;
- A8 configuration from prototype #1;
- early production-readiness concepts from the opening of Episodes 1–60 where required.

Season promise:
Understand what disciplines and decisions are required to build a prototype that teaches you something useful without silently creating manufacturing debt.

Independent entry point: YES.

### Season 2 — Prototype to Production-Intent Hardware
Primary audience: founders/engineering teams with a working prototype; early NPI/industrialization teams.
Primary maturity: DEV → production-intent → early LVP.

Core themes:
- why a working product is not production ready;
- DFX / manufacturability / assembly / testability;
- materials/process selection;
- tolerance/GD&T/metrology foundations;
- production-intent components;
- BOM/configuration maturity;
- engineering change/effectivity;
- test strategy transition from engineering verification to production acceptance.

Season promise:
Turn “it works” into a controlled design that can be built repeatedly by people other than the inventors.

Independent entry point: YES, with a short DEV recap.

### Season 3 — Build the First Real Production System
Primary audience: teams entering tens/hundreds of units.
Primary maturity: LVP.

Core themes:
- process definition;
- work instructions/routing;
- fixtures/tooling;
- manual vs assisted vs semi-automatic production;
- quality chain: CTQ → PFMEA → Control Plan → MSA → SPC/capability;
- NCR/rework;
- traceability/genealogy;
- pilot/PVT/run-at-rate;
- bottlenecks/WIP/accepted throughput;
- first production release.

Season promise:
Build tens or hundreds of units without depending on tribal knowledge or hiding failures behind rework.

Independent entry point: YES for a team with a first prototype.

### Season 4 — Suppliers, Cost and Industrialization
Primary audience: NPI, operations, supply chain, engineering managers and founders approaching scale.
Primary maturity: LVP → SVP preparation.

Core themes:
- prototype supplier vs production supplier;
- supplier qualification;
- FAI / PPAP applicability;
- sub-tier risk;
- supplier change/requalification;
- NRE / CapEx / unit economics;
- break-even / NPV / uncertainty;
- staged CapEx;
- industrialization suppliers/tooling/equipment suppliers;
- make/buy and scaling decisions.

Season promise:
Understand the supplier and economic system behind the product before volume exposes weak assumptions.

Independent entry point: YES, with configuration/quality prerequisites recapped.

### Season 5 — Automation, Capacity and Ramp
Primary audience: manufacturing/process/automation engineers, operations leaders, scaling founders.
Primary maturity: mature LVP → Ramp → SVP.

Core themes:
- Automation Ladder;
- AUTOMATE 10;
- machine vs system capacity;
- OEE and loss decomposition;
- failure/recovery engineering;
- safety applicability;
- automation qualification/release;
- moving constraints;
- sustainable rate;
- ramp exit evidence.

Season promise:
Automate and increase rate only after understanding the real constraint, failure mechanism and evidence required for controlled production.

Independent entry point: CONDITIONAL — recap of quality/configuration/capacity concepts required.

### Season 6 — The Digital Factory: Manufacturing Truth, Data and OT Security
Primary audience: manufacturing systems, automation, quality, operations and technical leadership.
Primary maturity: LVP → SVP.

Core themes:
- Minimum Viable Manufacturing Atlas;
- definition vs execution vs evidence;
- serial/lot genealogy;
- MES/ERP/PLM/QMS boundaries;
- ISA-95 / IEC 62264 concepts;
- OPC UA semantic integration;
- manufacturing claims/evidence/applicability;
- OT/ICS zones and conduits;
- remote access;
- configuration integrity;
- backup vs recovery;
- cyber → quality/evidence impact.

Season promise:
Create manufacturing truth that can be reconstructed, protected and trusted without buying an enterprise software stack before it is justified.

Independent entry point: YES for experienced manufacturing listeners; foundation recap required for early teams.

### Season 7 — Proving Commercial Production and Learning from the Field
Primary audience: cross-functional leadership, quality/reliability, NPI, operations.
Primary maturity: Ramp → SVP → field lifecycle.

Core themes:
- production validation;
- release evidence;
- reliability and field evidence;
- complaints/returns/field events;
- signal aggregation;
- CAPA/effectiveness evidence;
- minimum controlled production mode;
- recalls/containment;
- cross-industry case studies;
- corrective learning and requalification;
- what “commercially ready” actually means.

Season promise:
Close the loop between production release and field reality, and learn how mature systems respond when evidence changes.

Independent entry point: CONDITIONAL — short backbone recap required.

## 4. Listener paths

### Path A — “I have an idea / I am building my first hardware product”
Recommended:
Season 1 → Season 2 → selected Season 3 episodes → Season 4 economics/suppliers → later seasons as scale approaches.

Goal:
See future manufacturing obligations early enough to avoid expensive architectural debt.

### Path B — “Our prototype works; now we need to build 20–500 units”
Recommended entry:
Season 2 recap → Season 3 in full → relevant Season 4 → Season 5.

Goal:
Move from inventor-dependent builds to controlled LVP.

### Path C — “I run NPI / manufacturing / industrialization”
Recommended entry:
Season 3 → Season 4 → Season 5 → Season 6 → Season 7.

Use Season 1–2 as targeted references when design/development interfaces are the constraint.

### Path D — “I work in quality / reliability”
Recommended:
Season 2 production-intent/configuration episodes → Season 3 quality chain → supplier-quality content in Season 4 → release/recovery in Seasons 5–7.

### Path E — “I work in automation / manufacturing systems”
Recommended:
Season 3 process/quality foundations → Season 5 → Season 6 → relevant Season 7 recovery/case studies.

### Path F — “I am a founder/manager and need the executive path”
A curated short path will be produced during episode packaging using selected episodes from all seven seasons.
It must preserve the major decision gates without pretending to replace technical episodes.

## 5. Episode navigation metadata

Every Episode Research Pack must add these listener-facing fields in addition to the Episode Packaging Contract:

- Season
- Primary listener path(s)
- Good first episode? YES / WITH RECAP / NO
- Required prior concepts
- 2–5 minute prerequisite recap required? YES/NO
- DEV relevance
- LVP relevance
- SVP relevance
- Related episodes: BEFORE / NEXT / DEEP DIVE / ALTERNATE PATH
- Listener role tags
- Search/topic tags

## 6. Recap rule

A listener should not need to consume dozens of earlier episodes merely to understand one specialized topic.

When an episode depends on a canonical concept from another season:
1. give a concise recap;
2. use the same canonical terminology/framework;
3. point to the deeper episode;
4. do not duplicate the full technical treatment.

Target recap length: enough to restore the prerequisite mental model, typically 2–5 minutes, not a second episode hidden inside the episode.

## 7. Season trailer / orientation rule

Each season should begin with a short orientation asset explaining:
- who the season is for;
- where the listener is on DEV/LVP/SVP;
- what they should already know;
- what decisions they will be able to make by the end;
- which earlier episodes are optional prerequisites;
- where to enter if they already have experience.

This can be a short trailer/orientation episode rather than part of the canonical 68 technical episode count.

## 8. Navigation UX principle

The published index should allow at least four ways to find content:

1. **By season** — coherent learning journey.
2. **By maturity** — DEV / LVP / SVP.
3. **By role** — founder, mechanical, electronics, NPI, quality, supplier, automation, manufacturing data/OT.
4. **By problem** — e.g. “prototype works but cannot scale”, “supplier change”, “high scrap”, “automation decision”, “traceability”, “cyber recovery”.

The same episode may appear in several indexes without being duplicated.

## 9. Anti-patterns

Do not:
- publish a flat 68-item list as the primary navigation experience;
- force a specialist to start at A1;
- duplicate technical truth into multiple role-specific versions;
- rename canonical frameworks differently by season;
- imply that season order equals a universal product-development waterfall;
- hide prerequisite assumptions;
- make every episode depend on every earlier episode.

## 10. Relationship to Knowledge Backbone V1 Freeze

This document does not reopen the frozen backbone.

It changes the listener-facing organization and navigation only.
Canonical episode IDs, technical truth, P2 packages, global invariants, claim/evidence/applicability model and DEV/LVP/SVP definitions remain unchanged.

If episode packaging later reveals that a season requires genuinely missing technical knowledge, that becomes a controlled backbone gap request rather than an editorial workaround.

## 11. Pilot Batch implication

The first Episode Research Pack pilot should intentionally sample different seasons and listener paths.

Recommended five-pack:
- A1 — Season 1 / founder entry point;
- A4 — Season 1 / prototype-technology decision;
- Episode 1 — Season 2 / prototype-to-production bridge;
- Episode 23 — likely Season 3 / quality/process evidence stress test, subject to canonical title verification;
- Episode 29 — likely quantitative/industrialization stress test, subject to canonical title verification.

Before opening Episode 23 and 29 packs, verify their exact canonical titles and final season assignment from PODCAST_MAP.md rather than relying on remembered numbering.

## 12. Success criterion

A listener should be able to answer:

> “Where am I in the hardware journey, which path is relevant to my job/problem, what should I listen to next, and what can I safely skip for now?”

If the published navigation cannot answer those questions, the season architecture has failed even if all 68 episodes are technically excellent.
