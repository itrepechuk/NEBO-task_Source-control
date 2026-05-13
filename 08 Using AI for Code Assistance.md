# 08 — Using AI for Code Assistance

AI coding assistants can dramatically accelerate development — but only when used thoughtfully. This guide covers best practices for developers.

---

## What AI Does Well in Code

| Task | Quality |
|------|---------|
| Boilerplate generation | ⭐⭐⭐⭐⭐ Excellent |
| Explaining unfamiliar code | ⭐⭐⭐⭐⭐ Excellent |
| Writing unit tests | ⭐⭐⭐⭐ Very Good |
| Refactoring for readability | ⭐⭐⭐⭐ Very Good |
| Debugging with error messages | ⭐⭐⭐⭐ Very Good |
| Generating documentation | ⭐⭐⭐⭐ Very Good |
| Complex algorithm design | ⭐⭐⭐ Good (verify carefully) |
| Security-sensitive code | ⭐⭐ Use with caution |
| Cutting-edge/niche frameworks | ⭐⭐ May be outdated |

---

## Effective Prompts for Coding

### Generate Code
```
Write a [language] function that [what it does].
Inputs: [describe parameters]
Output: [describe return value]
Requirements: [edge cases, performance, style]
```

**Example:**
> "Write a Python function that takes a list of dictionaries and returns them sorted by the 'created_at' key in descending order. Handle the case where the key is missing."

---

### Debug Code
```
This code is supposed to [intended behavior] but instead [actual behavior / error].
Here is the error message: [paste error]
Here is the code: [paste code]
What is causing this and how do I fix it?
```

---

### Review Code
```
Review this [language] code for:
- Readability and naming conventions
- Edge cases or potential bugs
- Performance issues
- Security vulnerabilities
[paste code]
```

---

### Write Tests
```
Write unit tests for this function using [pytest / Jest / JUnit / etc.].
Cover: happy path, edge cases, and error conditions.
[paste function]
```

---

### Explain Code
```
Explain what this code does, line by line, as if I'm a junior developer.
[paste code]
```

---

## Best Practices

### ✅ Do

- **Provide context** — Tell the AI the language, framework version, and constraints
- **Paste error messages** — Include the full stack trace when debugging
- **Review generated code** — AI can produce functional but suboptimal or insecure code
- **Run tests on AI code** — Never deploy AI-generated code without testing
- **Use AI for first drafts** — Treat output as a starting point, not a final product
- **Ask for explanations** — If you don't understand the code, ask the AI to explain it

### ❌ Don't

- **Paste production secrets** — API keys, database credentials, private tokens (see [06-data-privacy.md](./06-data-privacy.md))
- **Trust AI on security logic** — Auth, encryption, and input sanitization require expert review
- **Blindly copy-paste** — Always read and understand the code you're adding to your codebase
- **Rely on AI for niche or very recent libraries** — Training data has a cutoff; check official docs
- **Use AI-generated code in regulated environments without review** — Financial, medical, and safety-critical systems need human oversight

---

## AI Coding Tool Comparison

| Tool | Best For | IDE Support |
|------|----------|-------------|
| **GitHub Copilot** | Inline completions, whole-line suggestions | VS Code, JetBrains, Neovim |
| **Cursor** | Multi-file editing, natural language coding | Cursor (VS Code fork) |
| **Claude** | Complex logic, explanation, large code review | Web / API |
| **ChatGPT** | General coding questions, debugging | Web / API |
| **Claude Code** | Agentic terminal-based coding tasks | Terminal |
| **Codeium** | Free Copilot alternative | Multiple IDEs |

---

## Code Review Workflow with AI

1. **Before submitting a PR** — Paste your diff into Claude and ask for a code review
2. **During debugging** — Share the error, relevant code, and what you've already tried
3. **When learning a new codebase** — Paste a complex function and ask for a plain-English explanation
4. **Writing documentation** — Paste functions and ask for docstrings, README sections, or API docs

---

## Security Note

AI-generated code has been shown to introduce security vulnerabilities in some studies — particularly in areas like:
- SQL injection (unsanitized inputs)
- Insecure deserialization
- Hardcoded credentials
- Missing authentication checks

Always run security linting tools (Bandit, ESLint security plugins, Semgrep) on AI-generated code before merging.

---

## Related

- [02-prompt-engineering.md](./02-prompt-engineering.md)
- [05-safety-and-ethics.md](./05-safety-and-ethics.md)
- [06-data-privacy.md](./06-data-privacy.md)
