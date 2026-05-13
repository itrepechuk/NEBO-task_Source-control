# 06 — Data Privacy & What Not to Share with AI

When you use an AI assistant, your prompts are typically sent to a remote server. Understanding what happens to that data — and what you should never share — is essential.

---

## How AI Tools Handle Your Data

Most AI providers:
- Process your input on their servers to generate a response
- May retain conversations for safety monitoring or model improvement (varies by provider and settings)
- Offer enterprise/API tiers with stronger data protection and opt-outs from training use

| Provider | Default Data Use | Enterprise Option |
|----------|-----------------|-------------------|
| Anthropic (Claude) | May use conversations to improve models (opt-out available) | Claude for Enterprise — no training on data |
| OpenAI (ChatGPT) | Similar; opt-out available in settings | API & Enterprise tiers available |
| Google (Gemini) | Reviewed by humans in some cases | Google Workspace with DPA |
| Microsoft Copilot | Enterprise tenants have stronger protections | Microsoft 365 compliance features |

**Always check the current privacy policy of the tool you're using.**

---

## 🚫 Never Enter These into AI Tools (Without Explicit Approval)

### Personal Data
- Full names + contact details of real individuals
- Social Security / national ID numbers
- Passport or driver's license numbers
- Biometric data
- Home addresses

### Financial Data
- Credit card or bank account numbers
- Payment credentials
- Salary information of specific individuals
- Unreleased financial results

### Health & Medical Data
- Patient records or medical histories
- Health insurance information
- Any HIPAA-protected information (US) or health data under GDPR (EU)

### Confidential Business Data
- Proprietary source code (use placeholder/anonymized code instead)
- Unreleased product roadmaps
- M&A plans or negotiation details
- Customer contracts with identifying information
- Internal audit findings

### Authentication & Security
- Passwords or API keys
- Private cryptographic keys
- Security vulnerability details for production systems

---

## ✅ Safe Practices

- **Anonymize before sharing.** Replace names, IDs, and specifics with generic placeholders.
  - ❌ "Our customer John Smith at Acme Corp signed a $2M deal"
  - ✅ "A large enterprise customer signed a multi-million dollar deal"

- **Use local/private AI where needed.** For highly sensitive tasks, explore self-hosted or local AI models that don't send data externally.

- **Review your AI tool's settings.** Many tools have options to disable conversation history or opt out of training data use.

- **Use enterprise-tier tools for work.** Consumer AI products have different (often weaker) data protections than enterprise agreements.

---

## GDPR & Regulatory Considerations

If you operate in or serve users in the EU:
- Entering personal data of EU residents into AI tools may trigger GDPR obligations
- You may need a Data Processing Agreement (DPA) with your AI provider
- Data subject rights (erasure, portability) may apply to AI-stored conversations

Consult your Data Protection Officer (DPO) or legal team if in doubt.

---

## Quick Reference Card

```
✅ OK to share with AI            ❌ Never share with AI
─────────────────────────         ─────────────────────────────
Generic business scenarios        Real customer names + data
Public information                Passwords or API keys
Anonymized examples               Internal financial projections
Your own writing for editing      Patient or health records
Hypothetical code problems        Production secrets or credentials
```

---

## Related

- [05-safety-and-ethics.md](./05-safety-and-ethics.md)
- [04-ai-tools-overview.md](./04-ai-tools-overview.md)
