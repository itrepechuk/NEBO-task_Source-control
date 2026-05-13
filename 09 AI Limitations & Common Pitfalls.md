# 09 — AI Limitations & Common Pitfalls

Understanding where AI fails is just as important as knowing where it excels. This guide helps you use AI without being burned by its limitations.

---

## Core Limitations

### 1. Hallucinations
AI can confidently state things that are completely false — fabricated citations, wrong statistics, invented historical events, or non-existent APIs.

**Why it happens:** The model predicts plausible-sounding text based on patterns, not by consulting a database of verified facts.

**How to handle it:**
- Verify any factual claim that matters
- Ask the AI to cite sources — then verify those sources exist
- Be especially skeptical of specific numbers, dates, names, and quotes

---

### 2. Knowledge Cutoff
AI models are trained on data up to a specific date. They don't know about:
- Recent news and events
- New software versions and APIs
- Changes in laws, regulations, or market conditions
- New research published after their cutoff

**How to handle it:**
- Ask the model what its knowledge cutoff is
- Use AI tools with web search for time-sensitive queries
- Always verify technical info against official, up-to-date documentation

---

### 3. No True Reasoning
Despite impressive outputs, current AI models don't "reason" the way humans do. They can fail at:
- Multi-step math problems
- Logic puzzles requiring deep inference
- Tasks requiring genuine understanding of cause and effect

**How to handle it:**
- Ask the AI to "think step by step" (chain-of-thought prompting)
- Verify any mathematical or logical output independently
- Break complex problems into smaller sub-tasks

---

### 4. Context Window Limits
AI can only process a limited amount of text at once. With very long documents:
- It may lose track of early information
- It may skip or compress important details
- Quality can degrade at the end of long outputs

**How to handle it:**
- Break long documents into chunks and process them separately
- Summarize earlier chunks and feed summaries forward
- Use models with larger context windows for long-document tasks

---

### 5. No Memory Between Conversations
By default, AI has no memory of previous conversations. Every session starts fresh.

**How to handle it:**
- Paste relevant context at the start of new conversations
- Use tools with memory features if available
- Keep a "context snippet" for recurring AI tasks

---

### 6. Sycophancy
AI models tend to agree with users — even when the user is wrong. If you push back on a correct answer, the AI may capitulate and change it.

**How to handle it:**
- Don't treat AI agreement as validation
- Explicitly ask: "Are you sure? What are the counterarguments?"
- Ask the AI to argue the opposite position to stress-test ideas

---

### 7. Inconsistency
AI can give different answers to the same question in different conversations — or even within the same conversation.

**How to handle it:**
- For critical outputs, run the same prompt multiple times and compare
- Use specific, constrained prompts to reduce variance
- Don't treat any single AI output as authoritative

---

## Common Pitfalls by Situation

| Situation | Pitfall | Prevention |
|-----------|---------|------------|
| Using AI for research | Fabricated citations | Verify every source manually |
| Asking for legal/medical advice | Oversimplified or wrong guidance | Consult a professional |
| Generating code | Plausible but buggy code | Test thoroughly; code review |
| Writing with AI | Generic, flat tone | Edit heavily for voice |
| Asking about recent events | Outdated information | Use web-enabled AI or search |
| Delegating decisions to AI | Lack of accountability | Human must own the decision |
| Entering sensitive data | Privacy/security breach | Anonymize or avoid sharing |

---

## Red Flags in AI Output

Watch out for these signs that output may be unreliable:

- **"As of my knowledge cutoff..."** — May be outdated; verify
- **Specific statistics without a source** — High hallucination risk
- **Overly confident tone on a complex topic** — AI doesn't express uncertainty well
- **Vague, generic advice** — The model may not have understood your question
- **Perfect-sounding but unverifiable claims** — A classic hallucination pattern

---

## The Right Mental Model

Think of AI as a **very well-read but sometimes unreliable colleague** who:
- Has read enormous amounts of text
- Can synthesize and communicate ideas brilliantly
- Occasionally makes things up with full confidence
- Works best when you give them clear direction
- Needs you to check their work on important matters

---

## Related

- [02-prompt-engineering.md](./02-prompt-engineering.md) — How to reduce errors through better prompts
- [05-safety-and-ethics.md](./05-safety-and-ethics.md) — Why human oversight matters
- [10-glossary.md](./10-glossary.md) — Definitions of hallucination, context window, etc.
