---
id: H2P-PW-016
title: Prototype Configuration Control
object_type: Process
domain: Prototype Workshop
subdomain: Strategy & Workshop Architecture
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, PVT]
status: Researching
summary: Lightweight but explicit control of the hardware, software, drawings, BOM, process instructions and test configuration associated with each prototype build.
tags: [configuration-management, revision-control, prototype]
---
# Prototype Configuration Control
## Definition
Prototype Configuration Control is the discipline of identifying which design and process configuration applies to a physical prototype and controlling changes well enough that test results can be tied to the exact item tested.
## Why It Matters
Without configuration control, teams can no longer answer a basic engineering question: **which version produced this result?** That destroys traceability and makes comparisons across builds unreliable.
## Minimum Viable Control for Prototypes
- unique build/unit identifier
- controlled drawing/CAD revision
- BOM revision
- firmware/software revision where relevant
- recorded deviations and substitutions
- test procedure revision
- date and responsible engineer
## Standards / Guidance
ISO 10007:2017 describes configuration management from concept through disposal and includes configuration planning, identification, change control, status accounting and configuration audit. NASA treats configuration management and technical data management as complementary lifecycle processes.
## Common Mistakes
- assuming configuration management starts only at production release
- relying on file names such as final_v7_new
- changing a prototype during debug without logging the change
- failing to record temporary component substitutions
- recording test results without configuration metadata
## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| REQUIRED_BY | H2P-PW-006 | Strong | High | a build plan needs an identifiable configuration | ISO 10007 / NASA |
| ENABLES | H2P-PW-017 | Mandatory | High | build record depends on configuration identity | systems engineering practice |
| ENABLES | H2P-PW-018 | Mandatory | High | traceability requires configuration identity | configuration management principles |
| SUPPORTS | H2P-PW-159 | Strong | High | prototype revision control is an implementation mechanism | project architecture |
| PRECEDES | H2P-PW-164 | Strong | High | disciplined prototype configuration reduces design-transfer ambiguity | project methodology |
## Sources
- ISO 10007:2017: https://www.iso.org/standard/70400.html
- NASA Technical Data Management: https://www.nasa.gov/reference/6-6-technical-data-management/
