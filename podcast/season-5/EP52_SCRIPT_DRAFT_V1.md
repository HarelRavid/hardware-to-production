# EP52 Full Script Draft V1 — Manufacturing Data Engineers Can Actually Use

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 5 — Automation, Data and the Connected Factory
source_outline: EP52_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-05/
spoken_normative_standard_claims: NONE
legal_cybersecurity_claims: NONE

## Production note — not spoken

NIST SP 800-82 Rev.3 carries generic OT-security guidance. IEC 62443 public IEC pages support role/part boundaries only; no protected clause detail, security-level calculation or site topology is prescribed.

# SPOKEN SCRIPT

## Opening

A factory has a data lake.

Millions of machine samples.

Temperatures.
Pressures.
Cycle times.
Alarms.
Motor current.
Vision images.

The data science team wants to compare two failed units.

They find the serial numbers.

But the dataset does not include:

Recipe revision.
Fixture identity.
Calibration state.
Rework history.
Supplier lot.
Product configuration.

The factory has lots of data.

It does not yet have decision-grade engineering data.

Then a second problem appears.

To make analytics easier, a connector is installed directly into the production network.

Credentials are broad.

The connector can reach more assets than the analytics use case requires.

Now the data project is also an OT architecture project.

That is where Season 5 ends.

Connected data have to preserve engineering meaning and respect the physical consequences of OT connectivity.

## 1. Start from the engineering decision

Do not begin by collecting every tag.

Begin with the question.

Why did these units fail?

Is this process drifting?

Did Supplier Lot B create higher rework?

Did Recipe R17 change sealing behavior?

Which automation cell produces the defect?

Now ask what information the decision needs.

This reverses the normal data-lake mindset.

Data collection becomes evidence architecture.

Not storage ambition.

## 2. Minimum decision-grade context

For a serious manufacturing dataset, useful context can include:

Product and configuration.
Unit, lot or batch.
Operation.
Equipment and fixture.
Recipe or software configuration.
Parameter value with units and time.
Measurement-system context.
Quality result.
Rework or disposition.
Material or supplier.
Maintenance or change state.
Provenance.
Access/security context.
Retention and recovery.

Not every analysis requires every field.

The fields are driven by the causal/evidence question.

But if the variable that changed the outcome is missing, no amount of machine-learning sophistication can reconstruct it reliably afterward.

## 3. Derived features and AI outputs need lineage

Suppose a model outputs:

Anomaly score = 0.87.

What does that number mean later?

Which raw inputs?
Which time window?
Which model version?
Which feature code?
Which product configuration?
Which training/evaluation lineage?
Which threshold?

If an AI result influences an engineering or release decision, preserve enough provenance to understand the result later.

Derived data are not a replacement for raw evidence lineage.

They are another evidence layer.

## 4. OT changes the consequence model

NIST SP 800-82 Rev.3 is useful here because it treats OT differently from generic enterprise IT.

OT systems interact with the physical environment.

Security decisions have to account for performance, reliability and safety requirements.

A manufacturing data connector can therefore affect more than confidentiality.

Availability.
Integrity.
Timing.
Production safety.
Process state.
Quality evidence.

That is why connecting production systems is not just an API-permissions decision.

## 5. Read-only and write-back are different authority classes

A data path that observes process values is different from a path that can change a recipe, setpoint or command.

Write-back can alter physical production.

That creates a different authority and risk problem.

But do not make the opposite mistake:

Read-only means safe.

A read-only system can still consume network resources, use credentials, introduce vulnerable software, create remote-access paths, expose sensitive data or create availability issues.

So classify the direction and consequence.

Then design the access accordingly.

## 6. IEC 62443 is a family with distributed responsibilities

IEC 62443 is not one checklist owned by IT.

The public scope of the current parts makes role differences visible.

Part 2-1 addresses security-program requirements for IACS asset owners.

Part 2-4 addresses service providers involved in integration and maintenance.

Part 3-2 addresses system security risk assessment, including systems under consideration, zones and conduits.

Part 3-3 addresses system security requirements and security levels.

Part 4-1 addresses secure product development lifecycle requirements for product developers and maintainers.

Part 4-2 addresses technical security requirements for IACS components.

One organization can play more than one role.

The point is responsibility clarity.

Who owns the asset?
Who integrates?
Who maintains?
Who develops the product?
Who supplies the component?

Do not ask one standard part to solve somebody else's responsibility.

## 7. Zones and conduits are risk architecture, not a drawing template

IEC 62443-3-2 explicitly uses zones and conduits in system risk assessment.

That is a valuable concept.

Group assets/functions with similar security needs.
Understand communication paths.
Assess risk.
Define requirements.

But this does not mean every factory needs the same number of zones or the same firewall drawing.

The architecture follows the system under consideration and its risk.

So this podcast will not give you a universal OT topology.

It will give you a question:

Which assets trust each other, what is allowed to flow between them, and what happens to production if that path is compromised or unavailable?

## 8. RBAC is necessary and still not the whole problem

Application role-based access control can be good engineering.

Who may view?
Edit?
Approve?
Release?

But OT security also includes system architecture.

Network paths.
Device identity.
Remote access.
Monitoring.
Asset/configuration awareness.
Backup.
Patch/change processes.
Incident recovery.
Physical consequence.

RBAC inside the analytics app does not solve a flat OT network or uncontrolled write authority.

Security has layers.

## 9. Build the Secure Data Path Review

For every integration, write:

Asset.
Trust boundary.
Data direction.
Identity/credential.
Least necessary authority.
Segmentation or controlled path.
Monitoring.
Change ownership.
Backup.
Recovery.
Evidence impact.

Then ask:

What if the connection is unavailable?
Wrong?
Compromised?

What production decision fails?

What physical action becomes possible?

That is much more useful than saying:

This connector uses encryption.

Encryption can be valuable.

It is not the architecture.

## 10. Recovery means more than restarting the machine

Imagine a cyber or configuration incident.

Machines stop.

IT and OT teams restore controllers and servers.

Production starts again.

Are we recovered?

Maybe.

But ask:

Which recipes are loaded?
Which software versions?
Which work orders and WIP were active?
Were genealogy records lost?
Were quality statuses changed?
Did test results remain linked?
Were credentials/configuration altered?
Which product was produced during the uncertain period?

Our global recovery rule is:

Running again is not full manufacturing recovery until configuration, quality, WIP/genealogy and release evidence are trustworthy for the affected scope.

Not every incident invalidates every record.

Assess what could have been affected.

Contain that population.

Restore trust.

Then release.

## 11. NIST SP 800-82 is guidance, not one universal topology

NIST's OT-security guide describes typical architectures, threats, vulnerabilities and countermeasures while emphasizing OT safety, reliability and performance.

Use it as engineering guidance.

Not as:

NIST requires this exact network.

Different plants have different consequences, legacy constraints, technologies and operating models.

The common requirement is disciplined risk reasoning.

## 12. The Engineering Data Fitness Check

Before using a manufacturing dataset for an important decision, check:

Identity.
Configuration.
Context.
Units.
Timing.
Genealogy.
Provenance.
Completeness.
Measurement adequacy.
Decision consequence.

If the data fail one of those dimensions, decide whether the conclusion must be narrowed.

Do not simply add more rows.

## 13. The Secure Data Path Review

Now pair it with security:

Asset.
Trust boundary.
Direction.
Authority.
Remote access.
Segmentation.
Monitoring.
Change.
Backup.
Recovery.
Evidence impact.

Together, the two tools answer:

Can we trust what this dataset means?

And can we obtain/use it without creating an uncontrolled production pathway?

## 14. DEV to LVP to SVP

In DEV, CSV exports and scripts can be perfectly reasonable.

Keep identities and context.

Do not casually expose production control.

In LVP, stable identifiers, provenance and controlled interfaces become more important.

In SVP, governed pipelines, OT-aware security, monitoring and tested recovery become production infrastructure.

The tools grow with consequence.

## 15. Six traps to avoid

More data equals better evidence.

Read-only connector is safe by definition.

RBAC alone solves OT security.

IEC 62443 mandates one network topology.

Machine restart equals recovery.

AI features can replace raw evidence lineage.

## 16. The action after this episode

Choose one analytics, cloud or reporting path connected to production.

Draw the path.

What can move from OT outward?
What can move back?
Which identity or credential is used?
Which assets are reachable?
What production decision depends on the data?
What happens if the data are wrong?
What happens if the connector is compromised or unavailable?

That diagram is the start of an engineering-grade data architecture.

## Season closing

Season 5 began with automation and ends with information.

We learned not to automate instability.
We built the economic case.
Chose the right automation boundary.
Controlled automated inspection.
Qualified equipment.
Scaled it.
Defined systems of record.
Built genealogy.
Linked claims and evidence.
Created the Manufacturing Atlas.
Preserved semantics.
And finally connected manufacturing data without separating it from production risk.

Now Season 6 can do something different.

Apply the entire system to real cases and decisions.

# End spoken script

## Draft source anchors — not spoken

- W5-S08 — NIST SP 800-82 Rev.3.
- W5-S09–S14 — current IEC 62443 role/system/product/component public scopes.
- W5-S04/S05/S06 — digital-thread/provenance context.
- Wave 02 — measurement adequacy.
- Wave 01 — configuration/effectivity/recovery trust.
- IEC 62443-2-1 status requires publication recheck due IEC stability date 2026.