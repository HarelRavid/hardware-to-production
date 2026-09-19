# EP13 Full Script Draft V1 — Metal Parts: Casting, Forming or Machining?

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 2 — How Hardware Is Actually Made
source_outline: EP13_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-06/
spoken_normative_standard_claims: NONE
universal_metal_process_numbers: NONE

## Production note — not spoken

NIST, ISO public scope, AFS and Forging Industry Association sources support generic process-state and defect/mechanism claims. No alloy-specific allowables, porosity limits, bend rules, machining allowances or NDT acceptance levels are generalized.

# SPOKEN SCRIPT

## Opening

A structural bracket starts life as a machined billet.

The prototype works.

It survives the load test.

Geometry is stable.

Demand increases.

Now the team asks:

Should we keep machining it?

Cast it?

Forge it?

Form it from sheet?

Extrude a near-net section and finish-machine the critical faces?

At first, this looks like a cost question.

Then the engineering questions begin.

Will a casting introduce porosity?

Will forging change grain flow?

Will sheet forming spring back?

Will heat treatment distort the datums?

Will residual stress move the part when finish machining releases material?

Which route gives the right final material state?

That is the real decision.

**For metal parts, the manufacturing process can change not only geometry, but microstructure, residual stress, defect population and final properties.**

---

## 1. Alloy name is not enough

“6061 aluminum.”

“17-4 stainless.”

“4140 steel.”

Useful.

Still incomplete.

What condition?

Temper?

Heat treatment?

Wrought?

Cast?

Forged?

Cold worked?

Stress relieved?

Solution treated and aged?

The process history can change properties and dimensional behavior.

So for route selection, define:

alloy plus state plus process history.

Not just alloy name.

---

## 2. Machining is powerful—but it is not neutral

Machining gives excellent flexibility.

Especially during DEV and LVP.

No hard forming tool.

Fast design changes.

Good access to precision features.

But machining still creates a process state.

Tool forces.

Heat.

Residual stress.

Workholding.

Tool wear.

Surface condition.

And the machine's published positioning accuracy is not the same as finished-part accuracy.

ISO 230-2 deals with axis positioning accuracy and repeatability.

ISO 230-12 explicitly recognizes that finished test-piece error can have other contributors beyond machine geometric errors.

That is the important distinction.

A machine spec helps describe equipment.

It does not prove your actual feature capability.

---

## 3. Casting creates the part through solidification

Casting is not “pour metal into the CAD shape.”

The liquid metal has to fill the mould.

Transfer heat.

Solidify.

Feed contraction.

Manage gas and inclusions.

Develop microstructure.

NIST's current solidification work covers phenomena including flow, segregation, porosity and inclusions.

The final part is a product of those mechanisms.

That is why casting DFM includes much more than geometry.

---

## 4. Porosity is not one thing

Teams often say:

“The casting has porosity.”

But porosity can come from different mechanisms.

Gas.

Solidification shrinkage.

Entrapped air.

And the engineering consequence depends on:

location,

size,

distribution,

connectivity,

load path,

sealing requirement,

later machining.

The American Foundry Society explicitly distinguishes gas-related and shrinkage-porosity families.

A small internal pore in one noncritical region may be irrelevant.

Porosity intersecting a sealing face or highly loaded region may be unacceptable.

So do not ask:

“Is porosity allowed?”

Ask:

**What defect population can this product tolerate, where, and how will we detect it?**

---

## 5. Forging and forming shape the material too

Forging is interesting because material flow itself becomes part of the part architecture.

The Forging Industry Association's design guidance discusses how developed grain flow can significantly affect material properties, and how material, forging process and heat treatment need to be considered together.

That does not mean forged is always better.

It means route and material state are coupled.

A poorly chosen forging route can still have defects, distortion, excess machining, high tooling cost or inspection burden.

The point is to include grain/material flow in the decision.

---

## 6. Sheet metal does not always stay where the die puts it

Formed sheet wants to recover elastically after the load is removed.

That is springback.

NIST has an active research program specifically around predicting springback in formed sheet, especially as advanced alloys become harder to model with old empirical rules.

Springback depends on material response and strain history.

That means the tool shape and final part shape are not necessarily identical.

Again:

the process creates the geometry.

It does not merely copy it.

---

## 7. Residual stress can make dimensions move later

Imagine a part with locked-in residual stress.

Now remove material during finish machining.

The stress field changes.

The part moves.

NIST has directly studied distortion during machining caused by prior residual stresses in hybrid manufactured metals.

That study is not a universal number for every billet or casting.

But the mechanism is important.

Previous process history can affect later dimensional stability.

That is why sequence matters.

Sometimes critical datums should be finished after a thermal or forming step.

Sometimes stress relief is justified.

Sometimes additional stock is retained.

The exact choice is application-specific.

---

## 8. Near-net plus machining can be a powerful combination

Manufacturing routes do not have to be pure.

A forging can create the material flow and rough geometry.

Machining creates precise bearing faces.

A casting creates a complex housing.

Machining finishes sealing lands and threaded interfaces.

An extrusion creates a continuous section.

Machining adds local features.

This can reduce material removal while keeping precision where it matters.

But it is not automatically cheaper.

You add:

tooling,

qualification,

inspection,

secondary setup,

supply complexity.

So compare the full chain.

Not “forging piece price” against “machining piece price.”

---

## 9. Inspection burden belongs in the route decision

Different process routes create different evidence problems.

Casting may require attention to internal defects.

Forging may require material/process verification.

Heat treatment may require property evidence.

Machining may require dimensional and surface verification.

There is no universal NDT package.

The inspection method follows the defect mechanism and consequence.

That burden belongs in the route comparison before sourcing.

---

## 10. Supplier capability is route-specific

A foundry says:

“We cast this alloy every day.”

A forge says:

“We hold tight tolerances.”

A machine shop says:

“Our machine positions to a few microns.”

Useful starting information.

Not production approval.

Actual source capability depends on:

alloy state,

geometry,

size,

tooling,

process,

inspection,

production rate,

supplier control.

Generic process capability narrows the shortlist.

Representative supplier evidence closes the decision.

---

## 11. The Metal Route Matrix

Here is the listener tool.

Start with:

Load and function.

Exact alloy/state.

Geometry and section.

Candidate route family.

Expected defects and variation.

Heat-treatment/material-state changes.

Machining or finish allowance.

Inspection/NDT.

Volume and tooling.

Supplier evidence.

Then ask:

What route produces the most useful final material state with the lowest total risk and cost for this lifecycle stage?

That is much better than:

“Can we cast this?”

---

## 12. Sentinel-style example

A structural bracket begins as five-axis machined billet.

That is reasonable in DEV.

The design is moving.

The quantity is low.

Later, volume grows.

Three candidates remain:

continued machining,

forging plus finish machining,

casting plus finish machining.

The decision compares:

load path,

alloy/material state,

grain flow,

porosity risk,

distortion,

tooling,

inspection,

scrap,

supplier capability,

and economics.

No route wins because it sounds more “production.”

The route wins because the evidence envelope fits the product and business.

---

## 13. Six traps to avoid

Machining is the default safe production route.

Same alloy name means same final properties.

Casting porosity is one simple defect.

Forging is always stronger.

Machine positioning accuracy equals part capability.

A formed sheet part should match the die exactly.

---

## 14. The action after this episode

Take one metal part.

For each candidate route write:

Exact material state delivered.

Main defect mechanism.

Main dimensional risk.

Secondary operations.

Inspection burden.

What final feature still needs machining.

What evidence the supplier must demonstrate.

If two routes look equal on piece price but very different on those fields, the decision is not equal.

---

## Closing

EP13 showed that producing a metal part changes material state and geometry together.

Now parts have to become assemblies.

And the interface itself becomes a manufacturing process.

Heat.

Surface preparation.

Preload.

Filler.

Cure.

Inspection.

Serviceability.

Episode 14:

**Joining — Welding, Adhesives, Brazing, Soldering and Fasteners.**

# End spoken script

## Draft source anchors — not spoken

- NIST Solidification 2026 — casting/solidification/segregation/porosity context.
- American Foundry Society — gas/shrinkage casting-defect families.
- Forging Industry Association — grain-flow/material/process/heat-treatment coupling.
- NIST Springback / NCAL — sheet-forming/material-response context.
- ISO 230-2:2014 + Amd1:2016 — machine-axis positioning.
- ISO 230-12:2022 — finished test-piece accuracy contributors.
- NIST residual-stress machining study — downstream distortion mechanism example.
- Wave 06A / Wave 03 — route selection and economics.
