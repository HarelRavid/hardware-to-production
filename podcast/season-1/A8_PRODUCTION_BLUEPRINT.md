# A8 Production Blueprint — Configuration Management from Prototype #1

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 1 — Build the Right Thing

## Listener transformation
Before: “We know roughly what changed between prototypes.”
After: “I can reconstruct what was built, tested, changed and reworked; bind evidence to a product configuration; and scope re-verification when change occurs.”

## Narrative hook
Two prototypes look identical. One passes, one fails. Weeks later the team discovers that one had a different connector lot, another firmware build and a hand rework nobody recorded. Without configuration identity, the failure cannot become knowledge.

## Teaching flow
### Segment 1 — Configuration management is product truth, not software tooling
Start with reconstructability. PLM/MES is optional in early DEV; identity and history are not.

### Segment 2 — Three distinct truths
Teach:
- **Definition:** what we intended to build;
- **As-built/as-programmed:** what this unit actually became;
- **Evidence:** what happened when it was tested/used.
They are different objects linked by traceability.

### Segment 3 — Minimum prototype identity
`Unit/build ID → mechanical rev → PCB/HW rev → BOM rev → FW/software build → configuration/calibration → critical supplier/material/lot → test procedure/result → deviations/rework`.

### Segment 4 — Rework adds history
A final PASS does not erase an original failure, modification or deviation. Show why this matters for root cause and later population analysis.

### Segment 5 — Change impact
Use the Change Impact Check:
`What changed → affected units/effectivity → dependent requirements/interfaces/CTQs → prior evidence dependencies → supplier/process/test impact → targeted re-verification → new configuration identity`.

### Segment 6 — Lightweight tools
Examples: spreadsheet + serial labels + Git commits + drawing/BOM revisions + controlled folders. Teach when these stop scaling and more formal tooling becomes justified.

### Segment 7 — Sentinel Node
Unit SN-DEV-07: enclosure Rev B, PCB A2, BOM A2.3, FW F-017, calibration C-04, connector lot L-118, environmental procedure TP-ENV-03, rework after initial fail. Show how later supplier change impacts only evidence that depends on connector behavior.

### Segment 8 — DEV→LVP→SVP horizon
DEV: minimal identities and visible change.
LVP: effectivity, supplier lots, deviations/rework, programming/calibration and controlled release become routine.
SVP: definition/as-built/genealogy/evidence support population segmentation, field learning and controlled change.

## Listener tools
### Minimum Prototype Configuration Record
One record per meaningful unit/build.

### Change Impact Check
Eight questions covering change, affected population, dependency and re-verification scope.

### Five-build reconstruction challenge
Ask the team to reconstruct the last five prototypes without asking the original builder. Every missing fact is configuration debt.

## Misconceptions to challenge
- “Version control is configuration management.”
- “CM means freezing the design.”
- “We are too small for revision control.”
- “Every change requires a full test campaign.”
- “A final passing configuration makes earlier failure history irrelevant.”
- “PLM software solves unclear ownership.”

## Standards/source backlog
NASA/government CM guidance and ISO 10007 where terminology is useful. Regulated/contractual CM rules stay application-specific.

## Season closing handoff
The listener can now move from an idea to a controlled engineering program. Season 2 begins with a working product and asks: **why is that still not enough to manufacture repeatedly?**
