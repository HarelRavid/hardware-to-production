# CNC Prototype Inspection & Metrology

Provenance: GNR + NIST/ASME evidence.

## 2.2.8.1 Inspection Strategy

Inspection should be driven by the engineering question and tolerance scheme, not by a generic desire to measure everything.

### Priority order
1. Functional interfaces and datums
2. Fits, seal lands, bearing seats and alignment features
3. Geometry controlling assembly or motion
4. Safety-critical dimensions
5. Cosmetic/noncritical dimensions only as needed

## 2.2.8.2 Measurement Method Selection

### Hand metrology
- Calipers: rapid general dimensional checks; limited for high-precision fits and geometric controls.
- Micrometers: higher-resolution external thickness/diameter measurements when geometry permits.
- Bore gauges / internal micrometers: controlled internal diameters.
- Height gauge + surface plate: useful for datum-referenced height/location checks.

### CMM / Optical
Use when the feature set, geometric tolerances, coordinate relationships or reporting needs justify coordinate measurement.

### On-machine probing
Useful for setup verification, work offsets, intermediate feature checks and potentially process correction. It does not automatically replace independent final inspection when machine error, thermal state or traceability requirements matter.

## 2.2.8.3 Datum-consistent inspection
A measurement method that does not reproduce the intended datum scheme can produce results that are difficult to compare with the drawing/model requirement.

## 2.2.8.4 Measurement uncertainty
Inspection capability must be adequate relative to the tolerance being evaluated. A tolerance should not be accepted or rejected using a measurement system whose uncertainty is too large for the decision.

## 2.2.8.5 Digital thread
NIST work on on-machine measurement demonstrates the value of linking product definition, manufacturing and dimensional measurement information in a standards-based digital thread.

## Key sources
- ASME Y14.5-2018 (R2024): GD&T design language and datum framework.
- NIST, On-Machine Measurement Use Cases and Information for Machining Operations (2019).
- NIST, Analysis of Dimensional Metrology Standards (NISTIR 6847).

## Relationships
- DEPENDS_ON: H2P-PW-062 Machining Datum Strategy
- VERIFIES: H2P-PW-063 Machining Tolerance Strategy
- SUPPORTS: H2P-PW-017 Prototype Build Record
- SUPPORTS: H2P-PW-018 Prototype Traceability
