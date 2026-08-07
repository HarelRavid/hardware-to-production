---
id: H2P-PW-060
title: Soft Jaws
object_type: Tool
domain: Prototype Workshop
subdomain: CNC & Subtractive Prototyping
lifecycle: [Prototype, Engineering Prototype, EVT, DVT, Pilot]
status: Researching
provenance: [GNR, IND, SYN]
---

# 2.2.4.2 — Soft Jaws

## 1. Definition
Custom-machined vise or chuck jaws used to locate and clamp a specific prototype geometry with greater conformity, repeatability or access than standard hard jaws.

## 2. Why Use Them
Soft jaws are useful when a prototype has irregular external geometry, needs a second-operation datum, must be protected from clamp damage, or will be produced in a small repeat batch where repeated location matters.

## 3. Design Considerations
- machine the jaws in the same clamped/preloaded state used during production;
- create positive location where practical rather than relying only on friction;
- avoid over-constraining compliant parts;
- preserve cutter access and chip evacuation;
- include sufficient jaw engagement to resist cutting loads;
- define how the part will be removed without damaging finished surfaces.

## 4. Common Failure Modes
- jaws machined without preload, causing position error under actual clamping;
- insufficient grip area;
- distortion of thin-wall parts;
- locating on a surface that is not stable from part to part;
- loss of datum after a jaw revision without configuration control.

## 5. Relationships
| Type | Target | Strength | Confidence | Reason | Evidence |
|---|---|---:|---:|---|---|
| USED_BY | H2P-PW-059 Prototype Workholding | Strong | High | Common custom workholding method | industry practice |
| SUPPORTS | H2P-PW-062 Machining Datum Strategy | Strong | High | Can create repeatable second-operation reference | GNR+SYN |
| ALTERNATIVE_TO | H2P-PW-061 Modular Fixturing | Medium | High | Custom vs reusable fixture strategy | industry practice |
| REDUCES | H2P-PW-153 CAD-to-Part Lead Time | Medium | Medium | Reusable jaws can shorten repeat setups | GNR+SYN |

## 6. Podcast Use
Listener tags: #CNC #SoftJaws #Workholding #Fixtures
