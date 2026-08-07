---
id: H2P-PW-055
title: 3-axis Machining
object_type: Method
domain: Prototype Workshop
subdomain: CNC & Subtractive Prototyping
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
provenance: [GNR, GOV, IND, SYN]
---

# 2.2.1.3 — 3-axis Machining

## 1. Definition
CNC machining in which controlled cutting motion is generated in X, Y and Z while the workpiece orientation remains fixed during a setup.

## 2. Engineering Use
3-axis machining is the default prototype route for prismatic parts that can be accessed from a limited number of orientations. Its strength is simplicity: lower programming and setup complexity, broad machine availability, and strong compatibility with standard vises and modular workholding.

## 3. Decision Criteria
Prefer 3-axis when:
- critical features can be reached from one or a few orthogonal setups;
- the part is predominantly prismatic;
- setup count remains acceptable;
- undercuts and compound-angle access are limited;
- minimizing programming and machine cost matters more than eliminating every setup.

Escalate to indexed/continuous multi-axis when geometry or datum continuity makes repeated re-fixturing the dominant risk or cost driver.

## 4. Key Constraints
- tool access is directional;
- every reorientation introduces another setup and another opportunity for datum transfer error;
- deep cavities may require long-reach tooling, increasing deflection and chatter risk;
- internal sharp corners remain constrained by cutter radius.

## 5. Relationships
| Type | Target | Strength | Confidence | Reason | Evidence |
|---|---|---:|---:|---|---|
| ALTERNATIVE_TO | H2P-PW-057 5-axis Machining | Strong | High | Axis count changes access/setup strategy | GNR+IND |
| REQUIRES | H2P-PW-059 Prototype Workholding | Mandatory | High | Workpiece must be constrained | machining fundamentals |
| REQUIRES | H2P-PW-062 Machining Datum Strategy | Mandatory | High | Setup coordinates require datum logic | ASME Y14.5 context |
| ENABLES | H2P-PW-049 CNC Milling | Strong | High | Common milling architecture | industry practice |

## 6. Evidence
NIST high-speed prototype machining research demonstrates CNC milling as a rapid route for functional metallic prototypes and identifies intelligent path generation and pre-process verification as enabling requirements.

## 7. Podcast Use
Listener tags: #CNC #3Axis #PrototypeMachining #Workholding
