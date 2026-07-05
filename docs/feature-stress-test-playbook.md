# Exercise 3: Feature Stress-Test — Simulated Focus Group

**Time box:** ~10 minutes
**Tool:** [Gemini](https://gemini.google.com/) (same conversation as Exercise 2, so the 3 personas stay in context)
**Goal:** Pressure-test a concrete feature proposal against your synthetic personas before it ever reaches a real user.

## The feature under test

**WhatsApp Trust Score:** users with a score over 800 — based on timely utility bill payments via WhatsApp Pay — get exclusive access to premium D2C brands at a 20% discount, directly inside the chat interface.

## Step 1 — Run the stress-test prompt

With Adit, Riya, and Vikram still live in the same Gemini conversation, run the prompt in [`prompts/strategic-prompts.md`](../prompts/strategic-prompts.md#step-3--gemini-feature-stress-test-prompt). It asks Gemini to role-play a focus group: for each persona, what's their immediate reaction, biggest friction point, and one incentive that would make them switch.

## What came back (summary)

| Persona | Immediate reaction | Biggest friction | Incentive to switch |
|---|---|---|---|
| **Adit** (HNW Executive) | Likes the exclusivity of an 800+ barrier, but wants the interface as visually rich as CRED | Trust & security — wary of financial data living inside a social platform he uses for work and family | Total utility automation — auto-scan every bill so he never has to think about due dates |
| **Riya** (Gamification Enthusiast) | Loves it immediately — the 800 score feels like a game level to beat | Reward fatigue — will lose interest if the D2C brands on offer feel generic or repetitive | Social status — shareable NFT-style badges on her WhatsApp Status to show off her score |
| **Vikram** (Skeptical Optimizer) | Sees clear value in the discount, but distrusts an opaque scoring system | Inbox clutter — fears marketing blasts turning his chat into a "store" | One-click redemption — discount applied automatically at checkout, no codes or extra taps |

Full simulated interview transcripts (verbatim from the reference run) are in [`reference-outputs/focus-group-transcript.md`](../reference-outputs/focus-group-transcript.md).

## Why this step matters

This is the point in the old workflow where a real strategy team would be scheduling recruiter calls and waiting weeks for a research firm. Here, three structurally different objections — trust/security, reward fatigue, and inbox clutter — surface in a single prompt, each one traceable to a specific persona trait from Exercise 2, and each one mapped to a named behavioral framework (the Hook Model, the BJ Fogg Behavior Model).

**Screenshot to capture:** `step-5-focus-group-simulation.png` — see [`screenshots/README.md`](../screenshots/README.md).

## What's next

→ **Exercise 4: Strategic Synthesis & Go/No-Go** — feed this transcript back into Gemini and ask it to synthesize the friction points into an actual product decision.
