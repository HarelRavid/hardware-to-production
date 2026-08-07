---
id: H2P-PW-066
title: Machining Surface Finish
object_type: Concept
domain: Prototype Workshop
subdomain: CNC & Subtractive Prototyping
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
provenance: [GNR, GOV, IND, STD, SYN]
---

# 2.2.6.6 — Machining Surface Finish

## 1. Definition
The resulting surface texture and condition created by the machining process and any subsequent finishing operation.

## 2. Engineering Relevance
Surface finish can affect sealing, friction, wear, fatigue, optical/cosmetic appearance, coating adhesion and dimensional inspection. A requirement should therefore be linked to function rather than applied uniformly to every surface.

## 3. Process Drivers
- cutter geometry and edge condition;
- feed per tooth / feed rate;
- spindle speed and stability;
- tool runout and holder rigidity;
- workpiece stiffness and clamping;
- material behavior;
- coolant/lubrication;
- finishing strategy and remaining stock.

NIST notes improved surface finish as one potential benefit of high-speed machining while also emphasizing system dynamics and tool wear as controlling factors.

## 4. Specification Rule
Use a defined surface-texture specification and measurement method where finish is functional. Do not substitute visual appearance or a generic 'as-machined' label for a quantified requirement when sealing, tribology or fatigue depends on it.

ISO 21920 is part of the current ISO GPS framework for profile surface texture; exact applicable part/edition should be checked when formal requirements are authored.

## 5. Relationships
| Type | Target | Strength | Confidence | Reason | Evidence |
|---|---|---:|---:|---|---|
| AFFECTED_BY | H2P-PW-065 CNC Tooling Selection | Strong | High | Tool condition/geometry affect texture | GOV+IND |
| AFFECTED_BY | H2P-PW-058 CAM for Prototyping | Strong | High | Finishing paths and feeds affect finish | GOV+IND |
| MEASURED_BY | H2P-PW-115 Surface Roughness Measurement | Mandatory | High | Quantified finish needs metrology | STD+IND |
| SUPPORTS | H2P-PW-174 Prototype Production Representativeness | Medium | High | Surface state can be functionally representative or misleading | GNR+SYN |

## 6. Podcast Use
Listener tags: #CNC #SurfaceFinish #Roughness #FunctionalSurface
