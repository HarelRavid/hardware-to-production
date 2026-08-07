# 2.2.10 CNC Prototype Case Studies

provenance: [GNR, GOV, IND, SYN]
status: Researching

## 2.2.10.1 NIST high-speed CNC as rapid prototyping
NIST documented high-speed machining as a route to monolithic metallic functional prototypes with process times competitive with other rapid-prototyping routes. The case is useful because it reframes CNC from 'production machining only' into a development tool when spindle capability, system dynamics, tool wear, path generation and verification are controlled.

### Lessons
- CNC can be a rapid-prototyping method when the required fidelity is functional and metallic.
- Toolpath generation and verification are part of the rapid-prototyping system, not administrative overhead.
- Machine dynamics and tool wear can dominate the practical parameter window.

## 2.2.10.2 NIST Instrument Maker Shop high-speed machining experience
NIST summarized shop-floor implementation lessons from its Instrument Maker Shop. This case is useful for prototype workshops because it ties high-speed-machining theory to real internal fabrication capability.

### Lessons
- In-house machining value is tied to engineering access and iteration, not only part cost.
- Stable process knowledge accumulates through repeated use of the same equipment and tooling system.

## 2.2.10.3 Closed-loop/on-machine inspection research
NIST work on process-intermittent and on-machine inspection demonstrates a development pattern where measurement is integrated into the machining loop to detect and compensate certain process errors before the final cut.

### Lessons
- Measurement can be part of the manufacturing process rather than only final acceptance.
- Not all error sources are observable in the same coordinate/reference system.
- Independent metrology remains important where machine-tool geometry itself could bias the result.

## 2.2.10.4 Difficult-to-machine material example
Seco documents titanium/stainless stacked machining as an example where parameters, chip control, coolant delivery and tool geometry must be designed around the more difficult material behavior.

### Lessons
- 'Machinability' is contextual.
- Mixed-material or high-performance prototypes can require conservative parameter selection based on the limiting material.
- Material choice can transform lead time and process risk even when geometry is unchanged.

## Relationships
- SUPPORTS -> H2P-PW-049 CNC Milling
- SUPPORTS -> H2P-PW-058 CAM for Prototyping
- SUPPORTS -> H2P-PW-064 Prototype Machining Material Selection
- SUPPORTS -> H2P-PW-200 CNC Prototype Lead-Time Drivers

## Sources
- NIST, Schmitz et al. (2001), The Application of High-Speed CNC Machining to Prototype Production
- NIST, Davies et al. (2001), How to Succeed at High Speed Machining
- NIST, on-machine measurement and process-intermittent inspection publications
- Seco Tools, difficult-to-machine materials guidance
