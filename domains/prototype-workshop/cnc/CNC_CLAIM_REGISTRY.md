# 2.2 CNC & Subtractive Prototyping — Engineering Claim Registry

All AI-originated claims carry `GNR` provenance per ADR-003. A claim may also carry external evidence provenance after verification.

## H2P-CLM-CNC-001 — High-speed CNC can function as rapid prototyping for metallic functional parts
Statement: CNC machining can serve as a rapid-prototyping route for functional metallic parts when machine dynamics, tool wear, path generation and pre-process verification are controlled.
- Classification: Academic/Government Evidence
- Confidence: High
- Provenance: [GNR, GOV, PPR]
- Evidence: NIST Schmitz et al. 2001
- Related Objects: H2P-PW-049, H2P-PW-058, H2P-PW-200

## H2P-CLM-CNC-002 — More axes are not automatically better
Statement: Increasing axis count can reduce re-fixturing and improve access, but also increases programming, simulation, machine and setup complexity; 5-axis is justified when those benefits exceed the added burden.
- Classification: Project Synthesis / Industry Practice
- Confidence: High
- Provenance: [GNR, IND, SYN]
- Related Objects: H2P-PW-055, H2P-PW-056, H2P-PW-057

## H2P-CLM-CNC-003 — Workholding is part of the tolerance system
Statement: Workholding influences achievable geometry because location error, clamping distortion and setup transfer can become part of the dimensional error budget.
- Classification: Engineering Synthesis
- Confidence: Very High
- Provenance: [GNR, IND, SYN]
- Related Objects: H2P-PW-059, H2P-PW-060, H2P-PW-061, H2P-PW-062, H2P-PW-063

## H2P-CLM-CNC-004 — Tight tolerances should be allocated by function, not capability alone
Statement: A prototype should not receive tight tolerances simply because CNC can achieve them; tolerance should be tied to fit, sealing, alignment, motion, stack-up or validation need.
- Classification: Industry Best Practice / Project Synthesis
- Confidence: Very High
- Provenance: [GNR, IND, SYN, STD]
- Evidence: ASME Y14.5 context; Protolabs/Xometry tolerance guidance
- Related Objects: H2P-PW-063, H2P-PW-199

## H2P-CLM-CNC-005 — Internal sharp corners are constrained by cutter geometry
Statement: Conventional milling produces an internal radius based on the cutting tool, so internal sharp corners generally require redesign, relief geometry, EDM or another process.
- Classification: Manufacturing Fact
- Confidence: Very High
- Provenance: [GNR, IND]
- Evidence: Protolabs CNC milling guidance
- Related Objects: H2P-PW-049, H2P-PW-065

## H2P-CLM-CNC-006 — Deep features can be limited by tool access and rigidity before nominal machine travel
Statement: Deep holes and cavities can become impractical because of chip evacuation, long tool reach, deflection, chatter and standardized tool availability even when the machine envelope is large enough.
- Classification: Industry Best Practice
- Confidence: High
- Provenance: [GNR, IND]
- Evidence: Protolabs DFM guidance; machining-tool literature
- Related Objects: H2P-PW-065, H2P-PW-197, H2P-PW-199

## H2P-CLM-CNC-007 — Thin walls create a coupled accuracy-cost problem
Statement: Thin/tall walls reduce workpiece stiffness, increasing vibration and distortion risk; holding tight geometry can therefore require slower machining, support strategy or process redesign.
- Classification: Industry Guidance
- Confidence: High
- Provenance: [GNR, IND]
- Evidence: Xometry thin-wall guidance
- Related Objects: H2P-PW-059, H2P-PW-199

## H2P-CLM-CNC-008 — Setup count is a major prototype cost and lead-time driver
Statement: For low-volume CNC prototypes, reducing a setup can be more valuable than marginally reducing cutting cycle time because setup planning, workholding, re-datuming and inspection recur at low quantities.
- Classification: Project Synthesis
- Confidence: High
- Provenance: [GNR, IND, SYN]
- Related Objects: H2P-PW-055, H2P-PW-057, H2P-PW-059, H2P-PW-199, H2P-PW-200

## H2P-CLM-CNC-009 — Hole process should be chosen by function
Statement: Drilling, interpolation, reaming and boring are not interchangeable; the appropriate process depends on diameter, depth, positional requirement, finish and fit/function.
- Classification: Industry Practice
- Confidence: Very High
- Provenance: [GNR, IND]
- Related Objects: H2P-PW-197, H2P-PW-063, H2P-PW-065

## H2P-CLM-CNC-010 — Thread depth guidance is provider/process-specific
Statement: Quick-turn supplier rules such as a maximum preferred thread-depth ratio are manufacturing-service rules, not universal physical limits of threading.
- Classification: Project Synthesis
- Confidence: Very High
- Provenance: [GNR, IND, SYN]
- Evidence: Protolabs threaded-hole guidance
- Related Objects: H2P-PW-198

## H2P-CLM-CNC-011 — Surface finish must be linked to function and measurement
Statement: When surface texture affects sealing, friction, fatigue or wear, a quantified surface requirement and measurement method are more meaningful than a generic 'as machined' description.
- Classification: Standards Context / Project Synthesis
- Confidence: High
- Provenance: [GNR, STD, SYN]
- Related Objects: H2P-PW-066, H2P-PW-115

## H2P-CLM-CNC-012 — Same material does not guarantee production-process representativeness
Statement: Machining the intended production material can improve material fidelity but may not reproduce production-process effects such as molding orientation, cast defects, forged grain flow or molded residual stress.
- Classification: Project Synthesis
- Confidence: High
- Provenance: [GNR, SYN]
- Related Objects: H2P-PW-064, H2P-PW-174

## H2P-CLM-CNC-013 — CAM simulation is part of prototype risk control
Statement: CAM verification should include stock, tool, holder and fixture context, especially for multi-axis work, because collision or unreachable stock can destroy a rapid-iteration schedule.
- Classification: Government/Industry Evidence + Synthesis
- Confidence: High
- Provenance: [GNR, GOV, IND, SYN]
- Evidence: NIST prototype machining requirements
- Related Objects: H2P-PW-058, H2P-PW-057

## H2P-CLM-CNC-014 — Special tooling can increase lead time more than it saves cycle time in one-off prototypes
Statement: For one-off or very low quantity builds, special tool procurement/design should be justified against elapsed lead time rather than production cycle-time optimization alone.
- Classification: Project Synthesis
- Confidence: Medium-High
- Provenance: [GNR, IND, SYN]
- Related Objects: H2P-PW-065, H2P-PW-200

## H2P-CLM-CNC-015 — Deburring state can be function-critical
Statement: Burr removal and edge break can affect assembly, sealing, handling, inspection and cleanliness; critical edges should therefore be explicitly defined rather than left entirely to shop convention.
- Classification: Industry Practice / Project Synthesis
- Confidence: High
- Provenance: [GNR, IND, SYN]
- Related Objects: H2P-PW-067
