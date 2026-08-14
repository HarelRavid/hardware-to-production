# Podcast Season & Listener Navigation Architecture

status: POST-FREEZE EDITORIAL BASELINE
version: 1.0
backbone_impact: NONE — editorial/navigation layer only
canonical_episode_source: PODCAST_MAP.md

## 1. Purpose

The canonical roadmap contains 68 episodes, but listeners should never experience the show as one mandatory 68-step sequence.

This document defines the listener-facing navigation layer: seasons, entry points, audience routes, lifecycle routes and recap rules. It does not renumber or change the technical truth of the frozen Knowledge Backbone.

Core principle:

> One knowledge backbone; multiple listener paths.

The show must allow a founder in early DEV, an NPI engineer entering LVP, and a production team preparing for SVP to enter at useful points without listening to dozens of unrelated episodes first.

## 2. Navigation model

Every episode keeps its canonical ID from PODCAST_MAP.md but receives listener-facing metadata:

- Season
- Primary audience
- Secondary audience
- Lifecycle stage: DEV / LVP / SVP / cross-stage
- Topic track(s)
- Entry-point suitability
- Prerequisite episodes
- Five-minute-or-less prerequisite recap requirements
- Recommended next episode(s)
- Related deep dives

No technical episode may depend on hidden prerequisite knowledge. If a prerequisite is important but the listener may reasonably enter mid-series, the episode must include a concise recap or point to an optional primer.

## 3. Listener-facing seasons

Exact episode allocation will be completed from the canonical 68-episode map during episode packaging. The season boundaries below are editorial containers, not new technical domains.

### Season 1 — Build the Right Thing
**Audience:** founders, early hardware developers, first technical hires.
**Lifecycle:** Idea → Requirements → Architecture → serious prototype.

Primary content:
- Opening Arc A1–A8;
- requirements and ownership;
- architecture/interfaces;
- prototype technology choices;
- first serious mechanical/electronics design;
- development verification;
- configuration discipline from prototype #1.

Promise to listener:
> Understand what disciplines and decisions your hardware project needs before prototype shortcuts become production debt.

Primary entry point: A1.
Alternative entry: A4 for teams already prototyping.

### Season 2 — Turn the Prototype into a Product
**Audience:** founders with a working prototype, product/NPI/industrialization teams.
**Lifecycle:** Integrated/engineering prototype → production-intent hardware.

Primary content:
- DFX;
- material/component industrialization;
- tolerances/GD&T/metrology;
- joining/assembly/testability/serviceability;
- configuration/change control;
- reliability and validation transition;
- production-intent design decisions.

Promise:
> Learn what must change when “it works” is no longer enough.

Primary entry point: canonical Episode 1.

### Season 3 — Build the Production System
**Audience:** manufacturing/process/NPI engineers and technical founders building LVP.
**Lifecycle:** Production-intent → tens/hundreds of units.

Primary content:
- manufacturing process selection;
- tooling/fixtures/work instructions;
- assembly architecture;
- process definition;
- pilot builds/PVT;
- capacity/takt/bottlenecks/WIP;
- manual vs assisted vs semi-automatic production.

Promise:
> Build a repeatable low-volume production system without prematurely buying a mass-production factory.

Primary entry point: production/process-selection episode or NPI entry point defined in episode metadata.

### Season 4 — Prove Quality, Reliability & Compliance
**Audience:** quality, reliability, test, NPI and engineering leadership.
**Lifecycle:** LVP → production validation.

Primary content:
- CTQs;
- PFMEA;
- Control Plan;
- MSA;
- SPC/capability;
- inspection/sampling;
- validation/qualification;
- reliability evidence;
- standards/applicability/compliance logic;
- reaction/CAPA/effectiveness evidence.

Promise:
> Replace “we tested it and it passed” with evidence that the product and process can be trusted.

Independent entry allowed with a short DEV/LVP/SVP recap.

### Season 5 — Suppliers, Cost & Scale
**Audience:** founders, operations, supply chain, manufacturing leadership.
**Lifecycle:** LVP → ramp.

Primary content:
- supplier industrialization;
- FAI/PPAP applicability;
- sub-tier control;
- supplier change/requalification;
- manufacturing economics;
- NRE/CapEx/unit economics;
- break-even/NPV;
- staged investment;
- ramp and moving constraints.

Promise:
> Learn how supply chain and economics change the technically possible into the commercially manufacturable.

### Season 6 — Automation & the Digital Factory
**Audience:** manufacturing/automation/data engineers and teams scaling beyond manual control.
**Lifecycle:** LVP → ramp → SVP.

Primary content:
- automation ladder;
- qualification/release;
- OEE/loss decomposition;
- fault/recovery;
- Manufacturing Atlas/digital thread;
- genealogy/effectivity;
- MES/PLM/ERP/QMS boundaries;
- ISA-95/IEC 62264 and OPC UA applicability;
- OT/ICS cybersecurity and IEC 62443;
- remote access, backup/recovery and controlled production modes.

Promise:
> Automate and digitize only after you know what truth, controls and recovery behavior the factory must preserve.

### Season 7 — Ramp, Field Reality & Continuous Learning
**Audience:** teams operating commercial hardware production.
**Lifecycle:** Ramp → SVP → field feedback/lifecycle.

Primary content:
- production release/ramp exit;
- field evidence loop;
- complaints/returns;
- signal aggregation;
- CAPA effectiveness;
- recalls/containment where relevant;
- change/requalification;
- cross-industry case studies;
- continuous learning back into requirements/design/process/supplier controls.

Promise:
> Production release is not the end of engineering; field evidence closes the loop.

## 4. Listener routes

Seasons are the browse structure. Routes are the fast navigation structure.

### Route A — “I have an idea / early prototype”
A1 → A3 → A4 → A5/A6 → A7 → A8 → Season 2.

Goal: prevent manufacturing debt without forcing a founder to learn factory operations prematurely.

### Route B — “My prototype works; now I need 50–500 units”
Episode 1 / Season 2 entry → production-intent design → Season 3 → quality essentials from Season 4 → supplier/cost essentials from Season 5.

Goal: move rapidly into controlled LVP.

### Route C — “I just joined NPI / manufacturing”
NPI entry episode → process/tooling → configuration/change → CTQ/PFMEA/Control Plan → pilot/capacity → supplier → automation as needed.

Goal: provide a practitioner path without requiring the Opening Arc.

### Route D — “We need to scale to commercial production”
LVP readiness recap → quality/capability → supplier/rate → economics → automation → Atlas/traceability → OT security → ramp/field loop.

Goal: focus on evidence needed for SVP.

### Route E — “I need one topic now”
Topic-based entry through Quality, Supplier, Automation, Manufacturing Data, Cybersecurity, Reliability, Economics or Manufacturing Process tracks.

Every deep-dive episode on this route must contain enough recap to stand alone or clearly link one optional primer.

## 5. Topic tracks

Episodes may belong to more than one track:

1. Product & Systems Engineering
2. Mechanical / Materials / Manufacturing Processes
3. Electronics / PCB / Embedded Hardware
4. DFX / Industrialization / NPI
5. Quality / Metrology / Statistics
6. Reliability / Validation / Compliance
7. Suppliers / Supply Chain
8. Manufacturing Economics / Capacity / Ramp
9. Automation / Equipment / OEE
10. Manufacturing Data / Digital Thread
11. OT / ICS Cybersecurity
12. Field Quality / CAPA / Lifecycle Learning

Tracks are navigation metadata, not additional episode numbering.

## 6. Episode card contract

Each published episode should expose a compact listener card:

**You are here:** DEV / LVP / SVP
**Best for:** audience/role
**You should already know:** maximum 1–3 prerequisites
**In this episode:** the decision/problem being solved
**You will leave with:** listener tool/checklist/calculation
**Prototype shortcut:** when relevant
**Shortcut expires when:** explicit condition
**Next:** 1–3 recommended episodes
**Deep dive:** optional related track episodes

This allows listeners to navigate non-linearly without losing lifecycle context.

## 7. Recap rule

A listener should not need to consume an entire earlier season solely to understand one later technical episode.

When an episode depends on a canonical framework:
- provide a 30–120 second recap for one concept;
- up to ~5 minutes for a genuinely necessary multi-concept primer;
- link the full foundation episode as optional deeper context.

Do not duplicate full episodes inside recaps.

## 8. Trailer / season opener rule

Each season receives a short navigation trailer, approximately 3–7 minutes, answering:

1. Who is this season for?
2. Where are we on the Hardware Evolution Ladder?
3. What problem does this season solve?
4. Which prior concepts matter?
5. Which episodes can be entered independently?
6. What evidence/readiness should the listener have by the end?

The trailer is navigation content and does not count as a new canonical technical episode.

## 9. DEV / LVP / SVP navigation tags

Every episode gets at least one maturity tag:

- **DEV-FIRST** — most useful before production intent.
- **LVP-FIRST** — most useful when building tens/hundreds.
- **SVP-FIRST** — most useful during scale/commercial production.
- **CROSS-STAGE** — decisions change across all three stages.

Where relevant the episode card shows all three takeaways rather than forcing a single stage.

## 10. Pilot Batch under this architecture

The first five research packs remain:

- A1 — validates the founder/DEV entry experience;
- A4 — validates prototype-shortcut/expiration logic;
- Episode 1 — validates the prototype-to-product entry point;
- Episode 23 — validates a standards/quality-heavy practitioner episode;
- Episode 29 — validates a quantitative/manufacturing decision episode.

Before these packs are considered successful, they must also prove:
- season placement works;
- episode card is useful;
- prerequisite burden is reasonable;
- recap rule works;
- recommended-next links create useful navigation;
- listener can enter without following the entire 68-episode sequence.

## 11. Navigation success criteria

PASS when:
1. no audience is forced through irrelevant prerequisite seasons;
2. DEV, LVP and SVP each have a clear entry route;
3. topic specialists can enter through a track;
4. canonical episode IDs remain stable;
5. season boundaries do not create duplicate engineering truth;
6. prerequisite recaps prevent hidden knowledge assumptions;
7. episode cards make next-step navigation obvious;
8. the show still communicates one coherent Idea → Field Learning journey.

## 12. Relationship to the frozen backbone

This document is an editorial/navigation layer and therefore does not reopen Knowledge Backbone V1.

If season packaging reveals a missing technical domain, contradictory invariant or missing lifecycle transition, that becomes a controlled backbone gap request under the Freeze Record. Mere episode movement, season renaming, track tagging or recap creation is editorial refinement.

## 13. Next action

Build the five Pilot Episode Research Packs using both:
- `podcast/EPISODE_PACKAGING_CONTRACT.md`; and
- this Season & Listener Navigation Architecture.

The pilot should validate the production system before opening all remaining episode packs.
