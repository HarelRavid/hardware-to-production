# Podcast Season Architecture

status: CANONICAL EDITORIAL LAYER
version: 1.0
aligned_with: PODCAST_MAP.md v2.0

## Purpose
Convert the 68-episode canonical learning journey into approachable, independently marketable seasons without breaking episode IDs, evidence mappings or the Hardware Evolution Ladder.

The canonical episode IDs remain unchanged. Seasons are a listener-facing navigation layer.

## Season design rules
1. Each season must answer a coherent listener problem and have a clear entry point.
2. A listener should be able to begin a season without listening to all prior seasons.
3. Each season opens with a short trailer/orientation episode (target ~5 minutes) that explains the relevant Hardware Evolution Ladder position and only the anchor frameworks needed for that season.
4. Trailer/orientation episodes are editorial assets, not new canonical engineering episodes unless later promoted deliberately.
5. DEV/LVP/SVP remains the recurring lens.
6. Cross-season concepts link back to the same Knowledge Objects and evidence; do not duplicate engineering truth.

## Proposed listener-facing seasons

### Season 1 — Build the Right Hardware Before Production Finds Your Mistakes
Primary audience: founders and early hardware development teams.
Canonical content: Opening A1–A8 + Episodes 1–10.
Journey: Idea -> Requirements -> Architecture -> POC -> Engineering Prototype -> Production Intent.
Promise: understand what disciplines, decisions, verification and configuration discipline are needed before scaling builds.

### Season 2 — How Hardware Is Actually Made
Primary audience: designers, founders, NPI/manufacturing engineers choosing production routes.
Canonical content: Episodes 11–19.
Journey: Production Intent -> process-chain selection.
Promise: choose processes by material, geometry, tolerance, volume, tooling, capability and cost per good part rather than process fashion.

### Season 3 — Build the Factory Before You Need the Factory
Primary audience: teams moving into tens/hundreds and first repeatable production.
Canonical content: Episodes 20–31.
Journey: LVP -> production validation -> ramp.
Promise: convert product definition into MBOM/routing, tooling, standard work, quality gates, pilot builds, capacity and controlled engineering change.

### Season 4 — Quality, Suppliers and the Reality of Scale
Primary audience: teams whose product/process now depends on repeatability across people and organizations.
Canonical content: Episodes 32–40.
Journey: stable production -> externalized/scaled production system.
Promise: capability, nonconformance, reliability, traceability, standards, supplier qualification and resilience.

### Season 5 — Automation, Data and the Connected Factory
Primary audience: teams deciding when/how to automate and connect production.
Canonical content: Episodes 41–52, including OT/ICS cybersecurity coverage integrated into the Data Hub/security arc.
Journey: scalable production -> automated/connected production.
Promise: automate only where economics and process maturity justify it; connect data without creating competing truth or unsafe IT/OT pathways.

### Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
Primary audience: cross-functional technical leaders and teams applying the full system.
Canonical content: Episodes 53–60.
Journey: integrated manufacturing operating system.
Promise: use recurring decision frameworks, cases, tradeoffs and evidence to make better hardware-to-production decisions.

## Season trailer template
Each trailer should answer:
- Where are you on the Hardware Evolution Ladder?
- What problem does this season solve?
- Which DEV/LVP/SVP context matters most?
- Which 2–4 anchor frameworks will recur?
- What can you skip if it does not apply to your product?
- What should you have by the end of the season?

## Entry-point rule
Marketing pages/show notes should offer at least these entry choices:
- I have an idea / early prototype -> Season 1
- I need to choose how to manufacture parts -> Season 2
- I need to build tens/hundreds repeatedly -> Season 3
- I need stable quality/suppliers/compliance -> Season 4
- I am considering automation/data integration -> Season 5
- I want decision frameworks/case studies -> Season 6

## Integrity rule
Season boundaries optimize listener navigation. They must never change standards applicability, evidence maturity, claim meaning or canonical episode-to-WBS mapping.