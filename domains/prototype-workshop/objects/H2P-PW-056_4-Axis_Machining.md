---
id: H2P-PW-056
title: 4-axis Machining
object_type: Method
domain: Prototype Workshop
subdomain: CNC & Subtractive Prototyping
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
provenance: [GNR, IND, SYN]
---

# 2.2.1.4 — 4-axis Machining

## 1. Definition
Machining that adds one rotational axis to the three linear axes, either for indexing between orientations or for simultaneous motion depending on the machine/control.

## 2. Engineering Use
Useful when several circumferential or side features must remain referenced to a common setup, or when rotary access can reduce manual re-fixturing.

## 3. Decision Criteria
Choose 4-axis when:
- cylindrical or quasi-cylindrical geometry has repeated features around an axis;
- multiple side faces can be machined by indexing;
- datum continuity is improved by retaining the part in one fixture;
- 5-axis flexibility is unnecessary or uneconomic.

## 4. Risks / Limitations
- rotary workholding can reduce accessible envelope;
- stock and fixture clearance must be simulated;
- simultaneous 4-axis toolpaths add programming and verification complexity;
- rotary-axis accuracy becomes part of the tolerance chain.

## 5. Relationships
| Type | Target | Strength | Confidence | Reason | Evidence |
|---|---|---:|---:|---|---|
| EXTENDS | H2P-PW-055 3-axis Machining | Strong | High | Adds rotational access | GNR+IND |
| ALTERNATIVE_TO | H2P-PW-057 5-axis Machining | Medium | High | Can solve many indexed-access needs with less complexity | industry practice |
| REDUCES | H2P-PW-059 Prototype Workholding | Medium | Medium | May reduce number of re-fixturing operations | GNR+SYN |
| DEPENDS_ON | H2P-PW-058 CAM for Prototyping | Strong | High | Rotary motion requires suitable CAM/post processing | industry practice |

## 6. Podcast Use
Listener tags: #CNC #4Axis #Indexing #SetupReduction
