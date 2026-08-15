# Episode 9 Research Pack — Tolerance, GD&T/GPS and Variation: Why One Good Prototype Proves Little

status: RESEARCH PACK OPEN
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
Nominal CAD describes an intended geometry; production creates distributions. Tolerances and geometric specification should communicate the functional variation the product can accept and provide a basis for manufacturing and verification.

One successful prototype is evidence about that specific configuration/unit. It does not characterize the distribution of future parts, the measurement system or process capability.

## 4. Draft claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP09-C01 | Nominal dimensions alone are insufficient to communicate acceptable manufacturing variation for consequential interfaces/features. | P0 | BACKBONE-SUPPORTED |
| EP09-C02 | Tolerances should originate from functional/interface requirements and be reconciled with process and measurement capability. | P0 | BACKBONE-SUPPORTED |
| EP09-C03 | Datum/reference strategy affects how geometry is manufactured, assembled and verified; it should reflect functional intent where applicable. | P0 | SOURCE + BACKBONE VERIFICATION REQUIRED |
| EP09-C04 | Tolerance accumulation across multiple contributors can create assembly/performance failure even when individual parts satisfy their own limits. | P0 | ENGINEERING FOUNDATION / SOURCE MAP REQUIRED |
| EP09-C05 | One conforming or functional prototype cannot establish a future production distribution or process capability. | P0 | BACKBONE-STABLE |
| EP09-C06 | Measurement-system adequacy must be considered before interpreting observed variation or capability. | P0 | GLOBAL INVARIANT / P2.03 |
| EP09-C07 | Statistical/worst-case tolerance analysis answer different questions and require explicit assumptions; neither should be applied mechanically. | P1 | SOURCE/QUANT AUDIT REQUIRED |
| EP09-C08 | GD&T/GPS symbols and rules are standards-governed language; exact definitions and interpretation require the applicable standard/edition rather than podcast shorthand. | P0 | APPLICABILITY GUARDRAIL |

## 5. Functional Tolerance Chain
For a consequential interface record:
`Function/requirement → mating/related features → functional reference/datum concept → dimensional/geometric contributors → allowed functional envelope → manufacturing contributors → measurement method → analysis assumption → evidence → reaction if margin is insufficient`.

The tool is intended to expose the chain before teams simply tighten every drawing tolerance.

## 6. Variation Evidence Review
Ask:
1. What function fails when this dimension/geometry moves?
2. Which contributors combine at the functional interface?
3. Are we analyzing worst-case assembly, expected population behavior, or both?
4. What independence/distribution/centering assumptions are being made?
5. Is the manufacturing process capable of the proposed limits?
6. Can the measurement system resolve the relevant variation?
7. Does the datum/reference scheme represent how the product actually functions and is assembled/verified?
8. Are supplier drawings/inspection methods using the same specification language and edition?
9. What evidence do we have from populations rather than hero parts?
10. Would changing architecture create more margin than simply tightening tolerances?

## 7. Worked example — enclosure, PCB and connector alignment
A prototype enclosure, PCB and panel connector fit because three individual parts happened to align favorably. In production, hole location, board outline/fixture position, connector position, enclosure geometry and assembly clearance all vary.

A useful analysis begins from the functional condition — connector mates/seals/aligns without harmful load — then identifies contributors, reference scheme, allowable envelope, process/measurement evidence and analysis assumptions.

The lesson is not “use tighter tolerances.” It is to create adequate functional margin and a controllable specification/process/measurement system.

## 8. Quantitative teaching plan
This episode may include simple arithmetic examples, but every equation/example receives an arithmetic audit before publication.

Potential examples:
- simple one-dimensional worst-case stack;
- root-sum-square illustration with explicit independence/statistical assumptions;
- effect of centering/shift on available margin;
- measurement resolution versus tolerance illustration.

No universal capability threshold or tolerance ratio will be taught here without applicable source verification.

## 9. DEV/LVP/SVP lens
**DEV:** use nominal geometry rapidly but identify consequential interfaces and uncertainty.
**LVP:** release bounded specifications, measure real populations and compare process/measurement behavior to functional margin.
**SVP:** maintain specification, process capability, measurement, supplier and change evidence across production populations.

## 10. Standards/source boundary
Exact GD&T/GPS definitions, symbols, defaults, datum rules and interpretation are normative-standard territory. Candidate source families include ASME Y14.5 and ISO GPS standards, but exact editions/applicability must be verified before normative script content.

The podcast must not mix ASME and ISO rule sets casually or imply they are interchangeable.

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
- measurement data equal true process variation without MSA consideration;
- one universal capability threshold applies to every product/process/customer.

## 14. Research backlog before CLAIM SET STABLE
1. Map exact ASME Y14.5 / ISO GPS standards relevant to claims and verify editions available in our standards library.
2. Cross-check P2.03 metrology/capability backbone.
3. Build two arithmetic examples and independently audit them.
4. Separate normative symbol/rule teaching from conceptual tolerance-chain teaching.
5. Technical review: mechanical design/GD&T + manufacturing + metrology/quality.

## 15. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: HIGH
Quantitative burden: MEDIUM-HIGH
Backbone risk: LOW if standards boundary is enforced
Source verification: OPEN

Next status target: `RESEARCH PACK OPEN → CLAIM SET STABLE`
