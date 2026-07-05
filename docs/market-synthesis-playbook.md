# Exercise 1: Market Synthesis with NotebookLM

**Time box:** ~15–20 minutes
**Tool:** [NotebookLM](https://notebooklm.google.com/)
**Goal:** Decode fragmented, unstructured market data into a structured strategic foundation — fast enough to act on inside a single working session.

## Why NotebookLM for this step

NotebookLM is purpose-built for exactly this job: point it at a set of source documents, and it answers questions *grounded only in those sources*, with inline citations back to the originals. That's the difference between this workflow and just asking a general-purpose chatbot — you get traceability, which matters when you're about to walk into a leadership room with a recommendation.

## Step 1 — Initialize the environment

1. Open [notebooklm.google.com](https://notebooklm.google.com/).
2. Create a new notebook and title it **"WhatsApp Monetization Strategy"**.
3. This notebook becomes the single, centralized workspace for every finding in this exercise — resist the urge to scatter research across tabs, docs, and Slack threads.

## Step 2 — Upload & cross-reference source material

Find and feed the model **2–3 recent articles, PDFs, or financial summaries** focused on:

- **CRED's business model** and its premium user demographics.
- **WhatsApp Business API & fintech payments in India** — adoption trends, regulatory context, payment volumes.

**Tip:** If you don't have PDFs handy, Click on Add Sources and enter the Market Research Prompt to generate sources to be referenced on the Go.

## Step 3 — Prompt for insights

Use NotebookLM's chat interface to run the targeted prompts in [`prompts/strategic-prompts.md`](../prompts/strategic-prompts.md) against your uploaded sources. These are designed to extract the specific strategic levers you need — not generic summaries.

## Step 4 — Save key insights as Notes

As NotebookLM generates strong answers, **pin the best responses as Notes** inside the notebook. This step matters more than it looks:

- It lets you bypass re-reading the same reports every time you need a fact.
- It isolates the exact premium demographics worth targeting on WhatsApp India.
- It creates a persistent, interactive knowledge base you (or your team) can return to as the strategy pivot evolves — rather than a research doc that goes stale the moment it's shared.

Use the [notes template](../notes-template/synthesis-notes-template.md) to turn your pinned notes into a shareable one-pager once you're done.

## What "done" looks like

By the end of this exercise you should have:

- [ ] A NotebookLM workspace with 2–3 credible sources uploaded
- [ ] Answers to the behavioral-lever and market-gap prompts, pinned as Notes
- [ ] A short written synthesis (using the notes template) that a PM could hand to a VP without further editing

From here, the synthesized notes feed directly into **[Exercise 2: Persona Generation](persona-generation-playbook.md)**, where the same insights are used to construct high-fidelity synthetic user personas in Gemini.
