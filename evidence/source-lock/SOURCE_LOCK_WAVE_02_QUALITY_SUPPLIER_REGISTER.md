# Source-Lock Wave 02 — Quality Chain + Supplier Approval Shared Source Register

status: SHARED SOURCE REGISTER LOCKED — DETAILED PROPRIETARY-METHOD CLAIMS REMAIN GATED
checked: 2026-09-19
scope: EP23 / EP24 / EP32 / EP39 / EP40
backbone: P2.03 Quality Chain + P2.06 Supplier Industrialization

## 1. Purpose

Lock the public/authoritative source layer shared by the quality-chain and supplier-approval episodes without pretending that protected AIAG manuals have been ingested.

Wave 02 publication rule:

`public identity/scope + open technical evidence → verified generic engineering claim`

`protected/manual-specific method detail → source located / publication-gated until licensed text is reviewed`

No AIAG/VDA/PPAP/MSA/Control Plan field, threshold, step, submission level or customer-specific requirement may be presented as exact normative content unless the relevant current manual/customer-specific source has been reviewed.

## 2. Current publication/status register

### W2-S01 — AIAG Quality Core Tools official overview
Owner: AIAG
Public source: https://www.aiag.org/expertise-areas/quality/quality-core-tools
Evidence class: V2/public industry-body scope; V1 only when exact manual requirement is separately verified.

Publicly supportable statements:
- AIAG groups APQP, Control Plan, PPAP, FMEA, MSA and SPC as Automotive Quality Core Tools.
- AIAG states most automotive manufacturers/suppliers require one or more Core Tools.
- Adoption outside automotive exists, but this does not make automotive customer-specific requirements universal.

Guardrail:
Do not infer exact method steps, acceptance limits or submission requirements from the overview page.

### W2-S02 — APQP 3rd Edition
Owner: AIAG
Current public identity checked: APQP-3, 3rd Edition
Published: Mar 2024
Source: https://www.aiag.org/training-and-resources/manuals/details/APQP-3

Publicly supportable statements:
- APQP 3rd Edition is the current listed AIAG APQP manual.
- AIAG describes it as addressing product-quality planning/new-product-launch work, including sourcing, change management, metrics, risk mitigation, gated management and traceability.

Guardrail:
Detailed phase deliverables/checklists remain manual-gated.

### W2-S03 — Control Plan 1st Edition
Owner: AIAG
Current public identity checked: standalone Control Plan, 1st Edition
Published: Mar 2024
Source family:
- https://www.aiag.org/expertise-areas/quality
- https://blog.aiag.org/our-presale-for-the-new-apqp-3rd-edition-and-standalone-control-plan-is-finally-here-1

Publicly supportable statements:
- Control Plan is now a standalone AIAG manual.
- AIAG publicly describes linkages to APQP and provides guidance for developing/using control plans.

Guardrail:
Exact fields, required phases, Safe Launch details and customer-specific mandates remain manual/customer-source gated.

### W2-S04 — AIAG & VDA SPC Manual, 1st Edition
Owner: AIAG + VDA
Published: Jul 2026
Product code: SPCAV-1
Public sources:
- https://www.aiag.org/about-aiag/newsroom/articles/2026/07/01/international-cooperation-for-higher-quality--vda-and-aiag-publish-joint-standard-for-statistical-process-control-in-the-automotive-industry
- AIAG manuals/catalog pages

Status finding:
The harmonized AIAG & VDA SPC Manual was released July 2026. The legacy AIAG SPC-3 page explicitly notes that a new edition was released in July 2026.

Publicly supportable statements:
- the new manual harmonizes AIAG/VDA SPC approaches;
- it addresses machine/process capability, production-equipment/process qualification and monitoring/control in automotive context;
- AIAG publicly links SPC with FMEA, Control Plan and MSA/VDA 5.

Guardrail:
Wave 02 does not quote proprietary formulas, chart rules, thresholds or acceptance criteria from the manual without licensed review.

### W2-S05 — PPAP
Owner: AIAG
Current public identity checked: PPAP-4, 4th Edition, 2nd Printing
AIAG public catalog date: Nov 2009
Sources:
- https://www.aiag.org/expertise-areas/quality/continuous-quality-improvement
- https://www.aiag.org/international/united-kingdom

Publicly supportable statement:
AIAG describes PPAP as the automotive production-part approval process intended to ensure engineering design/specification requirements are consistently met and to establish supplier understanding of processes used during actual production at production rates.

Guardrail:
Submission levels, required records, change-notification/resubmission triggers and customer-specific requirements are manual/customer-specific and remain gated.

### W2-S06 — MSA
Owner: AIAG
Current public identity checked: MSA-4, Version 4
Source: https://www.aiag.org/training-and-resources/manuals

Publicly supportable statement:
MSA remains a current AIAG Core Tool.

Guardrail:
No universal GR&R acceptance percentage or exact AIAG study rule enters the script without licensed manual/current customer applicability.

### W2-S07 — NIST Measurement Process Characterization
Owner: NIST/SEMATECH
Publication: Engineering Statistics Handbook, Chapter 2 — Measurement Process Characterization
Source: https://www.nist.gov/publications/nistsematech-engineering-statistics-handbook-chapter-2-measurement-process

Strong support:
- measurement processes have repeatability, reproducibility and stability behavior;
- measurement-process control and uncertainty characterization matter;
- calibration status alone is not a complete description of measurement-process adequacy.

Episode use:
EP24 primary open technical source; EP23/EP32 prerequisite support.

### W2-S08 — NIST repeatability/reproducibility terminology
Owner: NIST
Source: https://www.nist.gov/pml/nist-technical-note-1297/nist-tn-1297-appendix-d1-terminology

Strong support:
- repeatability concerns successive measurements under the same conditions;
- reproducibility concerns agreement under changed measurement conditions, which must be identified.

Episode use:
EP24 terminology support.

### W2-S09 — NIST measurement-system characterization/traceability
Owner: NIST
Source: https://www.nist.gov/publications/traceability-considerations-characterization-and-use-measuring-systems

Strong support:
Measuring systems may be characterized through calibration, adjustment, verification/testing, operating/influence conditions, resolution and repeatability; how a system is characterized influences later measurement results/claims.

Episode use:
EP24 claim that a calibration sticker does not by itself prove the full measurement method is decision-capable.

### W2-S10 — NIST process capability
Owner: NIST/SEMATECH
Sources:
- https://www.itl.nist.gov/div898/handbook/pmc/section1/pmc16.htm
- https://www.itl.nist.gov/div898/handbook/ppc/section4/ppc46.htm

Strong support:
- process capability compares process output/variation with engineering specification limits;
- NIST frames capability in relation to a stable/in-control process;
- Cp compares specification width with process spread.

Episode use:
EP32 core generic capability concepts and numerical worked example.

### W2-S11 — NIST MEP supply-chain management
Owner: NIST Manufacturing Extension Partnership
Source: https://www.nist.gov/mep/supply-chain

Strong support:
NIST MEP publicly frames supplier work around supplier evaluation/selection, total cost of ownership, supplier segmentation, supplier metrics/scorecards, quality-system development and supplier development.

Episode use:
EP39/EP40 generic supplier selection/performance/resilience layer.

Guardrail:
This does not create universal supplier change-notification, PPAP, FAI or dual-source qualification requirements.

### W2-S12 — IAQG 9102 First Article Inspection
Owner: IAQG
Current public family: 9102 Rev C resources/forms/guidance
Sources:
- https://iaqg.org/standard/9102-first-article-inspection-requirement/
- https://iaqg.org/standards/forms/
- https://scmh.iaqg.org/scmh-make/

Publicly supportable statements:
- 9102 standardizes FAI process/documentation for verification of aviation, space and defense product;
- IAQG states it can be used across supply-chain levels and may also be used in other sectors where standardized FAI is needed;
- IAQG currently publishes Rev C forms/guidance.

Applicability guardrail:
FAI is not a universal supplier-approval requirement for all hardware sectors. Contract/customer/sector applicability controls whether 9102 is required.

## 3. Shared Wave 02 engineering claims

### W2-C01 — Quality tools should connect risk to execution and evidence
Status: VERIFIED AS INTERNAL SYNTHESIS WITH OFFICIAL METHOD CONTEXT
Claim:
PFMEA/FMEA-style risk analysis, control planning, measurement adequacy and SPC/capability are most useful when linked as an engineering evidence chain rather than maintained as disconnected paperwork.

Support:
AIAG publicly groups the Core Tools and describes current APQP/Control Plan/SPC relationships; NIST supports the measurement/stability/capability technical links.

Boundary:
The repository's `Risk → Control → Measurement → Stability → Capability → Reaction` chain is our synthesis, not a quoted AIAG standard sequence.

### W2-C02 — Measurement adequacy precedes strong process conclusions
Status: VERIFIED
Claim:
Before treating observed production variation as process truth, the measurement method/system must be adequate for the decision.

Support:
NIST measurement-process characterization and traceability sources.

Boundary:
No universal GR&R percentage threshold is claimed.

### W2-C03 — Control limits and specification limits answer different questions
Status: VERIFIED
Claim:
Engineering specification limits define required product/process outcomes; statistical process-control limits describe expected process behavior under the chosen chart/model.

Support:
NIST/SEMATECH statistical handbook.

### W2-C04 — Stable does not automatically mean capable
Status: VERIFIED
Claim:
A process may be stable/in control and still be poorly positioned or too variable relative to specification limits.

Support:
NIST process-capability guidance.

### W2-C05 — Capability indices are conditional evidence
Status: VERIFIED
Claim:
A capability index is not decision-worthy merely because a formula can be calculated; measurement adequacy, process stability, data/model assumptions and sampling context matter.

Support:
NIST process-capability guidance + Wave 02 synthesis.

Boundary:
No universal Cpk threshold enters the generic podcast narrative.

### W2-C06 — FAI, PPAP-style approval and sustained capability are different evidence questions
Status: VERIFIED AS CROSS-SOURCE SYNTHESIS
Claim:
A first-article/configuration verification, an automotive production-part/process approval package, and evidence of sustained production capability answer different questions and should not be treated as synonyms.

Support:
IAQG 9102 public scope + AIAG PPAP public scope + NIST process-capability principles.

Boundary:
Exact mandatory contents/triggers depend on the governing standard/customer contract.

### W2-C07 — Approved supplier name is not permanent evidence
Status: VERIFIED AS BACKBONE SYNTHESIS
Claim:
Supplier approval is meaningful only inside the demonstrated product/process/source/configuration/rate evidence envelope; change can require impact assessment and renewed evidence.

Support:
P2.02 configuration/change invariant + AIAG PPAP/IAQG FAI method context + NIST supplier-development framing.

Boundary:
Exact notification/reapproval obligations are sector/customer-specific.

### W2-C08 — Supplier scorecards should not hide hard-stop evidence
Status: VERIFIED AS SYNTHESIS
Claim:
Quality, delivery, responsiveness, change discipline and capacity can be monitored as supplier-performance dimensions, but a blended score should not override an unresolved safety/regulatory/critical-quality hard stop.

Support:
NIST MEP supplier metrics/scorecard support + repository hard-stop invariant.

## 4. Episode mapping

EP23:
- owns risk-to-control translation;
- may use AIAG public Core Tool relationships;
- exact FMEA method/AP/RPN/Control Plan fields remain licensed-manual gated.

EP24:
- owns measurement-system adequacy;
- primary technical lock comes from NIST;
- AIAG MSA provides industry-method context only until detailed manual review.

EP32:
- owns stability/capability distinction and basic Cp/Cpk teaching;
- primary technical lock comes from NIST;
- 2026 AIAG/VDA SPC manual remains current automotive context, not the generic authority.

EP39:
- owns RFQ technical package and first-production approval evidence;
- FAI and PPAP are comparison examples with explicit applicability;
- no universal supplier approval package/sample count.

EP40:
- owns sustained supplier quality, change, alternate-source and resilience;
- NIST supports evaluation/metrics/TCO/supplier-development context;
- exact change-notification/dual-source/requalification requirements remain sector/customer specific.

## 5. Numerical gate

The Sentinel numerical examples remain pedagogical.
Before script use:
- independently recalculate Cp/Cpk examples;
- label all synthetic measurements as illustrative;
- do not present illustrative control limits as universal chart construction;
- do not attach AIAG acceptance thresholds unless licensed/current source and applicability are verified.

## 6. Wave 02 unresolved gates

1. Licensed AIAG & VDA FMEA handbook review before exact method steps/Action Priority/RPN language is presented as authoritative.
2. Licensed AIAG Control Plan 1st Edition review before exact field/phase requirements are narrated.
3. Licensed AIAG MSA 4th Edition review before any AIAG-specific study design or acceptance threshold is narrated.
4. Licensed AIAG & VDA SPC 1st Edition review before automotive-specific chart/rule/capability approval details are narrated.
5. Licensed/current PPAP source or customer-specific requirements before exact submission levels/change/resubmission rules are narrated.
6. Current contractual/sector source before any supplier-change notification, dual-source qualification or special-process flow-down is stated as mandatory.

These are not blockers for generic engineering scripts if the episodes remain within the verified open-source claims above.
