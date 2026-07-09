---
name: plan
description: "Build a plan by working backward from the goal, using the 3Things \"Start from the End\" framework — Output (goal) → Process (steps) → Input (what's needed). Use this whenever the user wants to plan, map out, or figure out how to reach something: \"how do I get to X,\" \"plan for launching/achieving Y,\" \"I want to become/reach Z, where do I start,\" \"roadmap for,\" \"backward plan,\" or setting a goal and needing the path to it. Trigger even when the user starts from \"what's my first step?\" — the value is defining the destination FIRST, so every step actually points at the goal instead of just keeping busy. Do NOT trigger for planning code changes or implementation steps in a coding session — that is Claude Code's plan mode, not this skill. This skill is for real-world goals: business, career, launches, projects."
---

# Plan — Start from the End (Mundur dari Tujuan)

Build the plan by starting at the finish line, not the starting line. Define the goal first, then work backward to how you'll get there and what you'll need. This is the most powerful — and most overlooked — planning technique in 3Things.

The structure is still three, just read in reverse:

- **Output (Goal):** What is the end result you want?
- **Process (How):** What has to be done to reach it?
- **Input (Needs):** What do you need for that process to run?

## Not this skill?

- Something is broken and needs a diagnosis → use /solve
- Weighing named alternatives ("A or B?") → use /decide
- Only needs condensing, not planning → use /summarize

Planning code changes or implementation steps in a coding session is Claude Code's plan mode, not this skill.

## Why work backward

Starting from the beginning traps you in *"what's my first step?"* — and without a clear goal, that first step is often just motion to feel productive. Start from the end, and every step earns its place: it exists *because* it's needed to reach the goal. Clarity about the destination turns work from "busy" into "busy toward something." It's the difference between working hard and going nowhere, and working hard toward something clear. This is also the backbone of backward planning in modern project management: fix the deadline, then count backward to when each stage must finish.

## Before planning

If the Output (goal), timeline, or available resources are missing, ask up to three questions whose answers would change the plan's shape. Draft on assumptions only if the user asks for an immediate draft — then list those assumptions at the top of the plan.

## Required output format

Write the entire output in the user's language — Indonesian input gets an Indonesian plan, including the structure labels (Output (Goal) → Output (Tujuan), Process (How) → Proses (Cara), Input (Needs) → Input (Kebutuhan), Execution order → Urutan eksekusi). The template below shows English labels only as placeholders.

Define the three layers backward (Output → Process → Input), then present the plan forward so it's executable:

```
**Output (Goal)**
[The clear end result — one sentence.]

**Process (How)**
[The steps required to reach it — ideally grouped into about three phases/moves.]

**Input (Needs)**
[What must be in place for the process to run — people, skills, resources, tools.]

**Execution order (forward):**
1. [First thing to secure / do — start from the Inputs]
2. [Next]
3. [...toward the goal]
```

Reasoning runs backward (goal → needs); *doing* runs forward (needs → goal). Give the user both.

## Examples

Winning a competition:
> **Output:** Win the competition.
> **Process:** Train with the right, disciplined program.
> **Input:** Talented athletes and a good coach.
> **Execution (forward):** secure athletes + coach → run the training program → compete to win.

Career target:
> **Output:** Become a manager within five years.
> **Process:** Gain project-leadership experience and specific skills.
> **Input:** Take on more responsibility now; enroll in the right courses.
> **Execution (forward):** volunteer for more responsibility + start the courses → lead projects to build the track record → step into the manager role.

From confusion, the user gets a clear three-step map.

## When to use this vs. describing a process

`Start from the End` is for **planning toward a goal** — a target you want to reach. If the user instead wants to *explain how something already works*, step by step, flip to the forward **Water Flow** — same three layers, read forward — and skip the backward planning steps:

**Input** [what goes in] → **Process** [what happens to it] → **Output** [what comes out]

Present those three in forward order, one line or short paragraph each. Backward planning looks from the finish line and turns around; Water Flow looks forward step by step.

## Guardrails

- **Nail the goal first.** If the Output is fuzzy, the whole plan drifts. Push for a clear, single-sentence end result before mapping steps.
- **Every step must point at the goal.** If a step doesn't trace back to the Output, cut it — it's busywork.
- **Group the steps.** Around three phases keeps the plan graspable; if there are many tasks, cluster them into a few logical phases (e.g., Prep – Execution – Review) each with its own deadline.
- **Deliver reasoning backward, execution forward.** Don't hand the user a reversed to-do list; translate the backward logic into a forward sequence they can actually start on Monday.
