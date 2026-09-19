# EP11 Full Script Draft V1 — How to Select a Manufacturing Process

status: FULL SCRIPT DRAFT V1 — SCRIPT REVIEW NEXT
season: Season 2 — How Hardware Is Actually Made
source_outline: EP11_SCRIPT_OUTLINE_V1.md
source_lock: evidence/source-lock/wave-06/
spoken_normative_standard_claims: NONE
process_specific_numeric_rules: NONE

## Production note — not spoken

NIST conceptual process-planning/material-selection work supports the generic decision architecture. Process-specific limits are deliberately deferred to EP12–18.

# SPOKEN SCRIPT

## Opening

A team builds a beautiful CNC-machined polymer enclosure.

It fits.

It seals.

It survives the prototype tests.

Demand starts to grow.

Someone says:

“Great. Now we injection mold it. Same part, lower cost.”

A tool is ordered.

The first molded parts arrive.

One wall sinks.

The enclosure warps.

A connector opening moves.

A sealing interface behaves differently.

The CAD is almost the same.

The manufacturing state is not.

The mistake happened before tooling.

The team never actually selected a production process.

It selected a process name.

That is what this episode fixes.

By the end, I want you to be able to compare manufacturing routes as engineering alternatives—not as categories like prototype process and production process.

---

## 1. Manufacturing-process selection begins before the drawing is finished

NIST process-planning research makes a simple point:

Manufacturability and manufacturing cost are affected by decisions made during specification and design.

That means process planning is not something manufacturing does after engineering is “done.”

The design constrains processes.

The process constrains design.

Those two decisions evolve together.

If you discover the production route only after every geometry, datum, material and interface is frozen, the manufacturing team may be left optimizing inside a very small box.

So process selection starts early.

Not with final commitment.

With candidates.

---

## 2. Material and process are coupled

Teams often ask:

“What material should we use?”

Then later:

“How should we manufacture it?”

But NIST material/process-selection research treats those as coupled decisions.

Why?

Because process choice changes which material states and forms are practical.

And material choice changes which processes are feasible.

Aluminum billet.

Casting alloy.

Forging stock.

Thermoplastic resin.

Elastomer.

Prepreg.

Powder.

Same broad material family can behave very differently depending on form and process history.

So the question is not simply:

Which material?

It is:

**Which material-state and manufacturing-route combination satisfies the product claim?**

---

## 3. Geometry alone does not select the process

A part may be printable.

Machinable.

Moldable.

Castable.

Formable.

That tells you feasibility.

Not necessarily the best route.

Now add:

Function.

Loads.

Environment.

Material state.

Tolerance.

Surface.

Sealing.

Assembly.

Inspection.

Volume.

Rate.

Tooling.

Lead time.

Design-change frequency.

Supplier maturity.

Yield.

Secondary operations.

Cost per accepted product.

Suddenly process selection becomes multi-attribute.

That is exactly what NIST process-selection work found decades ago:

early requirements are uncertain, and alternatives must be considered across multiple factors.

The answer is rarely hidden in one geometry rule.

---

## 4. Early uncertainty is allowed

At concept stage, you may not know annual demand.

Maybe the range is:

500 to 5,000.

You may not know final tolerance.

Maybe the requirement is still being characterized.

You may not know whether sealing is customer-critical.

That does not mean process selection must wait.

Create candidate routes.

Use ranges.

Mark assumptions.

Ask what uncertainty changes the ranking.

Maybe machining wins below one scenario.

Maybe molding becomes attractive if demand and geometry stabilize.

Maybe additive is valuable because tooling avoidance matters more than nominal unit cost.

The point is not to predict perfectly.

The point is to identify which unknowns drive the manufacturing decision.

---

## 5. Compare routes, not primary operations

Suppose Route A is machining.

Route B is molding.

The wrong comparison is:

machining quote versus molded piece price.

A real route may include:

Material procurement.

Primary processing.

Heat treatment or conditioning.

Secondary machining.

Cleaning.

Surface treatment.

Inspection.

Assembly.

Test.

Rework.

Packaging.

Tooling.

Qualification.

Supplier management.

A lower primary-operation quote can lose once the chain is included.

So define the system boundary before comparing economics.

This connects directly to Wave 03:

Cost per good unit.

Capacity.

Yield.

Maintenance.

Change.

Time.

Uncertainty.

The economic model is downstream of the manufacturing evidence.

---

## 6. Process-family capability is not supplier capability

You read:

Injection molding can hold X.

Machining can hold Y.

Additive can achieve Z.

Those statements can be useful starting points.

They are not supplier-release evidence.

Real source capability depends on:

Material.

Geometry.

Machine.

Tooling.

Fixture.

Process window.

Measurement.

Operator.

Maintenance.

Supplier system.

So use generic capability to shortlist.

Use demonstrated source capability to approve.

That distinction prevents an enormous amount of bad sourcing.

---

## 7. Prototype success transfers selectively

Back to our CNC polymer enclosure.

What did CNC prove?

Maybe:

Overall packaging.

Mounting interfaces.

Assembly access.

A sealing geometry under the machined material state.

Functional fit.

What did it not prove?

Mold filling.

Shrink distribution.

Warpage.

Gate/weld-line effects.

Ejection.

Molded residual stress.

Production-tool variation.

The old evidence is not useless.

It is bounded.

When the route changes, ask characteristic by characteristic:

Which evidence still transfers?

Which mechanism changed?

That is a much stronger rule than:

“Prototype test passed, so production should pass too.”

---

## 8. Bridge manufacturing can be the correct route

Not every team should rush to the eventual high-volume process.

Imagine:

Design is still changing.

Demand is uncertain.

Tool lead time is long.

But customers need 100 units.

A bridge route can be rational.

Machining.

Soft tooling.

Additive.

Urethane casting.

Manual or semi-manual assembly.

Whatever fits the product.

The important thing is to define the expiration trigger.

When does the bridge become too expensive?

Too slow?

Too variable?

Too supplier dependent?

When does it stop representing the required product behavior?

When does redesign for the next process need to begin?

Bridge manufacturing is not immature manufacturing.

Invisible bridge expiration is manufacturing debt.

---

## 9. “High volume” does not select the winner by itself

People love rules like:

“At 10,000 units, molding wins.”

Maybe for one part.

One tool.

One material.

One labor market.

One forecast.

The threshold can change dramatically with:

Tooling cost.

Part size.

Cavity count.

Cycle time.

Yield.

Secondary operations.

Design-change frequency.

Supplier capacity.

Product life.

Demand confidence.

That is why this episode will not give you universal break-even volumes.

We already have the economic tools.

Use project-specific inputs.

---

## 10. The Process Selection Decision Grid

Here is the listener tool.

Start with function.

Then material and required state.

Geometry.

Tolerance and surface.

Lifecycle stage and volume.

Candidate routes.

Capability evidence.

Inspection.

Supplier/resource readiness.

Tooling and NRE.

Yield and secondary operations.

Cost per accepted good unit.

Exit trigger.

Do not score the routes blindly.

First eliminate routes that violate hard requirements.

Then compare the feasible routes.

That is the difference between engineering screening and spreadsheet voting.

---

## 11. Sentinel Node example

Our Sentinel enclosure starts in DEV as a print.

That is useful for packaging.

Then a CNC route may make sense for LVP.

Why?

No hard tooling.

Fast changes.

Good dimensional control.

But if demand grows and the geometry stabilizes, molding may become economically attractive.

Does that mean molding is “more mature?”

No.

It means the evidence/economic envelope changed.

And before switching, the team has to validate the characteristics that the new process changes.

That is route maturity.

Not process prestige.

---

## 12. Five traps to avoid

Geometry selects the process.

Molding equals production and CNC equals prototype.

Cheapest quote equals cheapest manufacturing route.

One successful prototype qualifies the production route.

High-volume process automatically wins at commercial volume.

Supplier brochure capability equals demonstrated source capability.

---

## 13. The action after this episode

Pick one important part.

Force yourself to define at least three plausible manufacturing routes.

For each one write:

What product claims it represents well.

What behavior it introduces.

What evidence is missing.

What tooling or NRE it needs.

What supplier capability matters.

What would make you leave that route.

If you only have one candidate, you may not have made a process-selection decision yet.

---

## Closing

EP11 gave us the selection method.

Now we apply it to the first process family.

Polymers.

Where the manufacturing process does not simply copy geometry.

It creates flow, shrinkage, warpage, surfaces and tooling constraints that become part of the design.

Episode 12:

**Polymer Parts — Injection Molding and the Alternatives.**

# End spoken script

## Draft source anchors — not spoken

- W6A-S01/S05 — NIST material/process selection and multi-attribute decision support.
- W6A-S02/S03/S04 — NIST conceptual process planning/design integration.
- W6A-S06/S07 — current 2026 Manufacturing Cost Guide context only, not part-cost calculator.
- W6A-S08/S09 — additive/economic system-boundary examples.
- Wave 03 — accepted-good-output/lifecycle economics.
