---
id: H2P-PW-006
title: Prototype Build Planning
object_type: Process
domain: Prototype Workshop
subdomain: Strategy & Workshop Architecture
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
summary: Structured planning of a prototype build so each build has a defined purpose, configuration, resources, tests, timing and learning objective.
tags: [prototype-build, planning, iteration, test]
---
# Prototype Build Planning
## Definition
Prototype Build Planning is the deliberate preparation of a build before fabrication starts: what will be built, why, which configuration is intended, which parts and resources are required, which tests will be run, and which decisions the build should enable.
## Purpose
Prevent prototype work from becoming ad-hoc fabrication. A build should be treated as an experiment with a defined learning objective.
## Core Inputs
- prototype purpose and required fidelity
- current design/configuration baseline
- BOM and long-lead items
- manufacturing route and workshop/supplier capacity
- test plan, fixtures and instrumentation
- safety constraints
## Core Outputs
- build objective
- build configuration/baseline
- build BOM
- fabrication/assembly route
- resource and schedule plan
- test allocation
- acceptance/learning criteria
- build identifier
## Key Evidence
NASA systems engineering guidance treats technical planning, configuration management, technical data management, verification and validation as linked lifecycle processes. Prototype/test articles therefore need identifiable configuration and planned verification activity, not only fabrication instructions.
## Common Mistakes
- building before deciding what question the prototype must answer
- changing design during the build without recording the change
- allowing different test teams to assume different configurations
- ignoring destructive test sequencing
- ordering long-lead prototype parts too late
## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| BASED_ON | H2P-PW-003 | Strong | High | build plan should follow prototype purpose | prototyping literature |
| REQUIRES | H2P-PW-016 | Strong | High | configuration must be controlled enough to identify what was built | ISO 10007 / NASA SE |
| PRODUCES | H2P-PW-017 | Mandatory | High | executed build should create a build record | project methodology |
| ENABLES | H2P-PW-162 | Strong | High | planned builds improve structured learning capture | NASA lessons learned |
| CONSTRAINED_BY | H2P-PW-168 | Medium | Medium | external sourcing lead time can dominate build schedule | NPD lead-time literature |
## Sources
- NASA Systems Engineering Handbook: https://www.nasa.gov/reference/systems-engineering-handbook/
- NASA Systems Engineering Handbook Appendix, verification/test articles: https://www.nasa.gov/reference/system-engineering-handbook-appendix/
- Ford prototype test scheduling study: https://www.sciencedirect.com/science/article/pii/S0305048316302080
