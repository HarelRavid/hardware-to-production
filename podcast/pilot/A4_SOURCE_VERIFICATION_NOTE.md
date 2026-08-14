# A4 Source Verification Note — Prototype Representativeness

status: SOURCE VERIFICATION — INITIAL PASS
supports: `podcast/pilot/A4_RESEARCH_PACK.md`

## Purpose

Provide authoritative external support for A4 without pretending that the repository's `REPRESENT 8` or shortcut-expiration framework is itself an external standard.

## Verified source anchors

### NASA Systems Engineering Handbook — verification/validation planning and test-article pedigree

Authoritative source: NASA Systems Engineering Handbook, Appendix / V&V guidance.

Relevant support:
- verification plans distinguish analysis, inspection, demonstration and test;
- qualification testing may be performed at component, subsystem or system level;
- V&V planning should identify the pedigree of test articles, including breadboards, prototypes, engineering units, qualification units and other article types;
- the type of test/analysis performed on each article should be described;
- developmental/engineering-unit evaluations are distinguished from formal verification activities.

A4 use:
This supports the principle that evidence must be interpreted in the context of the article/configuration and test purpose that produced it. It does NOT by itself prescribe our representativeness vector or shortcut-expiration tool.

Source:
https://www.nasa.gov/reference/system-engineering-handbook-appendix/

### GAO — production-representative prototypes and manufacturing-readiness evidence

Authoritative source: U.S. Government Accountability Office, GAO-06-368 and GAO-10-439 manufacturing-readiness work.

Relevant support:
- GAO identified production-representative prototypes and demonstrated manufacturing processes as important evidence before production commitment;
- GAO's discussion of Manufacturing Readiness Levels distinguishes laboratory/prototype capability from production-relevant/production-representative environments and later pilot/low-rate/full-rate production capability.

A4 use:
This supports the episode's warning that a successful prototype does not automatically establish manufacturing readiness, and that production-relevant evidence becomes progressively more important as a program approaches production.

Sources:
https://www.gao.gov/products/gao-06-368
https://www.gao.gov/assets/a303517.html

Guardrail:
Do not present DOD MRL levels as universal startup lifecycle requirements. DEV/LVP/SVP remains our editorial synthesis.

### NIST — manufacturability/process planning should be considered during design

Authoritative source family: NIST Design and Process Planning Integration publications.

Relevant support:
- NIST describes conceptual process planning as a way for designers to evaluate manufacturability and manufacturing cost early in product development;
- manufacturing process/resource selection depends on design factors including material, form, geometry/features, dimensions, tolerances, surface condition, production volume and production rate.

A4 use:
This supports the idea that changing material, process, tolerance, surface, volume/rate or resource assumptions can change the manufacturing conclusions that can legitimately be drawn from an earlier prototype route.

Sources:
https://www.nist.gov/publications/conceptual-process-planning-definition-and-functional-decomposition
https://www.nist.gov/publications/preliminary-design-and-manufacturing-planning-integration-using-intelligent-agents

## Claim disposition

| Claim | Disposition after initial pass |
|---|---|
| A4-C01 | CLAIM SET STABLE as repository synthesis supported by NASA/GAO evidence-context and production-representativeness principles. |
| A4-C02 | CLAIM SET STABLE as synthesis; process-specific examples still require process-source verification before final script. |
| A4-C03 | CLAIM SET STABLE as synthesis; NIST supports multiple design/manufacturing dimensions affecting process planning. |
| A4-C04 | CLAIM SET STABLE as internal lifecycle guidance. |
| A4-C05 | CLAIM SET STABLE as internal lifecycle guidance; do not universalize EVT/DVT/PVT or MRL schemes. |
| A4-C06 | CLAIM SET STABLE via frozen P2.02 evidence-dependency/change-control invariant. |
| A4-C07 | CLAIM SET STABLE via frozen P2.05 economics logic; numerical examples must be episode-verified if used. |
| A4-C08 | CLAIM SET STABLE with careful wording: visual/dimensional similarity alone is insufficient to establish claims that depend on other unrepresented attributes. |
| A4-C09 | CLAIM SET STABLE through P2.04/P2.06; strong numeric claims require source verification. |
| A4-C10 | CLAIM SET STABLE through configuration/genealogy backbone. |

## Source-vs-synthesis boundary

External sources support these premises:
- article/test pedigree matters;
- developmental evaluation differs from formal verification;
- production-representative evidence is important before production commitment;
- material/process/tolerance/surface/volume/rate influence manufacturing-process planning.

Repository synthesis remains:
- Prototype Evidence Transfer Matrix;
- Shortcut Expiration Card;
- REPRESENT 8;
- exact DEV/LVP/SVP transition logic;
- the specific twelve-dimension representativeness vector.

## Remaining work before EVIDENCE VERIFIED

1. Verify process-specific worked examples (3D-print → molded polymer, CNC → molding/casting, dev board → custom PCB) with authoritative process/electronics sources where the final script makes technical claims beyond obvious configuration differences.
2. Add one case study only if it improves narrative value without overcomplicating the episode.
3. Technical review across mechanical, electronics and NPI perspectives.
4. Package exact source-note excerpts/locations for final show notes.

## Status recommendation

`A4: RESEARCH PACK OPEN → CLAIM SET STABLE`
