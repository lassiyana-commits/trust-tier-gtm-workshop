# Exercise 2: Persona Generation with Gemini

**Time box:** ~10 minutes
**Tool:** [Gemini](https://gemini.google.com/)
**Goal:** Turn the behavioral research pulled from NotebookLM into concrete, distinct synthetic personas you can design and stress-test against — replacing weeks of recruiting real focus-group participants.

## Step 1 — Open Gemini

Go to [gemini.google.com](https://gemini.google.com/). Carry your NotebookLM findings forward by pasting in the pinned note from Exercise 1 (the behavioral levers CRED uses) as context — Gemini won't see it automatically.

## Step 2 — Run the persona creation prompt

See [`prompts/strategic-prompts.md`](../prompts/strategic-prompts.md#step-2--gemini-persona-creation-prompt) for the exact prompt. It asks Gemini to act as a Product Strategist and generate 3 detailed Indian user personas — with name, age, income, tech-savviness, and pain points — who'd be ideal early adopters of a "WhatsApp Premium Trust Tier."

## What good output looks like

A strong response gives you personas that are genuinely distinct from each other, not variations on the same profile. The reference run in this repo produced:

| Persona | Core driver | Why they matter for the feature |
|---|---|---|
| **Adit** (38, HNW Executive) | Exclusivity & security | Uses CRED for its "fenced," elite community feel — the feature has to feel as visually rich and secure as CRED, not like a plain chat window |
| **Riya** (27, Marketing Professional) | Dopamine & status (Gamification Enthusiast) | Loves variable rewards and spin-the-wheel mechanics — the feature lives or dies on whether the reward loop stays fresh |
| **Vikram** (45, Business Owner, uses the WhatsApp Business API) | Transparency & utility (Skeptical Optimizer) | Wary of spam and hidden logic — needs a transparent score and near-zero friction to trust the feature |

Full generated persona detail (financial habits, pain points, adoption rationale) is captured verbatim in [`reference-outputs/personas.md`](../reference-outputs/personas.md).

## Why this step matters

Static personas built from guesswork or a single stakeholder's assumptions are one of the most common ways PM strategy work goes sideways. Generating personas *from the research itself* — rather than from intuition — keeps the downstream feature stress-test (Exercise 3) honest: each persona's reaction is traceable back to a specific financial habit or pain point, not a vibe.

**Screenshot to capture:** `step-4-persona-prompt.png` — see [`screenshots/README.md`](../screenshots/README.md).

## What's next

→ **Exercise 3: Feature Stress-Test** — propose the actual "WhatsApp Trust Score" feature and simulate a focus-group interview with these three personas.
