# Polymer AM — Flex, Moisture and Environment Claims

Continuation of the canonical claim registry. Claim IDs remain globally unique.

## H2P-CLM-000015 — Snap-fit suitability depends on material ductility and print orientation

**Statement:** A printed snap-fit cannot be evaluated from geometry alone; material ductility/toughness and build orientation materially affect whether the flexing member survives insertion, retention and repeated use.

- Classification: Industrial Best Practice + Project Synthesis
- Confidence: High
- Applicable context: Polymer AM snap-fit prototypes
- Limitations: Required cycles, strain, geometry and process settings must be defined.
- Related Objects: H2P-PW-197, H2P-PW-033, H2P-PW-176, H2P-PW-177, H2P-PW-178
- Supports Decisions: material selection; orientation; snap-fit prototype validity
- Evidence: Formlabs Tough Resin V5 guidance; AM orientation evidence; current industrial design guidance

## H2P-CLM-000016 — Printed living hinges are not automatically production-representative

**Statement:** An additively manufactured living hinge may validate motion and packaging geometry while failing to represent the fatigue life and process-induced material structure of an injection-molded living hinge.

- Classification: Project Synthesis
- Confidence: High
- Applicable context: Prototype of future molded living-hinge parts
- Limitations: A production AM hinge is a different case and should be validated as its own process/material system.
- Related Objects: H2P-PW-198, H2P-PW-174
- Supports Decisions: prototype intent; DVT planning; living-hinge validation route
- Evidence: Formlabs resin-specific hinge guidance + process-representativeness model

## H2P-CLM-000017 — Support contact is a functional surface condition when the surface matters

**Statement:** For support-dependent AM processes, support contact and removal can alter local surface and geometry enough that support placement must be treated as a design variable on sealing, bearing, cosmetic, datum and fit-critical surfaces.

- Classification: Industrial Best Practice / Project Synthesis
- Confidence: High
- Applicable context: FDM/FFF and vat photopolymerization
- Limitations: Magnitude depends on support material/interface, geometry and post-processing.
- Related Objects: H2P-PW-199, H2P-PW-032, H2P-PW-037, H2P-PW-036
- Supports Decisions: orientation; support placement; machining allowance; inspection planning
- Evidence: process design guidance + NIST AM accuracy/surface framework

## H2P-CLM-000018 — Moisture condition can be part of the material/test configuration

**Statement:** For moisture-sensitive polymer AM systems, material/feedstock and printed-part conditioning state should be controlled and recorded whenever it can affect processing, dimensional response or measured mechanical performance.

- Classification: Industrial Best Practice + Project Synthesis
- Confidence: High
- Applicable context: Hygroscopic AM polymers, particularly polyamides
- Limitations: Degree of sensitivity is formulation-specific; not all nylons or filled grades behave alike.
- Related Objects: H2P-PW-179, H2P-PW-017, H2P-PW-176, H2P-PW-178
- Supports Decisions: material preparation; test comparability; build-record content
- Evidence: current UltiMaker Nylon guidance; PBF material datasets; polymer conditioning practice

## H2P-CLM-000019 — Environmental suitability must be evaluated by exposure mode and duration

**Statement:** A polymer-AM material label such as 'tough', 'nylon' or 'high strength' does not establish suitability for heat, UV, chemicals, humidity, creep or sustained load; environmental validity requires evidence for the exact material/process state and exposure mode.

- Classification: Project Synthesis
- Confidence: Very High
- Applicable context: Functional prototype and EVT/DVT testing
- Limitations: Short-term exposure and long-term service aging are separate questions.
- Related Objects: H2P-PW-180, H2P-PW-174, H2P-PW-176, H2P-PW-177, H2P-PW-178
- Supports Decisions: functional test validity; environmental-test material selection; production representativeness
- Evidence: UltiMaker Nylon technical guidance; Formlabs Tough Resin V5 limitations; material-specific TDS practice
