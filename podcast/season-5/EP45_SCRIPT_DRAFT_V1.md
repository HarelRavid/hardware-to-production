# EP45 Full Script Draft V1 — Automation Qualification, OEE and Maintenance

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 5 — Automation, Data and the Connected Factory
source_outline: EP45_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-04/
spoken_normative_standard_claims: NONE
clause_level_safety_design: EXCLUDED

## Production note — not spoken

IEC 62381:2024 is used for public FAT/FIT/SAT/SIT scope. NIST open sources support OEE and maintenance. Safety standards are named only in an applicability map; no PL/SIL/guarding/electrical design instruction is given.

# SPOKEN SCRIPT

## Opening

The machine passes FAT.

At the integrator, it hits the quoted cycle time.

The sequence looks clean.

The software works.

Everyone signs the punch list.

Then the machine is installed on the production floor.

A sensor creates false faults.

A part jams.

Fixture cleaning takes longer than expected.

Changeovers interrupt production.

A recipe mismatch creates a restart.

Maintenance waits for a vendor technician.

The machine is fast when it runs.

The production system is not ready.

This is why equipment acceptance and production readiness are not the same claim.

EP45 asks:

**What evidence says an automated process is ready to sustain production—not just complete nominal cycles?**

And once we have the data, how should we use OEE without turning one percentage into a false diagnosis?

---

## 1. FAT, SAT and SIT answer bounded acceptance questions

IEC 62381:2024 defines structured acceptance layers for process-industry automation systems including FAT, FIT, SAT and SIT.

At a high level, these tests are used to demonstrate that an automation system meets the applicable specification in the relevant factory/site/integration context.

That is valuable.

But the important podcast boundary is:

A FAT pass does not automatically prove production capability.

A SAT pass does not automatically prove sustained accepted throughput.

The automation system may meet its specification and still need production evidence for:

Real material.

Real product variation.

Normal operators.

Quality.

Rate.

Recovery.

Maintenance.

So use acceptance layers for the questions they actually answer.

Do not promote the result into a stronger claim without evidence.

---

## 2. Define the release envelope

Before saying a cell is production ready, define the envelope.

Which product configuration?

Which machine/tooling revision?

Which robot/PLC/software/recipe version?

Which component/material range?

Which operators?

Which utilities?

Which environment?

Which inspection/test method?

Which production rate/product mix?

A machine is not “qualified forever.”

It is released inside a demonstrated envelope.

When the envelope changes, evaluate whether the evidence still applies.

That is our recurring evidence rule.

---

## 3. Representative operation is more than the good cycle

Nominal automatic operation is the easy test.

Production readiness needs the messy conditions too.

Expected part variation.

Tool wear.

Utilities.

Changeover.

Material replenishment.

Normal staffing.

Minor stops.

Recovery.

Test/rework.

The same rule from production validation applies here:

If engineers or vendor experts are required every hour, the machine may still be useful—but the evidence does not support a claim of normal autonomous production readiness.

Record the support.

Do not hide it.

---

## 4. OEE — the formula

For an equipment-centric process, NIST describes OEE as:

Availability × Performance × Quality.

Let's calculate the Sentinel semi-automatic insertion station.

Planned production time:

420 minutes.

Unplanned downtime:

42 minutes.

Operating time:

378 minutes.

Availability:

378 divided by 420 equals 90 percent.

Ideal cycle time:

45 seconds.

Total cycles:

470.

Operating time:

22,680 seconds.

Performance:

45 times 470 divided by 22,680.

Approximately 93.25 percent.

Good units:

451 out of 470.

Quality:

approximately 95.96 percent.

Multiply the three:

OEE is approximately 80.54 percent.

That number is useful.

But it is not the answer to:

What should we fix?

---

## 5. Same OEE, completely different problems

Now compare two cells.

Cell A:

Availability 82 percent.

Performance 99 percent.

Quality 99 percent.

OEE:

80.3682 percent.

Cell B:

Availability 99 percent.

Performance 99 percent.

Quality 82 percent.

OEE:

also 80.3682 percent.

Same composite value.

Opposite engineering problems.

Cell A has reliability and recovery loss.

Sensor faults.

Jams.

Long restart.

When it runs, process quality is excellent.

Cell B runs almost continuously.

At target speed.

But quality is poor.

Maybe fixture alignment.

Component variation.

Force window.

Measurement.

Making Cell A faster is the wrong first response.

Making Cell B more available is the wrong first response.

That is why OEE is a loss lens.

The decomposition tells you where to investigate.

The physical mechanism tells you what to change.

---

## 6. OEE is not system capacity

Another critical boundary.

Suppose we improve the insertion cell OEE.

Great.

But calibration remains the factory constraint.

Accepted system throughput does not increase.

Local OEE improved.

Business output did not.

This is exactly why EP29 owns capacity.

OEE tells us how a work unit loses productive potential.

It does not automatically tell us what limits the whole production system.

Do not optimize the prettiest OEE dashboard.

Optimize the system problem.

---

## 7. Fault and recovery qualification

Now move beyond metrics.

What faults should the cell survive or control?

Missing connector.

Wrong orientation.

Partial insertion.

Force signal outside window.

Sensor disagreement.

Loss of pneumatic pressure.

Communication loss.

Power interruption.

Wrong recipe.

Jam requiring access.

For each relevant abnormal state, ask:

Does the system go to the intended safe/controlled state?

Is the fault diagnosable?

Who can recover?

What product is suspect?

Does genealogy remain intact?

Does restart repeat, skip or bypass a quality step?

What proves the first good unit after restart?

How long does recovery take?

These are qualification questions too.

---

## 8. Maintenance belongs in the release case

Maintenance is not a document the OEM hands over after qualification.

It is part of the production architecture.

What wears?

What needs calibration?

Which spares have long lead times?

What requires specialist support?

Can the team restore software/configuration?

Does maintenance change a setting that affects quality?

Does replacing a sensor require verification?

NIST maintenance-economics research supports treating downtime and maintenance strategy as material manufacturing costs.

But do not turn that into:

Predictive maintenance is always best.

The strategy should fit the failure mechanism, consequence, data quality and economics.

---

## 9. Machinery safety is an applicability stack

A generic automation project can touch several safety-standard families.

ISO 12100 for machinery risk assessment/risk reduction principles.

ISO 13849 or IEC 62061 for safety-related control systems depending on design/applicability.

ISO 10218 for industrial robots and applications/cells.

IEC 60204-1 for machine electrical equipment.

But that list is not a universal compliance recipe.

Machine type.

Application.

Jurisdiction.

Regional adoption.

Other Type-B/Type-C standards.

Legal requirements.

All matter.

The episode-level engineering rule is simpler:

A robot component label is not the application safety case.

The integrated machine/application needs the appropriate risk assessment, safeguards, safety functions and verification for its actual use.

Detailed safety design belongs with competent machinery-safety engineering and current applicable standards.

---

## 10. Restart is not automatically recovery

A technician clears the jam.

Presses reset.

Machine runs.

Are we recovered?

Mechanically, perhaps.

But ask:

Correct recipe?

Correct calibration?

Correct product state?

Suspect WIP identified?

Test sequence completed?

Serial/result association intact?

Quality controls restored?

If a maintenance intervention can alter the evidence state, restart is not enough.

Recovery means returning to a trustworthy production state.

This is the same global invariant we will later reuse in OT/cyber recovery.

---

## 11. The Automation Production-Readiness Pack

Before release, capture:

Intended envelope.

Acceptance criteria.

FAT/SAT evidence as applicable.

Representative product/process run.

Quality/measurement evidence.

Accepted throughput.

Fault/recovery cases.

OEE/loss decomposition.

Maintenance plan.

Spares.

Calibration/verification.

Software/configuration backup.

Owner/escalation.

Release authority.

Change/requalification triggers.

That is much closer to production readiness than a certificate that says the machine completed one good cycle.

---

## 12. LOSS 8

When someone gives you OEE, ask:

Definitions consistent?

Dominant loss?

Physical mechanism?

Average hiding tail events?

Recovery owner?

Quality/rework attribution?

System effect?

Representative evidence?

That is LOSS 8.

The number starts the conversation.

It does not end it.

---

## 13. Five traps

FAT pass equals production ready.

OEE tells root cause.

85 percent OEE is universally world class.

Higher local OEE means higher factory throughput.

Predictive maintenance is always best.

All false or incomplete.

---

## 14. The action after this episode

Take the last month's OEE for one automated asset.

Do not try to improve the percentage.

Break the dominant loss into named events.

Sensor fault.

Jam.

Changeover.

Slow cycle.

False reject.

Rework.

Then assign physical mechanism and recovery owner.

That is the engineering program.

---

## Closing

EP45 gave us a qualified, maintainable automated cell.

Now leadership wants another one.

Then another.

The temptation is:

Clone the machine.

Double capacity.

But equipment can be identical while the process evidence is not.

EP46 asks:

**When is an automated process mature enough to replicate without multiplying defects and hidden instability?**

Scaling Without Automating Defects.

# End spoken script

## Draft source anchors — not spoken

- W4-S08 — IEC 62381:2024 public scope.
- W4-S11/S12 — NIST OEE formula and maintenance.
- W4-S01–S07 — safety applicability/current-status map only.
- Wave 03 — capacity/constraint.
- Wave 01/02 — recovery/configuration/quality.
