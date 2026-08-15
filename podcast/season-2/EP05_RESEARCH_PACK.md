# Episode 5 Research Pack — EVT, DVT, PVT, Pilot and Ramp Without the Buzzwords

status: RESEARCH PACK OPEN
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: systems, NPI, manufacturing, quality, operations, program management
lifecycle: DEV → LVP → SVP
entry_point: LIFECYCLE/GATE TRANSLATION
technical_depth: foundation-practitioner

## 1. Episode promise
Explain common hardware phase labels without pretending they have one universal definition, and teach teams to replace label-driven decisions with explicit entry questions, evidence objectives and exit decisions.

Canonical listener question:
> What are EVT, DVT, PVT, pilot and ramp actually supposed to accomplish — and what should we do when our industry or company uses different names?

## 2. Navigation card
**You are here:** readiness evidence → lifecycle transitions → designing for production.

**Best for:** teams building a development/NPI plan, preparing design-validation/pilot builds or translating customer/company phase terminology.

**Prerequisite:** Episode 4 recommended; standalone recap provided.

**You will leave with:** Phase Evidence Card + Gate Translation Table.

**Next:** Episode 6 DFM → Episode 7 DFA/mistake prevention → later pilot/ramp episodes.

## 3. Core thesis
EVT/DVT/PVT/pilot/ramp are useful planning language only when the team states what evidence each phase/build is intended to create and what decision follows.

Different companies and industries use these labels differently. The podcast therefore treats them as common shorthand, not standards-defined universal gates.

## 4. Draft claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP05-C01 | EVT/DVT/PVT terminology is not universally defined across all hardware industries and companies. | P0 | SOURCE VERIFICATION REQUIRED BEFORE EXTERNAL ATTRIBUTION |
| EP05-C02 | A useful lifecycle gate has an explicit purpose, entry context, evidence objective and exit/decision. | P0 | SYNTHESIS/BACKBONE |
| EP05-C03 | Phase labels should not substitute for configuration identity, representativeness or verification evidence. | P0 | BACKBONE-STABLE |
| EP05-C04 | Product and manufacturing evidence often mature in parallel rather than in a perfectly sequential handoff. | P0 | BACKBONE-SUPPORTED |
| EP05-C05 | Pilot builds should be designed as evidence-generating production-system experiments, not merely quantity milestones. | P0 | BACKBONE-SUPPORTED |
| EP05-C06 | Ramp introduces population/rate/variation/recovery questions that a small pilot may not expose. | P1 | BACKBONE-SUPPORTED |
| EP05-C07 | A phase may legitimately repeat or split when evidence gaps remain; build count alone does not advance maturity. | P1 | SYNTHESIS |
| EP05-C08 | Customer/regulated programs may define mandatory gates/evidence that override generic podcast terminology. | P0 | APPLICABILITY GUARDRAIL |

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
Instead of translating labels literally, translate them by purpose:

- **Engineering feasibility / architecture learning** — does the chosen architecture work and where are major technical risks?
- **Design verification / production-intent product evidence** — does a bounded product configuration meet relevant requirements under representative conditions?
- **Production-system validation / pilot evidence** — can intended suppliers/processes/tools/test/people repeatedly execute and reveal variation?
- **Ramp evidence** — can accepted output increase while yield, quality, recovery, traceability and economics remain controlled?
- **Serial/commercial operation** — can the released product/process/supplier system sustain its required envelope and changes over time?

A company may call these EVT/DVT/PVT/pilot/ramp or use entirely different names.

## 7. Pilot as an experiment
A useful pilot asks in advance:
- what process/supplier/tooling assumptions are being tested;
- which CTQs and measurement systems matter;
- what yield/rework/defect data must be captured;
- which manual interventions are allowed and how they are recorded;
- what rate/capacity learning is valid at this scale;
- which changes are permitted during the build and how effectivity is controlled;
- what evidence closes the pilot decision.

## 8. Worked example — Sentinel Node
A team calls Build 3 “DVT.” The label is not enough.

Evidence card shows:
- final-ish PCB and firmware configuration;
- bridge enclosure process;
- representative connector source;
- environmental verification planned;
- production calibration station still prototype;
- assembly fixture not final;
- supplier/process capability not demonstrated.

Conclusion: the build may be appropriate for selected design-verification claims, but it is not automatically evidence that the production system is ready for ramp.

## 9. DEV/LVP/SVP lens
### DEV
Use phases to organize learning without pretending every experiment is release evidence.

### LVP
Use controlled builds to connect product verification with supplier/process/test/traceability learning.

### SVP/ramp
Shift focus toward accepted throughput, population variation, capability, recovery, economics and controlled change while maintaining product evidence.

## 10. Applicability statement
Phase names are contextual. Where a customer, regulator, industry manual or quality system defines formal lifecycle gates, that definition governs its scope. The podcast's Gate Translation Table is an internal explanatory framework.

## 11. What this episode must NOT claim
- EVT/DVT/PVT have one universal definition;
- every company must run exactly three validation phases;
- a fixed unit count defines pilot or PVT success;
- finishing a phase means all gaps are closed;
- pilot quantity proves capability;
- ramp is merely increasing machine speed.

## 12. Research backlog before CLAIM SET STABLE
1. Gather authoritative examples of lifecycle terminology from multiple contexts without universalizing them.
2. Cross-check Episode 4 readiness and later pilot/ramp content.
3. Verify any named customer/industry phase definition before use.
4. Technical review: systems/NPI/manufacturing/program perspective.

## 13. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: MEDIUM because terminology is often misattributed
Quantitative burden: LOW
Backbone risk: LOW
Source verification: OPEN

Next status target:
`RESEARCH PACK OPEN → CLAIM SET STABLE`
