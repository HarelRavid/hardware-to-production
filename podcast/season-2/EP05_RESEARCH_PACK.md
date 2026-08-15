# Episode 5 Research Pack — EVT, DVT, PVT, Pilot and Ramp Without the Buzzwords

status: CLAIM SET STABLE
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: systems, NPI, manufacturing, quality, operations, program management
lifecycle: DEV → LVP → SVP
entry_point: LIFECYCLE/GATE TRANSLATION
technical_depth: foundation-practitioner

## 1. Episode promise
Explain common hardware phase labels without pretending they have one universal definition, and replace label-driven decisions with explicit evidence objectives and exit decisions.

Canonical listener question:
> What are EVT, DVT, PVT, pilot and ramp actually supposed to accomplish — and what if our company uses different names?

## 2. Navigation card
**You are here:** readiness evidence → lifecycle transitions → designing for production.
**Best for:** teams planning development/NPI, validation/pilot builds or translating customer/company phase terminology.
**Prerequisite:** Episode 4 recommended; standalone recap provided.
**You will leave with:** Phase Evidence Card + Gate Translation Table.
**Next:** Episode 6 DFM → Episode 7 DFA/mistake prevention → later pilot/ramp episodes.

## 3. Core thesis
EVT/DVT/PVT/pilot/ramp can be useful planning shorthand only when the team states what evidence each phase/build is intended to create and what decision follows. The labels themselves are not treated here as universal standards-defined gates.

## 4. Stable claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP05-C01 | EVT/DVT/PVT terminology must not be presented as universally defined across all hardware industries/companies without a scoped source. | P0 | APPLICABILITY GUARDRAIL / STABLE |
| EP05-C02 | A useful internal lifecycle gate states purpose, entry context, evidence objective and resulting decision. | P0 | SYNTHESIS/BACKBONE STABLE |
| EP05-C03 | Phase labels cannot substitute for configuration identity, representativeness or verification evidence. | P0 | BACKBONE-STABLE |
| EP05-C04 | Product and manufacturing evidence can mature in parallel rather than through a perfectly sequential handoff. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP05-C05 | A pilot should be designed to generate production-system evidence, not treated merely as a quantity milestone. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP05-C06 | Ramp introduces population, rate, variation and recovery questions a small pilot may not expose. | P1 | BACKBONE-SUPPORTED / STABLE |
| EP05-C07 | A phase/build may repeat or split when evidence gaps remain; build count alone does not advance maturity. | P1 | SYNTHESIS STABLE |
| EP05-C08 | Customer, regulatory or industry programs may define mandatory gates/evidence that govern their applicable scope. | P0 | APPLICABILITY GUARDRAIL / STABLE |

Important publication rule: any specific external definition of EVT, DVT, PVT, pilot or ramp remains `SOURCE VERIFICATION REQUIRED` until tied to a named source and applicability context.

## 5. Phase Evidence Card
For any named phase/build record:
| Field | Question |
|---|---|
| Local phase name | What does our team/customer call it? |
| Decision after phase | What commitment follows? |
| Entry assumptions | What must already be true? |
| Product evidence objective | What product claims must mature? |
| Manufacturing evidence objective | What process/supplier/test/rate claims must mature? |
| Configuration | Which design/process state is exercised? |
| Representativeness | What is production-intent and what remains bridge? |
| Population/quantity rationale | Why this many units? |
| Failure/learning capture | How are defects/rework/deviations preserved? |
| Exit evidence | What evidence permits the next decision? |
| Carryover gaps | What may remain open and why? |

## 6. Gate Translation Table
Translate labels by purpose rather than literally:
- **Engineering feasibility / architecture learning** — does the architecture work and where are major technical risks?
- **Design verification / production-intent product evidence** — does a bounded configuration meet relevant requirements under representative conditions?
- **Production-system validation / pilot evidence** — can intended suppliers/processes/tools/test/people repeatedly execute and expose variation?
- **Ramp evidence** — can accepted output increase while yield, quality, recovery, traceability and economics remain controlled?
- **Serial/commercial operation** — can the released product/process/supplier system sustain its required envelope and controlled changes over time?

A company may call these EVT/DVT/PVT/pilot/ramp or something entirely different.

## 7. Pilot as an experiment
Define in advance: process/supplier/tooling assumptions under test; CTQs/measurement; yield/rework/defect capture; permitted manual intervention; rate/capacity learning validity; change/effectivity rules; and the evidence that closes the decision.

## 8. Sentinel Node example
A team calls Build 3 “DVT.” The evidence card shows a bounded PCB/FW configuration, bridge enclosure process, representative connector source, environmental verification planned, prototype calibration station, nonfinal assembly fixture and no demonstrated supplier/process capability.

Conclusion: the build may support selected design-verification claims, but the label cannot establish production-system readiness for ramp.

## 9. DEV/LVP/SVP lens
**DEV:** organize learning without treating every experiment as release evidence.
**LVP:** connect product verification with controlled supplier/process/test/traceability learning.
**SVP/ramp:** emphasize accepted throughput, population variation, capability, recovery, economics and controlled change while preserving product evidence.

## 10. Boundary discipline
Episode 2 owns build maturity labels/evidence. Episode 4 owns readiness dimensions. Episode 5 owns lifecycle/gate translation. Detailed pilot execution, capability and ramp economics remain in later dedicated episodes.

## 11. Applicability statement
Phase names are contextual. Where a customer, regulator, industry manual or quality system defines formal lifecycle gates, that definition governs its scope. The Gate Translation Table is an internal explanatory framework.

## 12. What this episode must NOT claim
- EVT/DVT/PVT have one universal definition;
- every company must run exactly three validation phases;
- a fixed unit count defines pilot/PVT success;
- finishing a phase means all gaps are closed;
- pilot quantity proves capability;
- ramp is merely increasing machine speed.

## 13. Evidence backlog after claim stabilization
1. Collect authoritative examples of lifecycle terminology only as scoped examples.
2. Verify any named customer/industry phase definition before publication.
3. Technical review: systems + NPI/manufacturing + program perspective.
4. Preserve later pilot/ramp episode boundaries.

## 14. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: MEDIUM
Quantitative burden: LOW
Backbone risk: LOW
Claim set: STABLE
Source verification: CONTROLLED BACKLOG

Next status target: `CLAIM SET STABLE → EVIDENCE VERIFIED`
