---
name: decide
description: "Turn a decision into a transparent, trustworthy recommendation using the 3Things \"Options — Pros/Cons — Recommendation\" framework. Use this whenever the user is weighing choices or wants help deciding: \"should I do A or B,\" \"which option is best,\" \"help me choose between,\" \"evaluate these vendors/tools/offers,\" \"pros and cons of,\" or reviewing a proposal and deciding whether to go ahead. Trigger even when the user leans toward one option already — the value here is laying out the alternatives, weighing each honestly, and giving a reasoned recommendation others can trust, instead of a gut call."
---

# Decide — Options · Pros/Cons · Recommendation

Structure any decision into three parts: **the choices available (Options), the honest trade-offs of each (Pros/Cons), and a reasoned pick (Recommendation).** This is the 3Things decision frame. Its power isn't only the decision it produces — it's the *trust* it builds. When people see the alternatives and the honest trade-offs, they see your recommendation is considered judgment, not a hunch, and they tend to accept it even if they started out disagreeing.

## The three steps

1. **List the options.** Lay out the real alternatives — ideally around three.
2. **Weigh pros and cons honestly.** For each option, give its genuine upsides and downsides.
3. **Recommend.** Pick the one with the greatest benefit and the most acceptable downside — or a sensible middle path — and say *why*.

## Required output format

Always present the decision like this:

```
**The decision:** [one line stating what's being decided]

**Option 1 — [name]**
- Pros: [honest upsides]
- Cons: [honest downsides]

**Option 2 — [name]**
- Pros: [honest upsides]
- Cons: [honest downsides]

**Option 3 — [name]**
- Pros: [honest upsides]
- Cons: [honest downsides]

**Recommendation:** [the pick] — because [the reasoning, tied to the trade-offs above].
```

## Example

> **The decision:** How to get from Jakarta to Bandung.
>
> **Option 1 — Car**
> - Pros: flexible; set your own route and timing.
> - Cons: need to own or rent a car and buy fuel; tiring.
>
> **Option 2 — Train**
> - Pros: relaxed; you can sleep on the way.
> - Cons: must book a ticket and follow the schedule.
>
> **Option 3 — Plane**
> - Pros: fastest.
> - Cons: expensive, and still tied to a flight schedule.
>
> **Recommendation:** Take the train — it offers the best balance of comfort and practicality for this route.

The decision becomes clear *and* justified — anyone can see the reasoning and follow it.

## Guardrails

- **No straw-man options.** Never pad the list with fake choices to make your favorite look better. Sharp people smell it instantly, and the trust you were building collapses.
- **Be honest both ways.** Admit the downsides of the option you recommend, and the upsides of the ones you reject. That honesty is exactly what makes the recommendation strong — a good decision isn't afraid of the alternatives; it gets stronger for having been tested against them.
- **Always land the recommendation.** Laying out options without a pick leaves the user where they started. Weigh, then choose, and give the reason. (If the user explicitly wants only the trade-offs and will decide themselves, respect that.)
- **Around three options is the sweet spot.** One isn't a decision; five or more overwhelms and paralyzes. If there are many alternatives, honestly narrow to the strongest few.
- **How you present the decision matters as much as the decision.** A bare "we're picking the train" with no reasoning feels arbitrary and invites pushback, even when it's the right call. Show the work.
- Claude gives the factual trade-offs to support the user's own informed choice; for legal, financial, medical, or similarly weighty personal decisions, it notes it isn't a licensed professional in that field.
