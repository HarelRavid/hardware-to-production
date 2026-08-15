# Episode 9 Research Pack — Tolerance, GD&T/GPS and Variation: Why One Good Prototype Proves Little

status: CLAIM SET STABLE
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: mechanical, manufacturing, quality, metrology, NPI, suppliers
lifecycle: DEV → LVP → SVP
entry_point: VARIATION AND SPECIFICATION FOUNDATION
technical_depth: practitioner

## 1. Episode promise
Teach hardware teams to move from nominal geometry and one-good-part thinking toward functional specification, datum/reference strategy, tolerance accumulation, measurement and population variation.

Canonical listener question:
> If the prototype fits and works, what do tolerances, datums and process variation tell us about whether the next hundred or ten thousand units will still fit and work?

## 2. Navigation card
**You are here:** DFM/DFA/testability → specification and variation → reliability/service.
**Best for:** teams releasing drawings, debugging assembly variation, transferring parts to suppliers or preparing capability evidence.
**Prerequisite:** Episode 6 recommended; Episode 8 helpful.
**You will leave with:** Functional Tolerance Chain + Variation Evidence Review.
**Next:** Episode 10 Reliability/Service/Repair; later metrology/MSA/capability episodes deepen the statistics.

## 3. Core thesis
Nominal CAD describes intended geometry; production creates distributions. Tolerances and geometric specification communicate the allowable functional variation and provide a basis for manufacturing and verification.

One successful prototype is evidence about one realized configuration/unit. It does not establish the future production distribution, measurement capability or process capability.

## 4. Stable claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP09-C01 | Nominal dimensions alone are insufficient to communicate acceptable variation for consequential production interfaces/features. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP09-C02 | Tolerances should originate from functional/interface requirements and be reconciled with process and measurement capability. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP09-C03 | Datum/reference strategy affects how geometry is related for manufacture, assembly and verification; exact normative meaning depends on the invoked standard. | P0 | CONCEPT STABLE / NORMATIVE SOURCE GATED |
| EP09-C04 | Tolerance accumulation across multiple contributors can produce assembly/performance failure even when individual parts satisfy their own limits. | P0 | ENGINEERING FOUNDATION / STABLE |
| EP09-C05 | One conforming/functional prototype cannot establish a future production distribution or process capability. | P0 | BACKBONE-STABLE |
| EP09-C06 | Measurement-system adequacy must be considered before interpreting observed variation or capability. | P0 | GLOBAL INVARIANT / P2.03 / STABLE |
| EP09-C07 | Worst-case and statistical tolerance analyses answer different questions and require explicit assumptions. | P1 | CONCEPT STABLE / QUANT SOURCE GATED |
| EP09-C08 | GD&T/GPS symbols, defaults and rules are standards-governed language; exact interpretation requires the applicable standard/edition. | P0 | APPLICABILITY GUARDRAIL / STABLE |

Core claims: 8. Open P0 normative content: all exact ASME/ISO symbol/default/rule statements remain blocked until edition/source verification.

## 5. Functional Tolerance Chain
For a consequential interface record:
`Function/requirement → related features → functional reference/datum concept → dimensional/geometric contributors → allowed functional envelope → manufacturing contributors → measurement method → analysis assumption → evidence → reaction if margin is insufficient`.

The purpose is to expose the chain before teams tighten tolerances by reflex.

## 6. Variation Evidence Review
1. What function fails when this dimension/geometry moves?
2. Which contributors combine at the functional interface?
3. Are we analyzing allowable worst-case assembly, expected population behavior, or both?
4. What independence/distribution/centering assumptions are being made?
5. Can the intended process repeatedly achieve the proposed limits?
6. Can the measurement system resolve the relevant variation?
7. Does the reference/datum concept represent functional/assembly/verification intent?
8. Are supplier drawings/inspection methods using the same specification language and edition?
9. What population evidence exists beyond hero parts?
10. Would architecture create more robust margin than tighter tolerances?

## 7. Worked example — enclosure, PCB and connector alignment
A prototype enclosure, PCB and panel connector fit because the realized parts align favorably. In production, board location, connector placement, enclosure geometry, opening location and assembly positioning all vary.

Start with the functional condition — the connector must mate, align and seal without unacceptable load — then identify the contributors, reference scheme, allowable envelope, process/measurement evidence and analysis assumptions.

The lesson is not “use tighter tolerances.” It is to create adequate functional margin and a controllable specification/process/measurement system.

## 8. Quantitative teaching plan
The final episode may include:
- a simple one-dimensional worst-case stack;
- a root-sum-square illustration with explicit independence/statistical assumptions;
- a centering/shift example;
- a measurement-resolution-versus-tolerance illustration.

Every equation and unit must pass independent arithmetic audit before script use. No universal capability threshold or tolerance ratio is taught without scoped source verification.

## 9. DEV/LVP/SVP lens
**DEV:** use nominal geometry rapidly but identify consequential interfaces, assumptions and hand-fit behavior.
**LVP:** release bounded specifications, measure real populations and compare process/measurement behavior to functional margin.
**SVP:** maintain specification, capability, measurement, supplier and change evidence across production populations.

## 10. Standards/source boundary
Priority controlled sources include ASME Y14.5 and the relevant ISO GPS family (e.g. ISO 8015, ISO 1101, ISO 5459, ISO 14405 series, ISO 2692 where applicable). Exact editions, status and applicability must be verified before normative script content.

ASME Y14.5 and ISO GPS are not assumed to be interchangeable rule systems. The episode may compare them only after the exact rule being compared is sourced in both systems.

## 11. Boundary discipline
Episode 6 owns DFM/process-design fit. Episode 9 owns functional tolerance/variation thinking and standards-aware specification. Later metrology/MSA episodes own measurement-system depth; capability episodes own Cp/Cpk/Pp/Ppk and statistical process evidence.

## 12. Applicability statement
General hardware tolerance/variation foundation. Exact drawing/specification language is governed by the drawing's invoked standard, edition, company/customer rules and product context.

## 13. What this episode must NOT claim
- a good prototype proves the tolerance scheme is capable;
- tighter tolerances always improve quality;
- RSS is automatically valid for every stack;
- worst-case analysis predicts typical yield;
- GD&T and ISO GPS are interchangeable languages;
- measurement data equal true process variation without measurement-system consideration;
- one universal capability threshold applies to every product/process/customer.

## 14. Evidence backlog after claim stabilization
1. Verify exact ASME Y14.5 / ISO GPS editions and relevant clauses once standards are available.
2. Cross-check P2.03 metrology/capability backbone.
3. Build and independently audit two numerical stack examples.
4. Separate normative symbol/rule teaching from conceptual tolerance-chain teaching.
5. Technical review: mechanical design/GD&T + manufacturing + metrology/quality.

## 15. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: HIGH
Quantitative burden: MEDIUM-HIGH
Backbone risk: LOW if standards boundary is enforced
Claim set: STABLE
Source verification: CONTROLLED BACKLOG

Next status target: `CLAIM SET STABLE → EVIDENCE VERIFIED`
