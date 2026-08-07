# H2P-PW-033 — Additive Orientation Strategy

```yaml
id: H2P-PW-033
title: Additive Orientation Strategy
object_type: Method
domain: Prototype Workshop
subdomain: Additive Manufacturing — Cross-cutting
lifecycle: [POC, Prototype, Engineering Prototype, EVT, DVT]
status: Researching
summary: Deliberate selection of build orientation to control mechanical response, support demand, dimensional outcome, surface condition, build time and post-processing accessibility.
tags: [orientation, build-direction, anisotropy, additive-manufacturing]
created: 2026-08-07
last_reviewed: 2026-08-07
```

## 1. Definition
A structured method for choosing how a part is positioned in the AM build space based on the prototype objective and the process-specific consequences of that orientation.

## 2. Purpose
Prevent orientation from being treated as a slicer convenience. It is an engineering variable that can change measured prototype behavior.

## 3. Problem Solved
A prototype may fail or pass because of build orientation rather than because the underlying design is poor or good. Orientation strategy reduces this ambiguity.

## 4. Lifecycle Position
Relevant to every AM prototype; importance increases as prototypes are used for structural, dimensional or qualification decisions.

## 5. Inputs
Load directions; critical surfaces; tolerances; support access; process family; material; post-processing; build-volume constraints.

## 6. Outputs
Chosen build orientation plus engineering rationale recorded in the build record.

## 7. Decision Criteria
Prioritize the dimensions, interfaces and load paths that the prototype is intended to evaluate. Orientation should explicitly balance structural anisotropy, support/contact surfaces, stair-stepping, thermal distortion, drainage/depowdering, throughput and inspection access.

## 8. Key Engineering Rule
Orientation is part of the experimental design. If structural behavior is being compared across revisions, uncontrolled orientation changes can confound the result.

## 9. Process Differences
- FDM/FFF: layer interfaces and raster/toolpath orientation can strongly influence mechanical response.
- SLA/MSLA: support placement, peel/curing behavior and post-cure interact with orientation.
- SLS/MJF: external supports are generally unnecessary, but orientation still influences thermal history, feature quality, nesting and depowdering.

## 10. Common Mistakes
Auto-orienting without documenting rationale; changing orientation between prototype revisions; reporting material strength without build direction; orienting only for shortest print time; ignoring critical-surface finish.

## 11. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| AFFECTS | H2P-PW-021 FDM / FFF Printing | Strong | High | FFF mechanical behavior depends on build/toolpath direction. | Academic literature |
| AFFECTS | H2P-PW-022 SLA Printing | Strong | High | Orientation changes supports and finish. | Process principle |
| AFFECTS | H2P-PW-024 SLS Polymer Printing | Strong | High | Orientation/nesting influences thermal and geometric results. | PBF guidance |
| AFFECTS | H2P-PW-025 MJF Printing | Strong | High | Orientation remains relevant despite support-free powder bed. | Process principle |
| AFFECTS | H2P-PW-036 Additive Prototype Accuracy | Strong | High | Dimensional error can be orientation dependent. | NIST metrology work |
| AFFECTS | H2P-PW-037 Additive Prototype Surface Finish | Strong | High | Surface angle to layers/build direction changes texture. | AM metrology literature |
| SHOULD_BE_RECORDED_IN | H2P-PW-017 Prototype Build Record | Mandatory | High | Orientation is required context for reproducing and interpreting a build. | Knowledge governance |

## 12. Open Questions
Develop process-specific orientation checklists and evidence ranges by technology/material family.

## 13. Podcast Mapping
- Section: Prototype Shop
- Tags: #BuildOrientation #Anisotropy #3DPrinting
