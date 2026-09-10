# A1 Full Script Draft V1 — From an Idea to Engineering Requirements

status: FULL SCRIPT DRAFT V1 — EDITORIAL/TECHNICAL SCRIPT REVIEW NEXT
season: Season 1 — Build the Right Hardware Before Production Finds Your Mistakes
source_outline: `A1_SCRIPT_OUTLINE.md`
source_lock: `evidence/source-lock/wave-01/`
spoken_standard_claims: NONE PLANNED
real_case_claims: NONE — opening and Sentinel examples are illustrative

## Production note — not spoken

This draft intentionally keeps named standards out of the main narration unless they improve understanding. Authoritative NASA/ISO references belong primarily in source notes/show notes. The engineering premises are source locked; the listener tools and DEV/LVP/SVP framing are Hardware-to-Production synthesis.

---

# SPOKEN SCRIPT

## Opening

Imagine this.

A small hardware team has a good idea. The problem is real, the engineers are capable, and everybody is excited to finally build something.

Mechanical starts CAD.
Electronics starts choosing components.
Firmware starts on the dev board.
Someone orders connectors.
Someone else starts printing an enclosure.

Six weeks later, the first serious integration starts.

And suddenly the team discovers that nobody ever agreed on some very basic things.

What temperature does the product actually have to operate in?
How much power can it consume?
Which direction does the connector need to face in the real installation?
Can the customer clean it with alcohol? With detergent? With something more aggressive?
Is this an indoor product that may see an occasional splash, or an outdoor product that has to survive rain?
How often is it serviced?
How much space does the installer actually have around it?

None of the engineers necessarily did bad engineering.

The mechanical engineer solved one version of the product.
The electronics engineer solved another.
The firmware engineer solved a third.

The team had an idea.
It did not yet have enough shared engineering truth.

That is what this episode is about.

Not bureaucracy.
Not a hundred-page specification before you are allowed to touch a screwdriver.

The question is much smaller and much more useful:

**What do we need to make explicit before CAD, PCB and prototype work become expensive to unwind?**

By the end of this episode, I want you to be able to build one page: a Minimum Useful Requirements Sheet for the product you are working on now.

Not the final specification.
The minimum set of truths, targets and visible unknowns that make the next engineering step intentional.

---

## 1. An idea is direction. A requirement is an engineering input.

Most hardware products begin in language that is completely reasonable for an idea and almost useless for detailed engineering.

“We need a rugged sensor.”

“We need a portable machine.”

“It needs to be fast.”

“It has to work outdoors.”

“The customer wants it easy to service.”

Those statements are not wrong.
They are simply not finished.

Take “rugged.”

Rugged against what?
Temperature?
Drop?
Continuous vibration?
Dust?
Water?
Chemicals?
A technician hitting it with a tool cart?

Take “portable.”

Does portable mean one person can carry it?
Does it mean it fits in a vehicle?
Does it need a battery?
How long must it run?
What is the maximum acceptable mass?

Take “fast.”

Fast response?
Fast cycle time?
Fast startup?
Fast data transfer?
Fast installation?

Engineering starts becoming coordinated when those vague words become observable outcomes and constraints.

The important point is not that every statement needs a perfect number today.

The important point is that the team can see what it knows, what it only believes, and what still has to be learned.

That distinction is going to appear throughout this entire series.

A mature engineering team is not a team that knows everything early.

It is a team that knows which things are facts, which are assumptions, and which assumptions are about to become expensive.

---

## 2. The Minimum Useful Requirements

So what should go on the page?

I like to start with seven buckets.

You do not need fifty requirements in every bucket.
You need enough information to stop important design decisions from being driven by invisible assumptions.

### Bucket one: Function and performance

What must the product actually do?

And where it matters, how well must it do it?

Maybe it has to measure temperature.
Maybe it has to move a load.
Maybe it has to detect a defect.
Maybe it has to maintain pressure.
Maybe it has to transmit data.

Then ask whether there is already a meaningful performance target.

Accuracy.
Force.
Speed.
Range.
Response time.
Capacity.
Power.

If you know the value, write it.

If you only know a target range, write the range.

If you do not know yet, write that too.

A blank cell is dangerous because people fill it in mentally with different answers.
A visible TBD can be managed.

### Bucket two: Interfaces

What does the product physically or functionally connect to?

Mechanical mounting.
Connectors.
Voltage and current.
Communication protocol.
Fluid connection.
Thermal interface.
User interface.
Service interface.

Interfaces are where one person's perfectly reasonable assumption becomes another person's integration failure.

So make them visible early.

You do not have to solve every interface on day one.
But you should know which interfaces exist and which ones are still uncertain.

### Bucket three: Environment and operating context

Where will the product live?

Temperature.
Humidity.
Vibration.
Shock.
Dust.
Water.
Chemicals.
UV.
Corrosion.
Storage.
Transport.
Duty cycle.

Again, the objective is not to invent precision.

If the customer has not defined a temperature range, do not make one up just to make the document look complete.

Write:
“Operating temperature — TBD. Must be resolved before component derating and enclosure thermal design are frozen.”

Now the unknown has an engineering consequence and an expiration point.

### Bucket four: Safety and compliance watchlist

This is not where you declare the product compliant.

This is where you ask whether there are hazards, markets, customers or regulations that could change the architecture if discovered too late.

Electrical isolation.
Moving machinery.
Pressure.
Hot surfaces.
Lasers.
Batteries.
Chemicals.
Medical use.
Food contact.
Explosive atmosphere.
Radio equipment.

Different products and markets have completely different obligations.

The lesson here is not “apply this standard.”

The lesson is: **discover the boundary before the boundary redesigns the product for you.**

### Bucket five: Reliability, life and service

How is the product expected to live?

Continuous operation or occasional use?
Disposable or repairable?
Five-minute module replacement or factory return?
Consumables?
Maintenance interval?
Expected downtime?

You may not have final answers in early development.

But service assumptions can change fasteners, access, connectors, enclosure architecture, diagnostics and software behavior.

So if service matters to the product, it belongs in the conversation before the enclosure is beautiful and impossible to open.

### Bucket six: Manufacturing and supply horizon

This one needs restraint.

Early hardware teams sometimes make two opposite mistakes.

The first is ignoring manufacturing completely until the prototype is finished.

The second is trying to design a million-unit factory for a product that has not yet proved anybody wants ten units.

What you need early is the horizon.

Are we making three prototypes?
Thirty field units?
Three hundred early customer units?
Is there a credible path to thousands?

Do we already know that a certain component has long lead time or only one realistic supplier?

Will the product require calibration?
Will every unit require final test?
Is there an assembly feature that will obviously become painful once somebody other than the inventor builds it?

You are not designing the final production system yet.

You are making sure today's architecture does not unknowingly assume that tomorrow's production problem does not exist.

### Bucket seven: Assumptions and TBDs

This may be the most useful part of the sheet.

For every important unknown, record five things:

What are we assuming today?
Why is it unknown?
What will teach us the answer?
Who owns that learning?
When does the assumption expire?

That last question changes everything.

“Sensor accuracy TBD” is not necessarily a problem during early characterization.

It becomes a problem when the customer claim, calibration method or acceptance test depends on the accuracy value.

“Connector TBD” can be fine on a bench prototype.

It stops being fine when enclosure geometry, sealing, cable compatibility or production test depends on the connector.

The goal is not to eliminate uncertainty.

The goal is to stop uncertainty from becoming invisible architecture.

---

## 3. Requirement or solution?

There is another trap worth catching early.

Teams often write the design they already imagined and call it a requirement.

For example:

“The module shall use four M3 screws.”

Maybe that is a legitimate constraint.
Maybe the whole platform uses those screws.
Maybe the customer requires compatibility.
Maybe a safety analysis or service strategy led to that choice.

But maybe the real requirement is:

“A technician must be able to replace the module in the installed environment using the defined service tools.”

Those are not the same statement.

The first one tells the designer the solution.
The second one tells the designer the required outcome.

Why does this matter?

Because early in development, design space is valuable.

If you freeze solutions without remembering why they exist, you can spend months optimizing around a decision that was never actually required.

So add one simple field to important requirements:

**Why?**

Where did this come from?
Customer need?
Interface?
Hazard?
Existing platform?
Business decision?
Regulation?
A previous failure?

You do not need an essay.
One line of rationale can prevent a surprising amount of future confusion.

---

## 4. Unknowns are allowed. Invisible unknowns are not.

Let's take a simple example.

Your product uses a sensor, and you do not yet know what final accuracy is realistic across temperature.

One option is to write a confident-looking number because the requirements spreadsheet needs a value.

That feels decisive.
It is also fiction.

The other option is to write:

“Accuracy target: plus or minus X in nominal conditions. Full temperature accuracy TBD after characterization test T-01.”

Now engineering can move.

Electronics knows what is being explored.
Firmware knows calibration may change.
Mechanical knows temperature behavior may matter.
Test knows an experiment is coming.
Product knows the external claim is not final.

The team has not solved the uncertainty.

It has controlled the uncertainty.

That is a much more realistic picture of early hardware development.

And as the product matures, some of those TBDs have to disappear.

Not because “the process says so.”

Because other decisions start depending on them.

A requirement becomes expensive to leave vague when it controls an interface, safety decision, supplier specification, tooling commitment, customer claim, verification criterion or production acceptance decision.

That is the expiration trigger.

---

## 5. Eight questions for a requirement that matters

Here is the second tool for this episode.

Take any requirement or important constraint and ask eight questions.

**One: Why?**
What need, hazard, interface or business constraint drives it?

**Two: What?**
What observable outcome are we actually asking for?

**Three: How much?**
Does this need a value, range or unit?

**Four: Where and when?**
Under what operating conditions does the requirement apply?

**Five: Who or what depends on it?**
Which subsystem, supplier, test, service activity or interface will make decisions based on this answer?

**Six: How could we verify it?**
Not the full test plan. Just the verification idea.
What evidence could tell us whether it is true?

**Seven: What is its maturity?**
Confirmed requirement?
Target?
Assumption?
TBD?

**Eight: What happens if it changes?**
Who must know, and which current decisions might need another look?

If you cannot answer all eight today, that is fine.

The point is to see which blanks are harmless and which blanks are already driving design.

---

## 6. Sentinel Node: turning a sentence into useful engineering truth

Throughout this series we will use a fictional product called the Sentinel Node.

It is a small industrial condition-monitoring device mounted near rotating equipment. It measures vibration and temperature, processes some information locally and communicates with an industrial system.

The original product sentence might be:

“Build a rugged industrial sensor node that monitors machines.”

Good product direction.
Not enough to coordinate engineering.

So let's create a deliberately incomplete first requirements sheet.

Function:
Measure vibration and temperature well enough to support the target condition-monitoring use case.

Notice I did not invent an accuracy number yet.
That becomes a target/TBD tied to characterization.

Power:
24-volt industrial supply is the current candidate.
The exact allowable supply range and transient behavior still need to be defined.

Mounting:
The node must attach to the target machine without requiring modification of the process equipment.
The mounting geometry and transfer behavior are still being investigated.

Communication:
A wired industrial interface is the current direction.
Final protocol and connector are not yet frozen.

Environment:
Industrial dust and wet exposure are expected.
Exact ingress and temperature requirements are still under investigation.

Service:
Field replacement should be possible without opening the process equipment.
The exact service-time target is not yet defined.

Development access:
Programming and debug access are required during development.
We have not yet decided what remains accessible in the production product.

Now add the unknowns.

Sensor accuracy across temperature — resolve through characterization.

Mounting transfer function — resolve through representative installation tests.

Ingress target — resolve from customer environment and risk/compliance investigation before final enclosure architecture.

Connector family — resolve before sealing, cable and production-test interfaces are frozen.

Calibration method — resolve before low-volume production planning.

Is Sentinel Node now production ready?

Of course not.

But look at what changed.

Mechanical and electronics are no longer designing against completely different invisible products.

The next prototype has questions it is supposed to answer.

And when one of those assumptions changes, the team can see what else might move with it.

That is the purpose of early requirements.

Not certainty.
Coordination and learning.

---

## 7. Verification begins earlier than the test lab

There is one habit I want you to add to every important requirement from the beginning.

Ask:

**How could we eventually know this is true?**

If the requirement is maximum mass, maybe the method is obvious.

If it is sealing performance, the test article, assembly method and exposure conditions matter.

If it is sensing accuracy, calibration and measurement uncertainty matter.

If it is “easy to service,” you may realize that the statement is not yet defined well enough to verify at all.

You do not need to create the full verification plan in the first meeting.

But thinking about the evidence while the architecture is still flexible can expose a requirement that is vague, impossible to test or dependent on an interface nobody has designed access for.

Later in this season, we will spend a full episode on verification planning.

For now, the field on the sheet can simply say:

Verification idea.

What kind of evidence would make this claim believable?

---

## 8. What changes from DEV to LVP to serial production?

One reason requirements get a bad reputation is that people imagine only two states.

Either you are a startup and everything changes every day.

Or you are a giant company and the specification is frozen forever.

Real hardware development is not that binary.

In early development, your requirements baseline may contain targets, ranges, assumptions and TBDs.

The point is learning.

As you move toward low-volume production, more decisions start depending on those requirements.

Supplier specifications.
Interfaces.
Inspection limits.
Production tests.
Calibration.
Work instructions.
Acceptance decisions.

So the requirement and change records have to become more controlled.

By the time you are supporting serial commercial production, the system has to survive more suppliers, more units, more operators, more changes and more field evidence without losing the connection between what the product was supposed to do and what was actually built and verified.

That does not mean requirements stop changing.

It means changes become visible engineering events instead of edits that quietly rewrite history.

We will build that idea carefully as the series continues.

---

## 9. What not to do

Before we close, a few things I do **not** want you to take away from this episode.

I am not telling you to buy an enterprise requirements tool.

I am not telling you to write the complete product specification before prototyping.

I am not telling you that every requirement needs a number today.

I am not telling you that every customer wish should become a requirement.

I am not telling you that manufacturing should dictate every early product decision.

And I am definitely not telling you that a one-page checklist replaces the standards, regulations or safety engineering that may apply to your actual product.

The objective is much simpler.

Make the important truth visible early enough that engineering decisions can learn from each other.

---

## 10. The 20-minute action

Here is what I want you to do after this episode.

Take the hardware product you are working on right now.

Set a timer for twenty minutes.

Do **not** try to write the full specification.

Write only the ten to twenty requirements or constraints where a different answer would materially change the next prototype or architecture decision.

For each one, write:

The requirement or target.

Its status: confirmed, target, assumption or TBD.

Why it exists.

Who owns the next decision or learning activity.

Your current idea for how it could eventually be verified.

And the point at which the unknown can no longer safely stay unknown.

Then circle the lines where two disciplines could currently be assuming different answers.

That list is not paperwork.

That list is your next engineering meeting.

---

## Closing

At this point, we have moved from:

“I know what product I want to build”

to:

“We have enough shared engineering truth to begin making intentional technical decisions.”

But the moment you write down what must be true, another problem appears.

Who owns making each part of it true?

Mechanical?
Electronics?
Firmware?
Systems?
Test?
Manufacturing?
A supplier?
Someone nobody has hired yet?

That is where we go next.

In A2: **The Hardware Team Map.**

Because a requirement with no owner is just another assumption waiting to become expensive.

---

# End spoken script

## Draft source anchors — not spoken

- S-W1-01 — NASA Systems Engineering Handbook §4.0 System Design Processes / §4.2 Technical Requirements Definition.
- S-W1-02 — NASA Systems Engineering Handbook §6.2 Requirements Management.
- S-W1-03 — NASA Systems Engineering Handbook §5.3 Product Verification.
- S-W1-05 — NASA Systems Engineering Handbook Appendix C/D.
- ISO/IEC/IEEE 29148:2018 — show-notes/current-standard context only unless later full-text clause verification is added.

## Draft production flags

- No real-world case is implied by the opening scenario.
- No universal regulatory obligation is stated.
- No ISO clause-level claim is spoken.
- No engineering-significant numerical data are presented as empirical facts.
- `10–20 requirements` and `20-minute action` are editorial exercise guidance, not evidence-based thresholds.
- Sentinel Node is explicitly fictional and its requirements are illustrative.
