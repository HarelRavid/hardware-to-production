# Polymer Additive Manufacturing — Engineering Claim Registry

This registry seeds the Engineering Claim layer for the Polymer AM cluster. Claims must follow `knowledge-os/ENGINEERING_CLAIM_MODEL.md`.

## H2P-CLM-000001 — FFF mechanical behavior is orientation-dependent

**Statement:** Mechanical properties of FDM/FFF polymer parts can vary materially with build orientation and toolpath/infill configuration; feedstock properties alone are insufficient to characterize part performance.

- Classification: Academic Evidence
- Confidence: High
- Evidence level: Peer-reviewed / academic + NIST process-characterization framework
- Applicable context: Material-extrusion polymer AM
- Limitations: Magnitude depends on material, machine, process parameters, geometry and test method.
- Related Objects: H2P-PW-021, H2P-PW-033, H2P-PW-176
- Supports Decisions: prototype orientation choice; functional-test suitability; material/process selection
- Evidence: SRC-PW-036; SRC-PW-030; SRC-PW-033

## H2P-CLM-000002 — Printer resolution is not dimensional accuracy

**Statement:** Nominal machine resolution, layer height, nozzle diameter or pixel size should not be treated as equivalent to finished-part dimensional accuracy.

- Classification: Project Synthesis
- Confidence: Very High
- Evidence level: Authoritative NIST measurement research
- Applicable context: Polymer AM; generally applicable to AM
- Limitations: Specific capability must be established for defined process/material/geometry/measurement conditions.
- Related Objects: H2P-PW-036, H2P-PW-021, H2P-PW-022, H2P-PW-024, H2P-PW-025
- Supports Decisions: tolerance allocation; inspection planning; process selection
- Evidence: SRC-PW-031; SRC-PW-032

## H2P-CLM-000003 — SLA post-cure state is part of the material state

**Statement:** For photopolymer SLA parts, mechanical and thermal properties can change substantially with post-cure conditions; a resin grade without its cure state is an incomplete material specification for engineering evaluation.

- Classification: Manufacturer-Specific Guidance + Project Synthesis
- Confidence: High
- Evidence level: Industrial technical data; process principle
- Applicable context: Photopolymer vat polymerization
- Limitations: Property changes are resin- and cure-cycle-specific.
- Related Objects: H2P-PW-022, H2P-PW-183, H2P-PW-177
- Supports Decisions: functional material selection; thermal test planning; test repeatability
- Evidence: Formlabs technical datasheets/material guidance captured in Polymer AM research

## H2P-CLM-000004 — Polymer PBF design requires process-specific rules

**Statement:** Polymer laser powder-bed fusion requires process-specific design guidance beyond generic AM design rules.

- Classification: Normative / Standards-Based Guidance
- Confidence: Very High
- Evidence level: Standard
- Applicable context: Laser-based polymer powder bed fusion
- Limitations: Applies to the scope of ISO/ASTM 52911-2 and does not automatically cover all polymer PBF variants.
- Related Objects: H2P-PW-024, H2P-PW-031, H2P-PW-178
- Supports Decisions: SLS design review; process selection; feature design
- Evidence: SRC-PW-025; SRC-PW-023

## H2P-CLM-000005 — Material-extrusion feedstock must be specified beyond polymer family name

**Statement:** For material-extrusion AM, engineering material specification should distinguish feedstock form and composition, including filled or reinforced variants, rather than relying only on a generic polymer-family label.

- Classification: Standards-Based Guidance
- Confidence: Very High
- Evidence level: Standard
- Applicable context: Plastic material-extrusion AM
- Limitations: Does not itself define finished-part performance.
- Related Objects: H2P-PW-021, H2P-PW-176
- Supports Decisions: material qualification; sourcing; prototype specification
- Evidence: SRC-PW-033

## H2P-CLM-000006 — AM numerical properties require process context

**Statement:** Numerical dimensional or mechanical properties for an AM part are not safely generalizable without preserving relevant process context such as material grade, machine/process family, orientation, conditioning, post-processing and test method.

- Classification: Project Synthesis
- Confidence: Very High
- Evidence level: NIST measurement/qualification research + process-specific standards
- Applicable context: Additive manufacturing
- Limitations: Context fields required depend on the property being claimed.
- Related Objects: H2P-PW-036, H2P-PW-033, H2P-PW-035, H2P-PW-176, H2P-PW-177, H2P-PW-178
- Supports Decisions: data comparison; material selection; validation planning
- Evidence: SRC-PW-030; SRC-PW-031; SRC-PW-032; SRC-PW-023

## H2P-CLM-000007 — Prototype process selection should follow the learning objective

**Statement:** The appropriate prototype manufacturing process depends on what the prototype is intended to learn or validate; visual, geometric, functional, material and production-process fidelity are separable objectives.

- Classification: Academic Consensus / Project Synthesis
- Confidence: High
- Evidence level: Peer-reviewed review + university guidance
- Applicable context: Prototype development
- Limitations: Does not prescribe a single process without project-specific constraints.
- Related Objects: H2P-PW-001, H2P-PW-002, H2P-PW-003, H2P-PW-173, H2P-PW-174
- Supports Decisions: H2P-DEC future process-selection decision
- Evidence: SRC-PW-001; SRC-PW-028

## H2P-CLM-000008 — Production representativeness is not equivalent to geometric similarity

**Statement:** A prototype can match production geometry while failing to represent production-process-induced material behavior, variation, defects or surface condition.

- Classification: Project Synthesis
- Confidence: High
- Evidence level: Cross-process engineering synthesis
- Applicable context: Prototype through DVT/PVT planning
- Limitations: Degree of required representativeness depends on the validation question.
- Related Objects: H2P-PW-174, H2P-PW-173
- Supports Decisions: prototype route selection; DVT readiness; production validation planning
- Evidence: SRC-PW-028; SRC-PW-023; process-specific standards

## H2P-CLM-000009 — Published design-rule numbers are process-specific starting points, not universal AM limits

**Statement:** Numerical wall, clearance, hole and tolerance values published by a service provider or machine vendor should be treated as capability guidance for a defined process context, not as universal limits for an AM technology.

- Classification: Project Synthesis
- Confidence: Very High
- Evidence level: NIST measurement framework + process-specific standards + industrial guides
- Applicable context: FDM, SLA, SLS, MJF and other AM processes
- Limitations: A specific supplier may warrant its own tighter or looser values.
- Related Objects: H2P-PW-029, H2P-PW-030, H2P-PW-031, H2P-PW-036
- Supports Decisions: tolerance allocation; supplier selection; design-rule use
- Evidence: SRC-PW-030; SRC-PW-031; ISO/ASTM 52911-2; Forge Labs FDM/MJF guides

## H2P-CLM-000010 — Critical AM bores and fits may require secondary machining or calibration

**Statement:** When a prototype contains critical bores, bearing seats, sealing diameters or controlled fits, printing to nominal alone may be less robust than printing with machining/calibration allowance and finishing the feature afterward.

- Classification: Industrial Best Practice / Project Synthesis
- Confidence: High
- Evidence level: Industrial design guidance + NIST accuracy framework
- Applicable context: Polymer AM prototypes with function-critical interfaces
- Limitations: Some validated machine/material combinations can meet requirements directly.
- Related Objects: H2P-PW-029, H2P-PW-030, H2P-PW-031, H2P-PW-034, H2P-PW-036
- Supports Decisions: hole strategy; fit strategy; post-processing route
- Evidence: Forge Labs FDM/MJF guides; SRC-PW-031

## H2P-CLM-000011 — FDM repeated-use fine threads are generally better implemented with inserts or post-machined threads

**Statement:** For repeated assembly in FDM thermoplastic prototypes, fine printed threads are generally less robust than appropriately designed inserts or post-machined/tapped features.

- Classification: Industrial Best Practice
- Confidence: High
- Evidence level: Industrial design guidance
- Applicable context: FDM prototype fastening
- Limitations: Large coarse printed threads can be adequate for low-load or low-cycle applications.
- Related Objects: H2P-PW-029, H2P-PW-182
- Supports Decisions: fastener strategy; enclosure/jig design
- Evidence: Forge Labs FDM Design Guidelines

## H2P-CLM-000012 — Powder-bed self-support does not eliminate design constraints

**Statement:** SLS/MJF generally avoid dedicated support structures because the powder bed supports geometry, but design must still address powder escape, thermal distortion, surface condition and machine/material-specific feature limits.

- Classification: Standards-Based Guidance + Industrial Best Practice
- Confidence: Very High
- Evidence level: ISO/ASTM 52911-2 + industrial design guidance
- Applicable context: Polymer powder-bed prototypes
- Limitations: MJF is not identical to laser PBF and requires its own capability record.
- Related Objects: H2P-PW-024, H2P-PW-025, H2P-PW-031, H2P-PW-032
- Supports Decisions: enclosed geometry; process selection; powder-removal design
- Evidence: SRC-PW-025; Formlabs Fuse design guidance; Forge Labs MJF guide

## H2P-CLM-000013 — Large flat powder-bed parts are a thermal-warpage risk

**Statement:** Large flat surfaces in polymer powder-bed AM are more susceptible to distortion and should not be treated as inherently tolerance-stable merely because supports are unnecessary.

- Classification: Industrial Best Practice / Standards Context
- Confidence: High
- Evidence level: Industrial guidance + process-specific standard scope
- Applicable context: SLS/MJF polymer parts
- Limitations: Magnitude depends on part size, orientation, material, nesting and process controls.
- Related Objects: H2P-PW-031, H2P-PW-034, H2P-PW-178
- Supports Decisions: orientation; process selection; dimensional validation
- Evidence: Forge Labs MJF Design Guidelines; ISO/ASTM 52911-2

## H2P-CLM-000014 — Dimensional compensation must be derived from measured systematic bias

**Statement:** CAD or process compensation should be based on repeatable measured bias for a defined machine/material/process state, rather than applying generic shrinkage factors or arbitrary oversizing.

- Classification: Project Synthesis
- Confidence: Very High
- Evidence level: NIST accuracy/qualification framework + configuration-management logic
- Applicable context: Additive manufacturing
- Limitations: Compensation is ineffective against primarily random variation.
- Related Objects: H2P-PW-034, H2P-PW-036, H2P-PW-017
- Supports Decisions: compensation strategy; validation planning; process capability
- Evidence: SRC-PW-031; SRC-PW-032

## Next Claim Work

Next expansion should create claims for:

- moisture sensitivity and conditioning of PA-family AM materials;
- support-induced surface and geometry effects in SLA/FFF;
- snap-fit and living-hinge suitability by material/process;
- environmental exposure limitations (UV, heat, chemical compatibility);
- supplier-specific clearance and minimum-feature rules with validated conditions.
