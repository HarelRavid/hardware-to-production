# 2.2.8 CNC Inspection Capability & Measurement Uncertainty

provenance: [GNR, GOV, STD, SYN]
status: Researching

## 2.2.8.1 Core principle
A measurement result is an estimate, not absolute truth. Inspection planning must consider whether the measurement system has adequate capability and uncertainty relative to the tolerance or engineering decision.

## 2.2.8.2 On-machine probing
NIST work on touch-trigger probing evaluates probing repeatability, 2D/3D probing errors and workpiece-coordinate-system identification errors, explicitly as inputs to on-machine measurement uncertainty budgets.

On-machine probing is valuable for:
- work offset establishment
- setup verification
- process-intermittent checks
- detecting certain tool/process errors
- supporting closed-loop compensation

It should not automatically be treated as equivalent to independent final inspection.

## 2.2.8.3 Why independent measurement can still matter
NIST research on process-intermittent inspection distinguishes process errors detectable in-machine (for example tool setting, wear, tool or part deflection) from machine-tool geometric errors that can require inspection independent of the machine tool to identify reliably.

## 2.2.8.4 Measurement planning
For each critical characteristic define:
1. measurand / requirement
2. datum/reference scheme
3. measurement method
4. instrument capability
5. environmental conditions where relevant
6. sampling/repeat strategy
7. acceptance rule
8. measurement uncertainty or at minimum a justified capability margin

## 2.2.8.5 GR&R caution
Repeatability and reproducibility studies are useful for process understanding but should not automatically be interpreted as complete measurement uncertainty. NIST has published explicitly on the distinction and on methods for uncertainty R&R.

## 2.2.8.6 Prototype context
During early prototypes, inspection should be proportional to the learning objective. During EVT/DVT or supplier qualification, evidence needs become more formal and traceable.

## Relationships
- SUPPORTS -> H2P-PW-063 Machining Tolerance Strategy
- SUPPORTS -> H2P-PW-018 Prototype Traceability
- DEPENDS_ON -> H2P-PW-062 Machining Datum Strategy
- RELATED_TO -> H2P-PW-113 CMM
- RELATED_TO -> H2P-PW-114 Optical Measurement System

## Sources
- NIST: Methods, Practices, and Standards for Evaluating On-Machine Touch Trigger Probing of Workpieces (2010)
- NIST AMS 400-1: On-Machine Measurement Use Cases and Information for Machining Operations (2019)
- NISTIR 6415: Fast Probing Considerations for On-Machine Inspection of Parts (1999)
- NIST: A Methodology for Compensating Errors Detected by Process-Intermittent Inspection (2001)
- NIST: Uncertainty and Dimensional Calibrations (1997)
- NIST: Dimensional Measurement Uncertainty from Data, Part 2: Uncertainty R&R (2016)
