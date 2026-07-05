# Prompts — Full Exercise Flow

Copy-paste-ready prompts for all four steps of the exercise, in order. Steps 1 happens in **NotebookLM**; Steps 2–4 happen in **Gemini**.

---

## Step 1 — NotebookLM: Market Research Prompt

Run this in your NotebookLM workspace after uploading the CRED and WhatsApp/fintech sources (see [`docs/market-synthesis-playbook.md`](../docs/market-synthesis-playbook.md)):

```
Based on the uploaded sources, what are the top 3 behavioral
psychology levers CRED uses to retain its high-trust user base?
```

**Why this prompt:** Monetization strategy borrowed from a competitor only works if you understand *why* it works. This surfaces the retention mechanics (exclusivity, gamified trust scoring, social status signaling) that carry over into the WhatsApp persona work in Step 2.

Pin the answer as a **Note** before moving on — see [`screenshots/README.md`](../screenshots/README.md) for what to capture (`step-3-save-as-note.png`).

---

## Step 2 — Gemini: Persona Creation Prompt

Open [gemini.google.com](https://gemini.google.com/) and paste in your NotebookLM findings as context, then run:

```
Act as an expert Product Strategist. Based on the fact that CRED
relies on exclusivity and high-trust financial behavior, create 3
detailed user personas in India (Name, Age, Income, Tech-Savviness,
Pain points) who would be the ideal early adopters for a 'WhatsApp
Premium Trust Tier'. Give them distinct financial habits.
```

**Why this prompt:** Turns the raw behavioral research into three concrete, distinct target-user profiles you can stress-test a feature against. See [`reference-outputs/personas.md`](../reference-outputs/personas.md) for a full worked example (Adit, Riya, and Vikram).

---

## Step 3 — Gemini: Feature Stress-Test Prompt

With the 3 personas still in context, propose the actual feature and simulate a focus group:

```
I am proposing a new feature: 'WhatsApp Trust Score'. Users with a
score over 800 (based on timely utility bill payments via WhatsApp
Pay) get exclusive access to premium D2C brands at a 20% discount
directly in the chat interface.

Please simulate a focus group interview. You will play the role of
the 3 personas you just created. For each persona, tell me:
1. Their immediate reaction to the feature.
2. The biggest friction point.
3. One incentive that would make them switch.
```

**Why this prompt:** Replaces months of recruiting and running real focus groups with an instant, repeatable stress-test — see [`reference-outputs/focus-group-transcript.md`](../reference-outputs/focus-group-transcript.md) for the full simulated interview.

---

## Step 4 — Gemini: Strategic Synthesis & Go/No-Go Prompt

Copy the full focus group transcript from Step 3 into a **new** Gemini prompt (fresh context helps it analyze rather than just continue the roleplay), then ask:

```
Analyze the friction points across the three personas towards the
WhatsApp Trust Score Feature, highlighting the key points that the
PM should consider for a Go/No-Go decision for the feature.
```

**Why this prompt:** This is the step that turns three interesting conversations into an actual decision document — a friction matrix, the strategic tensions behind each friction point, and a clear recommendation. See [`reference-outputs/go-no-go-analysis.md`](../reference-outputs/go-no-go-analysis.md) for the full analysis, which landed on **"No-Go in current form"** with three specific conditions to flip it to a Go.

---

## Tips for better answers

- **Carry context forward deliberately.** Gemini doesn't automatically remember your NotebookLM findings — paste the pinned notes in as context before Step 2.
- **One question per prompt.** Resist bundling persona creation and feature stress-testing into a single message; the model reasons better in sequence.
- **Ask it to justify, not just conclude.** If Step 4's verdict feels thin, follow up with "Which single friction point is the biggest blocker, and why?"
- **Treat the output as a first draft.** The Go/No-Go verdict is a strong starting point for a real conversation with your VP, not a substitute for it.
