---
id: H2P-PW-067
title: Deburring
object_type: Process
domain: Prototype Workshop
subdomain: CNC & Subtractive Prototyping
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, Pilot]
status: Researching
provenance: [GNR, IND, SYN]
---

# 2.2.6.8 — Deburring

## 1. Definition
Controlled removal or conditioning of burrs and sharp edges created by cutting, drilling, milling and turning operations.

## 2. Why It Matters
Deburring is not merely cosmetic. Burrs can interfere with assembly, seals, sliding interfaces, inspection, wiring, handling safety and cleanliness. Conversely, uncontrolled edge breaking can alter critical dimensions or sealing edges.

## 3. Methods
- manual scraping/filing/abrasive finishing;
- chamfer tool or edge-break pass in CNC;
- tumbling/vibratory finishing;
- brushing;
- thermal/electrochemical methods for specialized production use.

## 4. Prototype Strategy
Where an edge is functionally critical, specify it explicitly rather than relying on a generic shop edge-break practice. Distinguish:
- 'remove burrs';
- defined chamfer/radius;
- sharp edge intentionally retained;
- sealing knife edge / metering edge / optical edge requiring special handling.

## 5. Relationships
| Type | Target | Strength | Confidence | Reason | Evidence |
|---|---|---:|---:|---|---|
| FOLLOWS | H2P-PW-049 CNC Milling | Strong | High | Milling commonly creates burrs | IND |
| FOLLOWS | H2P-PW-050 CNC Turning | Strong | High | Turning/cross holes/grooves create burrs | IND |
| AFFECTS | H2P-PW-066 Machining Surface Finish | Medium | High | Edge finishing can change local surface condition | IND |
| REQUIRES | H2P-PW-017 Prototype Build Record | Medium | Medium | Critical finishing state should be recorded | GNR+SYN |

## 6. Podcast Use
Listener tags: #CNC #Deburring #EdgeBreak #Finishing
