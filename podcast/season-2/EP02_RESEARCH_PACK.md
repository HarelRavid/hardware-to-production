# Episode 2 Research Pack — POC, Prototype, MVP and Production-Intent Hardware

status: CLAIM SET STABLE
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: founders, systems, NPI, manufacturing, quality, supply chain
lifecycle: DEV → LVP TRANSITION
entry_point: EARLY SEASON 2 / STANDALONE WITH SHORT RECAP
technical_depth: foundation-practitioner

## 1. Episode promise
Replace ambiguous build labels with an evidence-based way to describe what a hardware build actually demonstrates and what it still cannot support.

Canonical listener question:
> When someone says “POC,” “prototype,” “MVP” or “production-intent,” what should we actually ask before making the next engineering or manufacturing decision?

## 2. Navigation card
**You are here:** Working concept/prototype → maturity classification → production-intent gap closure.

**Best for:** teams debating whether a build is “ready,” planning the next prototype generation, or preparing supplier/NPI investment.

**Prerequisite:** none mandatory. Episode 1 recommended.

**You will leave with:** Build Evidence Card + Maturity Gap Review.

**Prototype shortcut:** build labels may remain informal if consequential decisions remain tied to explicit claims/evidence rather than the label.

**Shortcut expires when:** customer commitment, tooling, supplier transfer, qualification, production release, cost/rate planning or compliance decisions rely on the label as if it were proof.

**Next:** Episode 3 NPI ownership → Episode 4 Product vs Manufacturing Readiness → Episode 5 lifecycle gates.

## 3. Core thesis
POC, prototype, MVP and production-intent are useful communication labels but do not constitute universal evidence states.

The useful question is not “what do we call this build?” but:
> Which product/process claims can this exact build support, under what configuration and conditions, and which evidence gaps remain before the next decision?

## 4. Audience contract
### DEV takeaway
Use labels lightly; write down what the build is meant to learn or prove.

### Prototype shortcut
A POC may be ugly, manually supported and nonrepresentative if it answers the intended technical question quickly.

### Shortcut expiration
The label becomes insufficient when another team, supplier or customer assumes it implies evidence that was never demonstrated.

### LVP change
Production-intent builds increasingly represent bounded/released interfaces, components, materials, process assumptions, controlled test, configuration identity and repeatable execution.

### SVP evidence
Commercial serial release depends on demonstrated product/process/supplier/measurement/rate evidence, not on naming a build “PVT” or “production-intent.”

### Manufacturing-debt prevention
For every prototype generation, state what it proves, what it intentionally does not represent and what must change before the next stage.

### Listener action
Complete a Build Evidence Card for the current build before naming the next prototype generation.

## 5. Stable claim register
| ID | Claim | Class | Priority | Status | Publication note |
|---|---|---|---|---|---|
| EP02-C01 | POC/prototype/MVP/production-intent labels are context-dependent and do not by themselves define a universal evidence state. | V6 | P0 | SYNTHESIS STABLE | Never present internal labels as standards-defined phases. |
| EP02-C02 | Build maturity is multidimensional: function, interfaces, configuration, materials/components, process, supplier, test, reliability/compliance and economics can mature at different speeds. | V6 + P2.01 | P0 | BACKBONE-SUPPORTED / STABLE | Do not collapse into one score. |
| EP02-C03 | A POC may legitimately optimize learning speed over production representativeness. | V6 + A4 | P1 | BACKBONE-SUPPORTED / STABLE | Shortcut logic. |
| EP02-C04 | A production-intent claim should identify which attributes are actually representative and which remain bridge/TBD. | V6 + A4/A7 | P0 | BACKBONE-SUPPORTED / STABLE | Claim/evidence envelope. |
| EP02-C05 | One successful build cannot establish repeatable manufacturing capability. | V6 + Episode 1/P2.04 | P0 | BACKBONE-STABLE | Capability requires population/process evidence appropriate to claim. |
| EP02-C06 | Maturity labels cannot substitute for configuration identity or verification evidence. | V6 + A7/A8 | P0 | BACKBONE-STABLE | Critical handoff rule. |
| EP02-C07 | The next build should be selected to close consequential evidence gaps, not merely to look more finished. | V6 | P1 | SYNTHESIS STABLE | Editorial/action thesis. |
| EP02-C08 | Production-intent does not inherently require final mass-production tooling; a justified LVP/bridge route may be production-intent for a bounded claim/envelope. | V6 + P2.05 | P1 | BACKBONE-SUPPORTED / STABLE | Economics/applicability guardrail. |

Core claims: 8. Open P0 normative claims in conceptual core: 0. External readiness terminology remains evidence-verification work only if attributed to a named framework/industry.

## 6. Listener tool — Build Evidence Card
For every important build capture:
| Field | Question |
|---|---|
| Build ID/name | What exact build/configuration is this? |
| Primary objective | What must we learn/prove? |
| Product claims supported | Which claims have evidence? |
| Representativeness | geometry/material/process/supplier/configuration/test/environment/rate |
| Manual/temporary shortcuts | What remains non-production? |
| Verification evidence | Which tests/results support the claim? |
| Open failure mechanisms | What could still be hidden? |
| Production assumptions | Which process/supplier/tooling assumptions are provisional? |
| Expiration trigger | When does this build become insufficient evidence? |
| Next build objective | Which evidence gap must be closed next? |

## 7. Maturity Gap Review
Score each dimension `LEARNING / PARTIAL / REPRESENTATIVE / DEMONSTRATED FOR CLAIM`:
- requirements/interfaces;
- mechanical configuration;
- electronics/firmware configuration;
- materials/components;
- supplier/source;
- manufacturing process;
- assembly/joining;
- test/calibration;
- reliability/environment;
- compliance/safety applicability;
- traceability/configuration control;
- rate/capacity;
- cost/economics.

Do not average these into one readiness number. Use the pattern to choose the next evidence action.

## 8. Sentinel Node example
POC: sensor dev board + laptop logging + printed enclosure shell; objective is sensing/communication feasibility.

Integrated prototype: custom PCB candidate + integrated enclosure/interfaces + controlled firmware build; objective is interaction and thermal/power/interface learning.

Production-intent LVP candidate: bounded/released PCB/BOM/mechanical configuration + representative connector/source + intended assembly/programming/calibration/test method + serial identity + controlled deviations + production-intent route or justified bridge process.

The label is secondary; evidence gaps decide what the build can support.

## 9. Boundary with adjacent episodes
- Episode 1 owns the overall manufacturability evidence gap.
- Episode 2 owns build/evidence maturity language and prevents labels from becoming proof.
- Episode 3 owns the industrialization workstreams that close the gaps.
- Episode 4 owns the structured distinction between product readiness and manufacturing readiness.
- Episode 5 owns lifecycle/gate terminology and how evidence is reviewed at transitions.

## 10. Common failure modes
- “MVP” means market demo to one person and production-ready design to another.
- Prototype generation numbers become maturity claims without evidence.
- Cosmetic polish is mistaken for production intent.
- Final-looking enclosure hides dev-board electronics or engineering-only setup.
- Supplier/tooling money is committed because management believes a phase label proves readiness.
- Teams repeat prototypes without a defined evidence objective.

## 11. Applicability statement
This episode uses POC/prototype/MVP/production-intent as practical communication labels, not universal standard lifecycle definitions. Industry/customer programs may define formal phases/gates differently. Any externally attributed readiness level or phase definition must be verified and scoped before publication.

## 12. What this episode must NOT claim
- one universal definition exists for MVP/EVT/DVT/PVT;
- every prototype generation must become progressively more production-like in every dimension;
- production-intent means final tooling is mandatory;
- a maturity score can replace claim/evidence review;
- quantity produced proves maturity.

## 13. Evidence backlog after claim stabilization
Before EVIDENCE VERIFIED:
1. Add authoritative readiness/product-development sources only for terminology actually attributed externally.
2. Verify any industry/customer phase definition before quoting it.
3. Technical review: systems + NPI.
4. Preserve Episode 4/5 boundaries; do not duplicate their readiness/gate depth.

## 14. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: LOW
Quantitative burden: LOW
Backbone risk: LOW
Claim set: STABLE
Source verification: CONTROLLED BACKLOG

Next status target:
`CLAIM SET STABLE → EVIDENCE VERIFIED`
