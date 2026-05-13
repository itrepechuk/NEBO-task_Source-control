# 02 — Prompt Engineering

Prompt engineering is the practice of crafting inputs to an AI system to get the most accurate, useful, and relevant outputs. It's part skill, part experimentation.

---

## The Anatomy of a Good Prompt

A strong prompt typically includes some combination of:

1. **Role / Persona** — Who the AI should act as
2. **Task** — What you want done
3. **Context** — Background information relevant to the task
4. **Format** — How the output should be structured
5. **Constraints** — Length, tone, what to avoid

### Template

```
You are a [role]. 
I need you to [task].
Here is the context: [relevant background].
Please format your response as [format].
Keep it [length/tone]. Do not [constraint].
```

---

## Techniques

### 1. Zero-Shot Prompting
Ask directly without examples.
> "Summarize the following meeting notes in 5 bullet points."

### 2. Few-Shot Prompting
Provide examples to guide the format or style.
> "Here are two examples of how I write subject lines: [...]. Now write one for this email: [...]"

### 3. Chain-of-Thought Prompting
Ask the AI to reason step-by-step before answering.
> "Think through this problem step by step before giving your final answer."

### 4. Role Prompting
Give the AI a persona to shape its tone and expertise.
> "You are a senior software engineer reviewing a junior developer's code."

### 5. Iterative Refinement
Start broad, then narrow.
> First: "Draft a product announcement."
> Then: "Make it more concise and add a call to action."

---

## Prompt Anti-Patterns to Avoid

| Anti-Pattern | Problem | Fix |
|---|---|---|
| Vague requests | AI guesses your intent | Add specifics and context |
| Asking multiple unrelated questions | Answers get muddled | Split into separate prompts |
| Assuming the AI knows your background | Missing context | State your role and goal |
| Accepting the first output | First drafts aren't always best | Iterate and refine |
| Overloading with instructions | AI may miss some | Prioritize key instructions |

---

## Advanced Tips

- **Use delimiters** to separate parts of a prompt: triple quotes `"""`, XML tags `<document>...</document>`, or dashes `---`
- **Ask for confidence**: "If you're unsure about any part, say so."
- **Request alternatives**: "Give me 3 different versions of this headline."
- **Specify the audience**: "Explain this to someone with no technical background."
- **Use negative constraints**: "Do not use buzzwords like 'synergy' or 'leverage'."

---

## Prompt Examples by Task

### Summarization
> "Summarize the following article in 3 sentences for a busy executive. Focus on the key decision and its implications."

### Writing
> "Write a professional but warm email declining a meeting request. Keep it under 100 words."

### Analysis
> "Here is our Q3 sales data. Identify the top 3 trends and suggest one action for each."

### Brainstorming
> "Generate 10 creative names for a productivity app aimed at remote teams. Make them memorable and domain-friendly."

---

## Further Reading

- [OpenAI Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering)
- [Anthropic's Claude Prompting Guide](https://docs.claude.ai/en/docs/build-with-claude/prompt-engineering/overview)
- See also: [01-getting-started.md](./01-getting-started.md)
