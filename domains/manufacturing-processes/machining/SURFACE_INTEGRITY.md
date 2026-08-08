# 3.6.10 Surface Integrity

status: Researching
provenance: [GNR]

## 3.6.10.1 Definition
Surface integrity is treated as the condition of the manufactured surface and near-surface region, not merely a roughness value.

## 3.6.10.2 Objects
- Surface texture
- Roughness
- Waviness
- Lay
- Burr / edge condition
- Residual stress
- Work hardening
- Thermal damage
- Grinding burn
- Microcracking
- White/recast layer
- Metallurgical transformation
- Surface contamination

## 3.6.10.3 Engineering meaning
The drawing can be dimensionally compliant while the near-surface condition is unsuitable for fatigue, sealing, friction, coating, bonding or corrosion performance.

## 3.6.10.4 Functional links
Surface integrity -> influences -> fatigue
Surface texture -> influences -> sealing
Surface texture -> influences -> friction
Surface condition -> influences -> coating/bonding
Thermal damage -> may influence -> hardness/microstructure
EDM -> may create -> recast/heat-affected surface layer
Grinding -> may create -> thermal damage

## 3.6.10.5 Questions answered
1. When is Ra alone an insufficient specification?
2. Which functional surfaces require surface-integrity requirements beyond texture?
3. When should machining validation include residual stress, hardness, sectioning or metallography?
4. How should a process change be assessed when dimensions remain compliant but surface generation changes?

## 3.6.10.6 Decision objects
### D-SI-001 — Does this feature require a surface-integrity requirement?
Inputs: fatigue criticality, sealing, tribology, coating/bonding, corrosion, safety, process.

### D-SI-002 — Is secondary finishing required?
Candidates: reaming, honing, lapping, grinding, polishing, deburring, superfinishing.

## 3.6.10.7 Evidence backlog
- ISO GPS/surface texture standards and current revisions
- process-specific surface integrity literature
- fatigue and tribology literature
- NIST/metrology references

No numeric roughness or residual-stress recommendation is published here until source and functional scope are attached.