# EP53 Case Evidence Pack — Hardware Launch Failures and What Was Missed

status: EVIDENCE PACK V1 — CASE SET SELECTED, CLAIM/CAUSAL REVIEW ACTIVE
season: Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
canonical_episode: EP53 — Hardware Launch Failures and What Was Missed
primary_mode: comparative case analysis
opened: 2026-09-08

## 1. Episode job

EP53 is the listener's transition from learning frameworks to applying them against documented reality.

It must answer:

> When a hardware launch or early scale-up fails, what category of evidence was missing, misunderstood, scoped too narrowly or acted on too late?

The episode must NOT imply that every failure has one root cause or that the Hardware-to-Production frameworks retrospectively “predict” every event.

Required separation for every case:

`DOCUMENTED FACT → SOURCE-SUPPORTED INTERPRETATION → OUR FRAMEWORK LESSON`

## 2. Selected case set

1. Samsung Galaxy Note7 — product/component failure + remedy population also failed.
2. Tesla Model 3 ramp — automation/process maturity + moving bottleneck + temporary bridge mode.
3. Boeing 737 MAX JATR — changed-product/system-integration assumptions and cumulative interaction.
4. Peloton Tread+ — field-signal aggregation and escalation/reporting timing.

The four cases intentionally exercise different failure classes.

## 3. Evidence-strength rule

- CPSC/FAA findings and regulatory records may support direct factual statements within their scope.
- SEC filings support what the company represented in the filing; do not convert risk-factor/management language into independent regulator causation findings.
- Samsung's root-cause conclusions remain attributed to Samsung and the independent organizations it cites.
- The Peloton settlement record includes CPSC staff charges and an explicit Peloton non-admission. The episode must preserve that distinction.

---

# CASE 53-01 — Samsung Galaxy Note7

## A. Case identity
- Product: Samsung Galaxy Note7 smartphone
- Lifecycle: launch / early field
- Primary lens: component/product evidence; corrective-action effectiveness
- Evidence sources: CPSC recall records + Samsung investigation/QA announcements

## B. Documented fact set

### F53-01-01 — initial U.S. recall
CPSC announced a recall on 15 September 2016 covering about 1 million Galaxy Note7 phones because the lithium-ion battery could overheat and catch fire.

Source:
https://www.cpsc.gov/Recalls/2016/Samsung-Recalls-Galaxy-Note7-Smartphones

Source locator:
Recall Details → Hazard / Units / Incidents-Injuries.

### F53-01-02 — replacement population was not a closed remedy
CPSC expanded the recall on 13 October 2016 to about 1.9 million phones and explicitly included replacement Note7 devices supplied under the first recall.

Source:
https://www.cpsc.gov/Recalls/2017/Samsung-Expands-Recall-of-Galaxy-Note7-Smartphones-Based-on-Additional-Incidents-with-Replacement-Phones

Source locator:
Recall Details → Units / Description / Incidents-Injuries.

### F53-01-03 — post-incident technical conclusion
On 23 January 2017 Samsung announced that its investigation and investigations by UL, Exponent and TÜV Rheinland concluded that batteries were the cause of the Note7 incidents.

Source:
https://news.samsung.com/global/samsung-electronics-announces-cause-of-galaxy-note7-incidents-in-press-conference

Attribution rule:
Say **“Samsung and the independent organizations presented by Samsung concluded…”**, not “CPSC proved…” unless a separate regulator source supports the exact mechanism.

### F53-01-04 — process/control response
Samsung announced an enhanced 8-Point Battery Safety Check and multi-layer safety measures after the incidents.

Source:
https://news.samsung.com/global/samsung-announces-new-and-enhanced-quality-assurance-measures-to-improve-product-safety

## C. Source-supported interpretation
The public record establishes that the first replacement action did not eliminate the field hazard across the replacement population because replacement Note7 devices were later included in the expanded recall.

This supports an **effectiveness-evidence** lesson without requiring speculation about internal decision-making.

## D. Framework lesson
- Corrective action is a new engineering state that requires evidence.
- Replacement/remediation does not inherit trust from the intent of the corrective action.
- Component evidence and product-level evidence must remain linked to configuration/population.
- FIELD EVENT → SIGNAL AGGREGATION → CONTAINMENT → EFFECTIVENESS EVIDENCE.

## E. What EP53 must NOT claim
- that one single battery-manufacturing defect explains every Note7 event unless the source supports that exact scope;
- that Samsung had no battery testing before launch;
- that all replacement batteries were defective;
- that CPSC made Samsung's later technical root-cause findings.

## F. Case readiness
FACT set: STRONG
Causal wording: ATTRIBUTED
Population/effectiveness lesson: STRONG
Episode use: FLAGSHIP

---

# CASE 53-02 — Tesla Model 3 production ramp

## A. Case identity
- Product: Tesla Model 3
- Lifecycle: production ramp
- Primary lens: automation maturity / bottleneck migration / controlled bridge production
- Evidence source: Tesla SEC Form 10-Q

## B. Documented fact set

### F53-02-01 — automation pace
Tesla's Form 10-Q for the quarter ended 31 March 2018 states that the company had added automation too quickly in certain Model 3 manufacturing processes.

### F53-02-02 — affected areas
The filing identifies challenges in portions of the battery-module line at Gigafactory 1, the materials-flow system and two general-assembly steps.

### F53-02-03 — temporary production-mode change
Tesla states that it temporarily reduced automation in these areas and introduced semi-automated or manual processes while working toward later full automation.

### F53-02-04 — moving constraint
Tesla states that the battery-module line had been its main production bottleneck for months and that after largely overcoming it the company planned downtime to address other known constraints.

### F53-02-05 — staged capacity decision
The filing states that after achieving the targeted 5,000/week rate Tesla intended to increase output on existing lines and then add incremental capacity in a capital-efficient manner.

Source for F53-02-01 through F53-02-05:
https://www.sec.gov/Archives/edgar/data/1318605/000156459018011086/tsla-10q_20180331.htm

Source locator:
Form 10-Q → manufacturing/Model 3 ramp discussion in Risk Factors / production-ramp narrative.

## C. Source-supported interpretation
Tesla itself documented a mismatch between the pace of automation introduction and the maturity/ramp behavior of selected processes, and it deliberately used less-automated modes while stabilizing them.

## D. Framework lesson
- “More automated” is not automatically “more mature.”
- A manual/semi-automated mode can be a legitimate MINIMUM CONTROLLED PRODUCTION MODE if risk, quality and rate remain controlled.
- Constraint ownership moves after a bottleneck is relieved.
- Sustainable accepted throughput matters more than one short peak-rate event.
- CapEx can be staged behind demonstrated rate/evidence rather than committed all at once.

## E. What EP53 must NOT claim
- that automation caused all Model 3 delays;
- that Tesla abandoned automation as a strategy;
- that manual assembly is inherently more reliable;
- that the specific Tesla response is universally optimal.

## F. Case readiness
FACT set: STRONG, company filing
Causal wording: COMPANY-ATTRIBUTED / scoped
Quantitative use: verify any rate/date numbers immediately before scripting
Episode use: FLAGSHIP

---

# CASE 53-03 — Boeing 737 MAX / Joint Authorities Technical Review

## A. Case identity
- Product: Boeing 737 MAX flight-control system certification context
- Lifecycle: changed product / certification / field failure aftermath
- Primary lens: cumulative change, system interaction, assumption evidence
- Evidence source: FAA-chartered Joint Authorities Technical Review

## B. Scope warning before facts
The JATR reviewed the type certification of the MAX flight-control system and related interfaces. It was not chartered to determine every cause of the two accidents or to review every aspect of the aircraft.

This scope statement must appear in the episode before drawing lessons.

## C. Documented fact set

### F53-03-01 — discrete change process vs integrated effects
The JATR found that the Changed Product Rule process was followed and was effective for discrete changes, but did not adequately address cumulative effects, system integration and human-factors issues.

Source:
https://www.faa.gov/sites/faa.gov/files/2021-08/Final_JATR_Submittal_to_FAA_Oct_2019.pdf

Locator:
Executive Summary, Changed Product Rule, roman page IV (PDF display page around 9–10).

### F53-03-02 — interaction assessment
The JATR stated that the process lacked adequate assessment of how proposed design changes integrate with existing systems and the impact of those interactions at aircraft level.

Same source/locator as F53-03-01.

### F53-03-03 — recommendation
JATR Recommendation R1 called for a top-down integrated whole-aircraft perspective for changed products and explicitly described the aircraft system as including aircraft/subsystems, flight crew and maintenance crew.

Same source/locator.

### F53-03-04 — assumptions
Elsewhere in the report, the JATR recommended that the FAA develop a practice of questioning applicant assumptions and found that certain assumptions about MAX/NG pilot experience and pilot response did not appear warranted.

Source locator:
JATR report → Recommendation R6.12 / Findings F6.12-A and F6.12-B.

## D. Source-supported interpretation
A formally compliant changed-product process can still leave a gap when evidence is organized around discrete changes but the consequential risk exists in cumulative/system interactions.

This is a direct bridge to the Hardware-to-Production **INTERACTION CLAIM** object.

## E. Framework lesson
- Change impact is not only “which part changed?” but “which interactions/evidence dependencies changed?”
- Inherited evidence is valid only inside its applicability envelope.
- Assumptions must be explicit evidence objects, especially when reused across generations/configurations.
- Interfaces include humans, maintenance and operating context when they materially affect system behavior.

## F. What EP53 must NOT claim
- that the Changed Product Rule itself was the sole cause of the accidents;
- that JATR found the certification process generally useless;
- that the aviation regulatory process transfers directly to ordinary industrial hardware;
- that every product revision requires complete requalification of everything.

## G. Case readiness
FACT set: STRONG
Primary-source locator: STRONG
Transfer boundary: HIGH IMPORTANCE
Episode use: FLAGSHIP

---

# CASE 53-04 — Peloton Tread+ field signal and escalation

## A. Case identity
- Product: Peloton Tread+ treadmill (TR01)
- Lifecycle: field / post-launch
- Primary lens: field-signal aggregation, reporting/escalation, recall containment
- Evidence sources: CPSC recall + CPSC/Peloton Settlement Agreement

## B. Legal-source handling rule
The Settlement Agreement contains **CPSC staff charges** and an explicit Peloton statement that the agreement is not an admission of those charges or of liability/violation.

Therefore the episode must distinguish:
- `CPSC STAFF CHARGED / AGREEMENT RECORDS`
from
- `PELOTON ADMISSION` — which the agreement explicitly says it is not.

## C. Documented fact set

### F53-04-01 — public recall facts
CPSC's May 5, 2021 recall states that one six-year-old child had died and that Peloton had received 72 reports of adult users, children, pets and/or objects being pulled under the rear of the Tread+, including 29 reports of child injuries.

Source:
https://www.cpsc.gov/Recalls/2021/Peloton-Recalls-Tread-Plus-Treadmills-After-One-Child-Died-and-More-than-70-Incidents-Reported

### F53-04-02 — signal accumulation in settlement record
The CPSC/Peloton Settlement Agreement staff-charges section states that by March 4, 2021 there were more than 150 reports of persons, pets and/or objects being pulled under the rear of the Tread+, including the child death and 13 injuries described there.

Source:
https://www.cpsc.gov/s3fs-public/PelotonInteractiveIncProvSettlementAgreementandOrder23C0001p.pdf

Locator:
Settlement Agreement paragraphs 10–14, printed page 5.

### F53-04-03 — reporting allegation and settlement qualification
Paragraphs 15–16 set out CPSC staff's failure-to-timely-report charges. Paragraphs 23–24 state that the agreement does not constitute an admission by Peloton and that Peloton does not admit violation of the CPSA or other law.

Same source.

### F53-04-04 — resulting compliance controls
The agreement later requires an enhanced compliance program including procedures for safety-claim/report review, prompt identification/quarantine/disposition of recalled goods, consolidated product information and effectiveness review/reporting.

Locator:
Settlement Agreement paragraphs 34–35.

## D. Source-supported interpretation
Independent of the disputed/legal-admission question, the record demonstrates why isolated field events must become a structured SIGNAL AGGREGATION system with defined escalation, containment and population identity.

## E. Framework lesson
- A complaint is not just customer service data when it can alter a safety/quality claim.
- Field events require structured aggregation across configuration/population/time.
- Containment requires both product identity and distribution-control mechanisms.
- Effectiveness evidence includes whether containment/recall controls actually prevent affected product from continuing to flow.

## F. What EP53 must NOT claim
- that Peloton admitted the CPSC staff charges;
- that every field complaint requires a recall;
- that the number of reports alone proves causation;
- that U.S. CPSA reporting rules apply to all hardware sectors/jurisdictions.

## G. Case readiness
FACT set: STRONG with legal qualification
Legal wording risk: HIGH — controlled
Episode use: SECONDARY / field-evidence close

---

# 4. Cross-case comparison matrix

| Case | Failure/evidence class | What was demonstrably weak/missing in the public record | Canonical object applied | Transfer boundary |
|---|---|---|---|---|
| Note7 | component/product + remedy | remedy population did not close hazard; later technical investigation traced incidents to batteries | EFFECTIVENESS EVIDENCE / FIELD EVIDENCE LOOP | consumer electronics; company root-cause attribution |
| Model 3 | ramp/automation | selected automation/process areas did not ramp as intended; manual/semi-auto bridge used | MINIMUM CONTROLLED PRODUCTION MODE / MOVING CONSTRAINT LOOP / STAGED CAPEX | company filing; not a universal automation prescription |
| 737 MAX JATR | cumulative change/system integration | discrete-change process did not adequately address cumulative/system/human-factor interaction | INTERACTION CLAIM / Claim-Evidence-Applicability / change impact | aviation certification-specific context |
| Tread+ | field signal / escalation | field reports accumulated; regulator record centers reporting/recall-control response | FIELD EVENT / SIGNAL AGGREGATION / containment/effectiveness | U.S. consumer-product legal context |

## 5. Episode-level synthesis claim candidates

### EP53-C01
A successful prototype, approved component, completed audit or passed discrete change can still leave an unsupported system-level claim if the consequential risk lies in an interaction outside the demonstrated evidence envelope.

Status: SUPPORTED BY CROSS-CASE SYNTHESIS; phrase as internal framework conclusion, not external law.

### EP53-C02
Corrective action creates a new evidence obligation: the remedy must be shown effective for the affected configuration/population rather than presumed effective from intent.

Status: STRONG, supported by Note7 and later Season 6 medical evidence; internal synthesis.

### EP53-C03
Temporary manual/semi-automated production can be rational during ramp when it is an explicitly controlled bridge used to restore sustainable production while the target automation matures.

Status: CONTEXT-BOUND; Tesla supports an example, not a universal rule.

### EP53-C04
Field reports become more decision-useful when they are aggregated with configuration, population, time and consequence rather than treated as unrelated anecdotes.

Status: STRONG framework synthesis; Peloton demonstrates the value of signal aggregation but does not by itself define the universal threshold for action.

## 6. Narrative order recommendation

1. **Cold open — Note7 replacement phone also recalled.**
   Hook: fixing the known failure is not the same as proving the fix.
2. **Tesla — scaling can expose a different failure class.**
   Shift from product defect to production-system maturity.
3. **737 MAX JATR — the deepest layer: interaction claims and inherited assumptions.**
   Show that even formal processes can be scoped around the wrong unit of analysis.
4. **Peloton — the factory is not the end of the evidence chain.**
   Close with field signal → containment → learning loop.
5. **Synthesis — four different failures, one discipline:** define the claim, evidence and applicability envelope; watch what changes and what the field invalidates.

## 7. Editorial guardrails

- Do not use tragedy as entertainment or a “gotcha.”
- Do not imply internal intent/motivation without source support.
- Do not use “root cause” for a multi-factor case unless the authoritative source uses it in that scope.
- Distinguish design failure, manufacturing/process failure, evidence escape, reporting/escalation and corrective-action failure.
- Never imply that one industry's regulator/standard is a universal hardware requirement.
- Do not produce a single “10 mistakes every launch makes” list; the purpose is to teach case reconstruction.

## 8. Evidence gaps before EP53 Production Blueprint

1. Capture source-level exact technical battery mechanism from Samsung/independent investigation if the script needs detail beyond “battery cause.”
2. Recheck Tesla rate/date numbers against the filing immediately before any quantitative narration.
3. Add exact JATR page/section locator for R6.12 assumptions if used verbally.
4. Decide whether Peloton remains a full fourth case or becomes a 3–5 minute closing case; protect legal wording either way.
5. Run technical/editorial review of all causal verbs.

## 9. Gate

Case selection: COMPLETE
Primary-source foundation: STRONG
Cross-case diversity: STRONG
Causal-language controls: DEFINED
Remaining source work: TARGETED

Current status:

**EP53 CASE EVIDENCE PACK V1: COMPLETE — NOT YET PRODUCTION BLUEPRINT READY**

Next gate:
`targeted source locators → causal-language audit → EP53 Production Blueprint`
