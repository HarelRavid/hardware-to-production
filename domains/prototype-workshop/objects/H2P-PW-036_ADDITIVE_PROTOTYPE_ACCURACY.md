# H2P-PW-036 — Additive Prototype Accuracy

```yaml
id: H2P-PW-036
title: Additive Prototype Accuracy
object_type: Concept
domain: Prototype Workshop
subdomain: Additive Manufacturing — Cross-cutting
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
summary: The achieved dimensional agreement between intended CAD geometry and the finished AM part, including machine, process, thermal, orientation, post-processing and measurement contributions.
tags: [accuracy, dimensional-metrology, AM, prototype]
created: 2026-08-07
last_reviewed: 2026-08-07
```

## 1. Definition
Additive prototype accuracy is not a single printer specification. It is the dimensional result of the full manufacturing chain from digital geometry through build, thermal history, support/removal or depowdering, post-processing and measurement.

## 2. Purpose
Determine whether an AM prototype is suitable for fit, tolerance, interface or verification decisions.

## 3. Problem Solved
Prevents engineers from using nominal machine resolution or layer height as a proxy for finished-part dimensional capability.

## 4. Inputs
CAD nominal geometry; process; material; orientation; build parameters; compensation; part size/geometry; post-processing; inspection method.

## 5. Outputs
Measured deviations, capability observations, compensation rules and acceptance decision.

## 6. Key Principle
Accuracy must be qualified at the process/material/machine/geometry level when it matters. NIST notes that complex AM surfaces, internal features and topology challenge conventional dimensional characterization and qualification.

## 7. Sources of Error
Thermal shrinkage/warpage; layer and voxel/path discretization; support interaction; powder-bed thermal history; curing; machine calibration; geometry-dependent compensation; finishing; measurement uncertainty.

## 8. Common Mistakes
Equating layer height with XY/Z accuracy; quoting vendor 'accuracy' without test geometry; measuring immediately when parts need conditioning/post-cure; assuming the same compensation works across size and geometry; ignoring inspection uncertainty.

## 9. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| AFFECTED_BY | H2P-PW-033 Additive Orientation Strategy | Strong | High | Orientation can change thermal, support and geometric outcomes. | AM metrology literature |
| AFFECTED_BY | H2P-PW-035 Additive Post-processing | Strong | High | Cure, support removal, blasting or finishing can alter dimensions. | Process principle |
| MEASURED_BY | H2P-PW-113 CMM | Medium | High | CMM may be appropriate for accessible geometries. | Metrology practice |
| MEASURED_BY | H2P-PW-114 Optical Measurement System | Medium | High | Optical systems can quantify appropriate external geometry. | Metrology practice |
| AFFECTS | H2P-PW-173 Prototype Manufacturing Process Selection | Strong | High | Required dimensional fidelity is a primary selection criterion. | Selection framework |
| SHOULD_BE_RECORDED_IN | H2P-PW-017 Prototype Build Record | Strong | High | Dimensional outcome needs traceable build context. | Knowledge governance |

## 10. Standards / Evidence
NIST dimensional-accuracy and AM qualification research is the current government anchor. Process-specific standards such as ISO/ASTM 52911-2 provide design guidance but do not justify universal tolerance numbers.

## 11. Open Questions
Build separate validated capability envelopes by FDM, SLA, SLS and MJF, then by material/machine class, with explicit sample geometry and measurement method.

## 12. Podcast Mapping
- Section: Prototype Shop
- Tags: #Accuracy #Metrology #AdditiveManufacturing
