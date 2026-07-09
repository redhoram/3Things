---
name: solve
description: "Analyze a problem in three layers — Problem, Root Cause, and Solution — using the 3Things problem-solving framework. Use this whenever the user is facing something that's going wrong and wants to fix it: \"why does X keep happening,\" \"how do we fix Y,\" \"our process is slow / broken / failing,\" \"keep hitting the same issue,\" \"troubleshoot this,\" or any request to diagnose a recurring problem and design a fix. Trigger even when the user jumps straight to asking for a solution — the value of this skill is forcing a dig into the ROOT CAUSE first, so the fix attacks the disease, not just the symptom."
---

# Solve — Problem · Root Cause · Solution

Structure any problem into three layers: **what's wrong (Problem), why it's really happening (Root Cause), and what to do about it (Solution).** This is the most fundamental problem-solving frame in 3Things — and its whole power is the discipline of *not leaping to the solution* until the root is understood.

Treating a symptom without touching the root just makes the problem come back — like taking a fever reducer without treating the infection underneath.

## Not this skill?

- Weighing named alternatives ("A or B?") → use /decide
- No defect to fix, just a goal to reach → use /plan
- Only needs condensing, not fixing → use /summarize

If the request mixes them (e.g. "diagnose this, then pick a fix"), run this skill first, then hand the result to the next one.

## Before diagnosing

If the input lacks the facts needed to reach a real root cause, ask up to three targeted questions first. If the user wants an answer immediately, proceed — but flag every inferred cause as (hypothesis), not a finding.

## The three steps

1. **Define the problem clearly.** State what is actually wrong, plainly and specifically. A vague problem produces a vague fix.
2. **Dig for the root cause.** This is the step people skip most. Don't stop at the symptom — keep asking *"why?"* until you reach the real cause. What looks like the problem is often just a symptom of something deeper.
3. **Design a solution that attacks the root**, not one that merely papers over the symptom.

## The tool: ask "why" a few times (the 5 Whys)

Peel one layer per "why":

> Sales are down — why? Because customers are leaving. Why are they leaving? Because they're complaining. Why are they complaining? Because delivery is slow. Why is delivery slow? Because the warehouse is a mess.

The true root is *a messy warehouse* — not "sales are down." Stop at the first layer and you'll waste money on expensive promotions that fix nothing, because the problem was never there. Three to five "whys" is usually enough to hit bottom.

## Required output format

Write the entire output in the user's language — Indonesian input gets an Indonesian analysis, including the structure labels (Problem → Masalah, Root Cause → Akar Masalah, Solution → Solusi). The template below shows English labels only as placeholders.

Always present the analysis in these three labeled layers:

```
**Problem**
[The symptom, stated clearly and specifically.]

**Root Cause**
[The real underlying cause, reached by asking "why" down the chain.
 Show the why-chain briefly if it helps make the logic visible.
 Mark each link as (fact) — stated by the user — or (hypothesis) —
 your inference. Never present a hypothesis as a confirmed diagnosis.]

**Solution**
[Actions that target the root cause — not the symptom. If the root is
 a hypothesis, step 1 is the cheapest way to verify it — then the fix.]
```

If several root causes surface, group them (ideally into about three) and let the solution address each.

## Example

> **Problem**
> Our procurement process is too slow.
>
> **Root Cause**
> Digging in: requirements aren't defined clearly up front → approvals are multi-layered and slow → everything is still manual and paper-based.
>
> **Solution**
> Put in a digital system with electronic approvals and a standard catalog — hitting all three root causes at once.

Compare that to just telling people to "work faster." That's a symptom fix; the problem would never actually go away.

## Guardrails

- **Resist the jump to solution.** The instinct on seeing a problem is to reach for a fix immediately — it feels productive. But a solution built before the root is understood almost always misses. Hold the discipline: sit in the first two steps until the diagnosis is real.
- **Don't stop at the first "why."** The first answer is almost always still a symptom. Keep peeling.
- **Match the fix to the cause.** Every proposed action should trace clearly to a root cause you identified. If it doesn't, it's probably treating a symptom.
- **Slowing down to think is often faster.** Most big mistakes come from treating symptoms instead of roots. The deliberate pause to diagnose usually beats rushing in and having to redo the fix.
