---
id: H2P-PW-018
title: Prototype Traceability
object_type: Concept
domain: Prototype Workshop
subdomain: Strategy & Workshop Architecture
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, PVT]
status: Researching
summary: The ability to trace a prototype unit and its test results back to its design baseline, components, build history, changes and evidence.
tags: [traceability, configuration, test-data, prototype]
---
# Prototype Traceability
## Definition
Prototype Traceability is the ability to answer, for a physical prototype or test result: what configuration was used, which parts and process steps produced it, what changed, and where the supporting data is stored.
## Why It Matters
Prototype programs generate high variation by design. Traceability converts that variation from noise into usable evidence by preserving cause-and-effect context.
## Minimum Traceability Chain
Requirement or learning objective → build plan → design/BOM revision → unit/build ID → as-built deviations → test procedure → test data/result → engineering conclusion → resulting change.
## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| DEPENDS_ON | H2P-PW-016 | Mandatory | High | traceability requires identified configuration | ISO 10007 |
| DEPENDS_ON | H2P-PW-017 | Mandatory | High | as-built record is the physical-unit history | NASA technical data principles |
| ENABLES | H2P-PW-162 | Strong | High | lessons need reliable links to the actual build and evidence | NASA lessons learned |
| SUPPORTS | H2P-PW-164 | Strong | High | mature traceability reduces ambiguity in transfer to production | project methodology |
## Sources
- NASA Technical Data Management: https://www.nasa.gov/reference/6-6-technical-data-management/
- NASA Lessons Learned: https://www.nasa.gov/nasa-lessons-learned/
