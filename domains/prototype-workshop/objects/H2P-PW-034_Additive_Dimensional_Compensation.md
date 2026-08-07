---
id: H2P-PW-034
title: Additive Dimensional Compensation
object_type: Method
domain: Prototype Workshop
subdomain: Polymer Additive Manufacturing
lifecycle: [Prototype, Engineering Prototype, EVT, DVT]
status: Researching
---

# Additive Dimensional Compensation

## Definition
Intentional modification of nominal geometry or process settings to offset predictable dimensional bias such as shrinkage, hole undersize, warpage, support-related deformation, post-cure change, or axis-specific error.

## Why It Matters
A printed CAD nominal is not automatically the as-built nominal. Compensation should be based on measured process bias for the actual material, machine, orientation and post-process state.

## Typical Compensation Workflow
1. Define critical dimensions and datum scheme.
2. Print representative calibration artifacts using production-intent settings.
3. Measure systematic error separately from random variation.
4. Apply controlled geometry or process compensation only where bias is repeatable.
5. Reprint and verify.
6. Record the compensation in configuration-controlled build data.

## Examples of Bias Sources
- FDM: extrusion width, thermal contraction, elephant foot, anisotropic shrinkage, hole geometry, support interaction.
- SLA/MSLA: resin cure depth, support-induced distortion, wash/post-cure state and resin shrinkage.
- SLS/MJF: powder-bed thermal history, scale compensation, large-flat-surface warpage and hole/feature shrinkage.

## Engineering Rules
- Never treat a service-bureau tolerance as a compensation factor.
- Do not apply one global scale factor when error is geometry- or axis-dependent.
- For critical bores and interfaces, secondary machining may be more robust than aggressive CAD compensation.
- Compensation values should be versioned with machine/material/process settings and periodically revalidated.

## Relationships
| Type | Target Object | Strength | Confidence | Reason | Evidence |
|---|---|---:|---:|---|---|
| DEPENDS_ON | H2P-PW-036 | Mandatory | High | Compensation requires measured accuracy/bias | NIST accuracy work |
| DEPENDS_ON | H2P-PW-033 | Strong | High | Orientation changes error pattern | research/industrial evidence |
| AFFECTS | H2P-PW-029 | Strong | High | FDM design allowances may need compensation | industrial guidance |
| AFFECTS | H2P-PW-030 | Strong | High | Resin processes can change after cure | manufacturer data |
| AFFECTS | H2P-PW-031 | Strong | High | Powder-bed shrinkage and warpage require process-aware compensation | ISO/ASTM 52911-2 + industrial guidance |
| REQUIRES | H2P-PW-017 | Strong | High | Build records are needed to preserve compensation state | configuration-management logic |
