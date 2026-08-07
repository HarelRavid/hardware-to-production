# H2P-PW-022 — SLA Printing

```yaml
id: H2P-PW-022
title: SLA Printing
aliases: [Stereolithography, Vat Photopolymerization]
object_type: Manufacturing Process
domain: Prototype Workshop
subdomain: Additive Manufacturing — Polymer
lifecycle: [POC, Prototype, Engineering Prototype, EVT]
status: Researching
summary: Vat-photopolymerization process valued for fine detail and smooth surfaces; performance depends strongly on resin chemistry, cure state, support strategy and post-cure, so geometric fidelity and material fidelity must be considered separately.
tags: [SLA, vat-photopolymerization, resin-printing, rapid-prototyping]
created: 2026-08-07
last_reviewed: 2026-08-07
```

## 1. Definition
Stereolithography is a vat-photopolymerization AM process in which selected regions of a liquid photopolymer are cured layer by layer using light.

## 2. Purpose
Produce detailed, visually refined and dimensionally useful prototypes where surface quality, small features and presentation quality are important.

## 3. Problem Solved
Provides a practical route to high-detail polymer prototypes without injection tooling or subtractive machining of every feature.

## 4. Lifecycle Position
Common from POC through EVT for form/fit models, fluidic geometries, housings, master patterns and selected functional prototypes. Later-stage use requires careful validation of resin aging, temperature, chemical and mechanical behavior.

## 5. Typical Owner / Responsible Roles
Mechanical engineer, prototype engineer, additive manufacturing engineer, workshop technician.

## 6. Inputs / Preconditions
CAD model; purpose/fidelity target; resin selection; orientation; supports; wash and post-cure plan; acceptance criteria.

## 7. Outputs / Deliverables
Printed and post-cured part; support-removal result; process settings; inspection data; build record.

## 8. How It Works
A light source selectively polymerizes a photoreactive resin. Parts are removed from the vat, cleaned and typically post-cured. Final dimensions and properties therefore depend on both the printing step and downstream wash/cure conditions.

## 9. Decision Criteria
Prefer when fine detail, smooth surface, transparent/optical variants, small channels or presentation quality outweigh the need for production-polymer equivalence. Avoid assuming resin behavior represents molded thermoplastics.

## 10. Alternatives and Tradeoffs
FDM for low-cost fast workshop iteration; SLS/MJF for support-free powder-bed parts and nested batches; CNC for stock-material mechanical fidelity and precision interfaces.

## 11. Limitations / Failure Conditions
Support contact marks; resin shrinkage and cure effects; uncured resin handling; post-cure dependency; photopolymer aging/environmental sensitivity; trapped resin in enclosed cavities; brittle behavior in some resin families.

## 12. Common Mistakes
Equating excellent visual finish with production readiness; testing mechanical behavior before controlled post-cure; ignoring resin drainage; designing inaccessible support regions; generalizing properties from one resin family to all SLA.

## 13. Standards and Regulations
ISO/ASTM 52900 provides the vat-photopolymerization process category and terminology. Application-specific and material-specific standards should be linked when evidence is available. Ceramic vat-photopolymerization feedstock characterization is covered separately by ISO/ASTM 52940:2025 and should not be generalized to ordinary polymer resins.

## 14. Academic Evidence
Photopolymer AM literature shows that cure state, exposure, orientation and aging can influence dimensions and mechanical properties; numeric claims must remain resin- and process-specific.

## 15–18. Additional Sources / Case Studies
To be expanded during the dedicated SLA depth pass.

## 19. Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---|---|---|---|
| SPECIALIZES | H2P-PW-173 Prototype Manufacturing Process Selection | Strong | High | SLA is one process option in the common selection framework. | Knowledge architecture |
| REQUIRES | H2P-PW-032 Additive Support Strategy | Strong | High | Most SLA workflows require explicit support planning. | Process principle |
| REQUIRES | H2P-PW-033 Additive Orientation Strategy | Strong | High | Orientation influences supports, surface and dimensional result. | AM literature |
| REQUIRES | H2P-PW-035 Additive Post-processing | Mandatory | High | Cleaning and post-cure are integral to the finished SLA part. | Process principle |
| AFFECTS | H2P-PW-036 Additive Prototype Accuracy | Strong | High | Exposure, cure and orientation influence dimensions. | NIST AM metrology context |
| AFFECTS | H2P-PW-037 Additive Prototype Surface Finish | Strong | High | SLA is commonly selected for fine surface/detail. | Process literature |
| ALTERNATIVE_TO | H2P-PW-021 FDM / FFF Printing | Medium | High | Both support polymer rapid prototyping with different tradeoffs. | Process comparison |
| ALTERNATIVE_TO | H2P-PW-024 SLS Polymer Printing | Medium | High | Support requirement and material behavior differ materially. | Process comparison |

## 20. Open Questions / Evidence Gaps
Build a resin-family taxonomy for mechanical, thermal, chemical and aging fidelity; quantify post-cure sensitivity using standardized sources.

## 21. Podcast Mapping
- Relevant section: Prototype Shop
- Candidate episode(s): Polymer 3D Printing; Choosing a Prototype Process
- Listener tags: #SLA #VatPhotopolymerization #ResinPrinting
- Prerequisite objects: H2P-PW-001, H2P-PW-002, H2P-PW-173

## 22–23. Future Mapping
Reserved.

## 24. Revision Notes
Initial research-backed object created 2026-08-07.
