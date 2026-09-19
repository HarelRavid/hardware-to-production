# EP12 Full Script Draft V1 — Polymer Parts: Injection Molding and the Alternatives

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 2 — How Hardware Is Actually Made
source_outline: EP12_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-06/
spoken_normative_standard_claims: NONE
universal_polymer_dfm_numbers: NONE

## Production note — not spoken

ISO public metadata/scope is used for moulded-part tolerances, shrinkage test context and moisture absorption. BASF data remain grade-specific examples. Autodesk Moldflow/Covestro/DuPont material is used as technical process guidance, not universal normative authority.

# SPOKEN SCRIPT

## Opening

A team machines a polymer enclosure.

It fits beautifully.

The sealing surface is flat.

The connector opening lands exactly where expected.

The prototype survives the tests.

Demand grows.

The team moves to injection moulding.

The first moulded parts arrive.

A wall has moved.

There is visible sink near a boss.

The enclosure has warped enough to change a sealing interface.

A line appears where two flow fronts met.

The first reaction is often:

“Something is wrong with the mould.”

Maybe.

But there is a more important lesson.

The CNC part and the moulded part were never the same manufacturing object.

They shared CAD geometry.

They did not share the same material history, flow, cooling, shrinkage, tooling or residual state.

That is what this episode is about.

**Polymer manufacturing is not simply copying geometry into plastic. The route helps create the final geometry and material state.**

---

## 1. “Plastic” is not a complete material definition

Start with the material.

“It's nylon.”

“It's ABS.”

“It's PBT.”

That is not enough for serious production engineering.

Exact grade matters.

Reinforcement.

Fillers.

Additives.

Viscosity or flow behaviour.

Conditioning state.

Moisture exposure.

Color package.

Flame-retardant package.

Material supplier.

Processing history.

As one concrete example, BASF publishes grade-specific data for a glass-fibre-reinforced PA6 showing different moulding shrinkage parallel and normal to flow.

The same grade family can also show different properties in dry and conditioned states.

The point is not the BASF number.

The point is:

**the exact compound and state belong in the product/process definition.**

---

## 2. Polymer parts have several very different manufacturing routes

Injection moulding is important.

It is not the only polymer route.

There is extrusion.

Blow moulding.

Thermoforming.

Rotational moulding.

Compression and transfer moulding.

Reactive moulding.

Machining.

Additive manufacturing.

Soft-tool or bridge routes.

Each process has a geometry that feels natural to it.

Extrusion naturally creates continuous sections.

Blow moulding is useful for hollow forms.

Thermoforming starts from sheet and stretches it.

Rotational moulding can create large hollow parts.

Compression or transfer routes can suit different thermoset or filled systems.

And machining or additive can remain perfectly rational for low-volume or changing designs.

Do not rank these by maturity.

Rank them against the product claim and production envelope.

---

## 3. Injection moulding creates the part through a process

For injection moulding, think in a simple chain.

Fill.

Pack.

Cool.

Eject.

The polymer flows through the runner and gate into the cavity.

The cavity fills.

Pressure and material feed compensate for shrinkage while the gate remains effective.

The part cools.

Material orientation and residual state develop.

The tool constrains the geometry until ejection.

Then the part continues toward its final dimensional state.

That is why process conditions and mould design matter.

ISO 294-1, even though it is a test-specimen preparation standard rather than a production DFM standard, makes an important point:

reproducible moulding requires controlled conditions, and the exact conditions depend on the material.

So when someone says:

“The CAD dimension is 50.00, why isn't the moulded part 50.00?”

the answer is:

because the mould and process are designed around how the material transforms.

---

## 4. Moulded tolerances are not machined-metal tolerances

This is now especially clear in the current ISO standard.

ISO 20457 was revised in August 2026.

The current edition explicitly addresses geometrical and dimensional tolerances for plastic moulded parts and explains that moulded plastics can show dimensional, form and location variation because of material behaviour, shrinkage, processing conditions, geometry, warpage and non-uniform cooling.

That matters because teams often bring a metal-design mindset into polymer production.

They tighten dimensions.

Then tighten more.

But a tolerance does not remove a process mechanism.

If warpage moves a feature, the engineering problem may be:

wall/geometry,

material,

orientation,

cooling,

gate strategy,

fixture/datum strategy,

or process capability.

The solution is not automatically another decimal place on the drawing.

---

## 5. Shrinkage is not one magic percentage

A familiar shortcut is:

“This resin shrinks one percent.”

Then every mould dimension is scaled.

Real moulding is more complicated.

ISO 294-4 explicitly distinguishes shrinkage parallel and normal to flow.

Filled materials can become strongly directional.

Different regions of the part can cool differently.

Packing effectiveness changes across geometry.

Humidity or post-mould conditioning can affect some materials later.

So a shrinkage data-sheet value can be a useful starting input.

It is not automatically the final dimensional model for a complex production part.

This is where simulation, supplier experience, tooling strategy and actual mould trials become important.

---

## 6. Warpage is the result of nonuniform shrinkage

Warpage is not a mysterious defect category.

At a useful engineering level, think about different parts of the component wanting to shrink differently.

Autodesk Moldflow separates major contributors such as:

differential cooling,

differential shrinkage,

material or fibre orientation,

and geometry-related effects.

If one side cools differently from the other, the final shape can move.

If fibre orientation changes material behaviour in different directions, the part can distort.

If wall thickness changes abruptly, local cooling and shrinkage behaviour can change.

The important message is:

**warpage is a coupled material–geometry–process problem.**

Do not assume one global correction factor will solve it.

---

## 7. Sink marks and voids tell you about local material compensation

Imagine a thick boss connected to a cosmetic outer wall.

The outer surface freezes.

The thicker local mass continues cooling and shrinking.

If the process cannot compensate that local volume effectively, the surface may pull inward.

That becomes a sink mark.

Or the outer skin may resist movement and a void forms internally.

Moldflow technical guidance connects this behaviour to local thick sections, volumetric shrinkage, packing effectiveness, gate freeze and cooling/process conditions.

The practical lesson is not a magic rib ratio.

It is:

**local geometry changes the thermal and packing problem.**

Design and tooling have to treat it that way.

---

## 8. Weld and meld lines are flow-history features

Now imagine the melt front reaches a hole.

It splits.

Flows around both sides.

Then meets again.

The meeting region creates a weld or meld line.

Multiple gates can do the same thing.

These features can be cosmetic.

They can also become structurally important depending on:

material,

fillers,

temperature,

pressure,

flow-front condition,

and location relative to load.

So the design question is not:

“Are weld lines bad?”

It is:

“Where will the flow fronts meet, and what does that location mean for this product?”

This is why gating belongs in product/process engineering—not only toolmaker detail.

---

## 9. Tooling decisions are product decisions

Gate location.

Runner architecture.

Cooling channels.

Venting.

Parting line.

Ejection.

Tool access.

Cavity arrangement.

These decisions affect what the process can produce.

Covestro and DuPont technical guidance both emphasize mould/gate/cooling/ejection design as important parts of moulded-part production.

You do not need the product designer to design the entire mould.

But the product team must understand which critical features depend on the tool architecture.

A gate moved after tooling can move a weld line.

A cooling imbalance can move the part.

An ejector strategy can leave marks or distort a weak region.

Tooling is not downstream purchasing.

It is part of the production architecture.

---

## 10. Moisture and conditioning are material-specific

Some polymers absorb meaningful moisture.

Some much less.

That moisture can affect dimensions and properties.

ISO 62 provides a controlled method for evaluating water absorption.

BASF material data show why this matters at the grade level: different polyamide/PPA grades can have very different water uptake and dimensional behaviour.

But do not take the next bad shortcut.

This does **not** mean:

“All plastics must be dried the same way.”

Or:

“All nylon needs the same moisture target.”

Processing and conditioning requirements belong to the exact material supplier/process specification and product claim.

Material-state control has to be scoped.

---

## 11. Simulation is powerful—and still not qualification

Mould-flow simulation can help predict:

fill pattern,

pressure,

shrinkage,

warpage,

orientation,

weld-line location,

cooling behaviour.

That can save enormous time and tooling rework.

But simulation is a model.

It depends on:

material characterization,

mesh,

boundary conditions,

machine/process assumptions,

tool design.

So use simulation to improve decisions.

Then validate the real tool/process/product against the actual CTQs.

Simulation is evidence.

It is not automatically the final production qualification.

---

## 12. When injection moulding is not the right route yet

Suppose the product design is changing every month.

Demand is uncertain.

You need 100 customer units.

Hard tooling would take months.

Machining may be more expensive per piece and still be the better business and engineering choice.

Or additive.

Or soft tooling.

Or another bridge process.

Wave 06A gave us the rule:

bridge manufacturing is legitimate when the limitations are explicit and the exit trigger is visible.

Ask:

When does cost become unacceptable?

When does lead time become the problem?

Which production behaviour is not represented?

When must the design change for the next process?

Do not switch because injection moulding feels more “real.”

Switch when the evidence and economics justify it.

---

## 13. The Polymer Route Review

Here is the listener tool.

Start with:

Function and exact material state.

Geometry.

Forming mechanism.

Tooling.

Expected defect and variation mechanisms.

Inspection.

Lifecycle stage and volume.

Economics.

Evidence.

Route decision.

Then run a Moldability and Bridge Review.

Which interfaces are shrink or warp sensitive?

Where can flow split and rejoin?

Which thick features create packing/cooling risk?

Which material-state variables matter?

What does your prototype route fail to represent?

Which tooling change would be expensive after release?

What makes the current bridge process expire?

That is a much stronger production conversation than:

“Can this part be injection molded?”

---

## 14. Six traps to avoid

“Plastic” defines the material.

Moulded dimensions should equal CNC dimensions.

One shrink factor works everywhere.

Tighter tolerances fix warpage.

Simulation equals qualification.

Injection moulding automatically wins above some generic commercial volume.

---

## 15. The action after this episode

Pick one polymer part that may change manufacturing route.

Write two columns.

Column one:

What has the current prototype already proven?

Column two:

Which mechanisms will appear or change in the proposed production route?

Flow?

Shrinkage?

Warpage?

Moisture state?

Weld line?

Tooling?

Cooling?

Ejection?

That second column is your production-validation backlog.

---

## Closing

EP12 showed that polymer processing creates part state.

Now we move to metals.

Where the route can change not only geometry but:

grain flow,

porosity,

residual stress,

heat-treatment state,

distortion,

and machinability.

Episode 13:

**Metal Parts — Casting, Forming or Machining?**

# End spoken script

## Draft source anchors — not spoken

- ISO 20457:2026 — current moulded-part tolerances/acceptance public scope.
- ISO 294-1:2017 — reproducible injection-moulding test conditions/material dependence.
- ISO 294-4:2018 — directional moulding shrinkage.
- ISO 62:2008 — water absorption.
- BASF exact-grade data — grade/state-specific shrinkage and conditioning examples.
- Autodesk Moldflow — warpage, sink/void and weld-line process guidance.
- Covestro / DuPont — gate/mould/process technical guidance.
- Wave 06A / Wave 03 — route/economics/bridge logic.
