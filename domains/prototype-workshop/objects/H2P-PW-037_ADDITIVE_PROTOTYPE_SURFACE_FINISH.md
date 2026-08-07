# H2P-PW-037 — Additive Prototype Surface Finish

```yaml
id: H2P-PW-037
title: Additive Prototype Surface Finish
object_type: Concept
domain: Prototype Workshop
subdomain: Additive Manufacturing — Cross-cutting
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
summary: Surface condition produced by the AM process and subsequent finishing; affects cosmetics, sealing, friction, inspection, coating, bonding and sometimes dimensional interpretation.
tags: [surface-finish, roughness, AM, prototype]
created: 2026-08-07
last_reviewed: 2026-08-07
```

## 1. Definition
The topography and finish condition of an AM surface as delivered after build and any defined post-processing. It is process-, orientation-, geometry- and finishing-dependent.

## 2. Purpose
Determine whether an AM prototype can validly evaluate appearance, sealing, sliding, bonding/coating or surface-sensitive fit.

## 3. Problem Solved
Avoids treating a visually acceptable print as mechanically or functionally representative, and avoids comparing processes without specifying whether surfaces are raw or finished.

## 4. Key Drivers
Layer/voxel geometry; surface angle; powder particle interaction; support-contact surfaces; process energy; cure; blasting/polishing/tumbling/sanding; coating.

## 5. Process Context
FDM typically exhibits visible deposited-layer texture; SLA can deliver comparatively smooth and detailed surfaces but support-contact areas remain distinct; SLS/MJF exhibit powder-bed surface texture and are often blasted or otherwise finished.

## 6. Decision Criteria
Surface finish becomes a primary prototype-selection criterion for sealing interfaces, sliding parts, optics/cosmetics, coating/adhesive trials and tactile/user-facing prototypes.

## 7. Common Mistakes
Comparing raw FDM to post-processed MJF/SLS; quoting Ra without instrument/filter/cutoff and surface orientation; assuming one surface represents every orientation on a part; using cosmetic finishing that hides geometry defects needed for engineering learning.

## 8. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| AFFECTED_BY | H2P-PW-033 Additive Orientation Strategy | Strong | High | Surface angle/build direction changes layer/topography interaction. | AM metrology literature |
| AFFECTED_BY | H2P-PW-035 Additive Post-processing | Mandatory | High | Finishing can dominate delivered surface state. | Process principle |
| AFFECTS | H2P-PW-173 Prototype Manufacturing Process Selection | Strong | High | Surface requirements can drive process choice. | Selection framework |
| CHARACTERIZES | H2P-PW-021 FDM / FFF Printing | Strong | High | Layered deposition creates process-specific surfaces. | Process principle |
| CHARACTERIZES | H2P-PW-022 SLA Printing | Strong | High | Vat photopolymerization has distinct surface/support behavior. | Process principle |
| CHARACTERIZES | H2P-PW-024 SLS Polymer Printing | Strong | High | Powder-bed fusion yields characteristic granular surfaces. | NIST/ISO context |
| CHARACTERIZES | H2P-PW-025 MJF Printing | Strong | High | Powder-bed process and finishing define delivered surface. | Process principle |

## 9. Standards / Evidence
NIST treats surface finish as a core AM measurement and qualification challenge and has published dedicated dimensional-accuracy/surface-finish work. Process-specific quantitative values will be added only with defined material, machine and finishing condition.

## 10. Open Questions
Create raw-vs-finished surface condition matrices for FDM, SLA, SLS and MJF; link to sealing, friction, coating and bonding objects in later domains.

## 11. Podcast Mapping
- Section: Prototype Shop
- Tags: #SurfaceFinish #Roughness #AdditiveManufacturing
