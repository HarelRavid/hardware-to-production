---
id: H2P-PW-065
title: CNC Tooling Selection
object_type: Method
domain: Prototype Workshop
subdomain: CNC & Subtractive Prototyping
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
provenance: [GNR, IND, SYN]
---

# 2.2.5 — CNC Tooling Selection

## 1. Definition
Selecting cutters, drills, reamers, boring tools, thread tools, holders and cutting-edge geometry appropriate to material, feature, machine capability and prototype objective.

## 2. Selection Dimensions
- workpiece material and hardness;
- roughing vs finishing objective;
- feature geometry and access;
- required reach and tool rigidity;
- spindle power/speed range;
- holder interface and runout;
- coolant/chip evacuation;
- expected tool wear;
- surface-finish and tolerance requirement.

## 3. Tool Families
- solid carbide end mills;
- indexable milling cutters;
- face mills;
- drills;
- reamers;
- boring bars/heads;
- thread mills/taps;
- chamfer/deburr tools;
- form/profile tools when justified.

Kennametal's current catalog illustrates that milling tool choice spans solid and indexable systems and that boring may require stiffness/vibration-control solutions; these are examples of tooling categories, not project-specific prescriptions.

## 4. Prototype Heuristic
For one-off hardware, prefer a simple standardized toolset unless a special tool materially reduces setups, enables an otherwise impossible feature or protects a critical tolerance. A custom/special tool can increase lead time more than it reduces cutting time.

## 5. Relationships
| Type | Target | Strength | Confidence | Reason | Evidence |
|---|---|---:|---:|---|---|
| DEPENDS_ON | H2P-PW-064 Prototype Machining Material Selection | Strong | High | Work material controls grade/geometry/speed limits | IND |
| USED_BY | H2P-PW-058 CAM for Prototyping | Mandatory | High | CAM requires exact cutter/holder definition | GOV+IND |
| AFFECTS | H2P-PW-066 Machining Surface Finish | Strong | High | Cutter geometry/runout/wear affect finish | NIST+IND |
| AFFECTS | H2P-PW-153 CAD-to-Part Lead Time | Medium | Medium | Special tooling can increase procurement/setup time | GNR+SYN |

## 6. Podcast Use
Listener tags: #CNC #Tooling #EndMills #Drilling #Boring
