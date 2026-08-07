---
id: H2P-PW-017
title: Prototype Build Record
object_type: Document
domain: Prototype Workshop
subdomain: Strategy & Workshop Architecture
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, PVT]
status: Researching
summary: The authoritative record of what was physically built, how it differed from the intended configuration, and what evidence was generated from the build.
tags: [build-record, traceability, configuration, prototype]
---
# Prototype Build Record
## Definition
A Prototype Build Record captures the as-built state of a prototype rather than merely the as-designed state.
## Minimum Content
- build/unit ID
- build date and owner
- intended design baseline
- actual part/BOM revisions
- substitutions and deviations
- manufacturing route and important process parameters
- assembly notes and anomalies
- software/firmware versions
- test procedure/revision
- raw data and result links
- rework or changes made during debugging
## Principle
The record must preserve enough context that a later engineer can reconstruct what object produced the observed result.
## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| PRODUCED_BY | H2P-PW-006 | Mandatory | High | each planned build should generate an as-built record | project method |
| REQUIRES | H2P-PW-016 | Mandatory | High | as-built status needs controlled configuration identifiers | ISO 10007 |
| ENABLES | H2P-PW-018 | Mandatory | High | unit history is a prerequisite for prototype traceability | systems engineering practice |
| PROVIDES_EVIDENCE_FOR | H2P-PW-162 | Strong | High | build record provides facts used in learning capture | technical data management |
## Sources
- NASA Technical Data Management: https://www.nasa.gov/reference/6-6-technical-data-management/
- ISO 10007:2017: https://www.iso.org/standard/70400.html
