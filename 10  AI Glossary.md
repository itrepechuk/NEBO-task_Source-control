# 10 — AI Glossary

A reference guide to key terms you'll encounter when working with AI tools.

---

## A

**Agentic AI**
An AI system that can take sequences of actions autonomously — using tools, browsing the web, running code, or interacting with other systems — to complete a goal.

**AI (Artificial Intelligence)**
The broad field of computer science focused on building systems that can perform tasks typically requiring human intelligence, such as language understanding, reasoning, vision, and decision-making.

---

## B

**Benchmark**
A standardized test used to measure and compare AI model performance. Common benchmarks include MMLU (knowledge), HumanEval (coding), and MATH (mathematics).

**Bias**
Systematic errors or unfairness in AI outputs, often reflecting imbalances in the training data. Can manifest as stereotyping, underrepresentation, or differential performance across groups.

---

## C

**Chain-of-Thought (CoT)**
A prompting technique where the AI is instructed to reason step by step before giving a final answer, improving accuracy on complex reasoning tasks.

**Context Window**
The maximum amount of text (measured in tokens) that an AI model can process in a single interaction — including the conversation history, system prompt, and current message. Larger context windows allow the model to "see" more at once.

**Completion**
The AI's generated response to a prompt. Also called an "output" or "generation."

---

## E

**Embedding**
A mathematical representation of text (or other data) as a vector of numbers. Embeddings capture semantic meaning and are used in search, recommendation, and retrieval systems.

**Emergent Behavior**
Capabilities that arise in larger AI models that were not explicitly trained for — for example, the ability to do arithmetic or translate languages appearing without specific training on those tasks.

---

## F

**Fine-tuning**
The process of further training a pre-trained AI model on a specific dataset to adapt it to a particular task or domain.

**Foundation Model**
A large AI model trained on broad data (text, images, etc.) that can be adapted to many downstream tasks. Examples: GPT-4, Claude, Gemini.

---

## G

**Generative AI**
AI systems that can create new content — text, images, code, audio, video — rather than just classifying or analyzing existing data.

**GPT (Generative Pre-trained Transformer)**
A family of large language models developed by OpenAI. The architecture underlying ChatGPT. "Transformer" refers to the underlying neural network architecture.

---

## H

**Hallucination**
When an AI model generates information that is plausible-sounding but factually incorrect or entirely fabricated — such as fake citations, wrong statistics, or non-existent people. A fundamental challenge in current LLMs.

**Human-in-the-Loop (HITL)**
A design approach where human judgment is incorporated into AI workflows, especially for high-stakes decisions. Ensures accountability and error correction.

---

## I

**Inference**
The process of running a trained AI model to generate a response from a given input. The "live" use of a model (as opposed to training).

**In-Context Learning**
The ability of an LLM to perform new tasks based on examples provided within the prompt, without updating its weights.

---

## L

**Latency**
The time it takes for an AI model to generate a response. Relevant when AI is used in real-time applications.

**LLM (Large Language Model)**
A type of AI model trained on massive amounts of text data to understand and generate human language. The technology behind tools like Claude, ChatGPT, and Gemini.

---

## M

**Model**
The core AI system — a mathematical function with billions of parameters trained to predict outputs from inputs. Different models have different capabilities, sizes, and specializations.

**Multimodal AI**
An AI model that can process and generate multiple types of data — e.g., both text and images (like GPT-4o or Gemini).

---

## P

**Parameters**
The internal numerical values of an AI model, adjusted during training. More parameters generally (though not always) correlate with greater capability. GPT-4 has an estimated ~1 trillion parameters.

**Prompt**
The input text (question, instruction, or context) that you send to an AI model.

**Prompt Engineering**
The practice of crafting prompts to reliably elicit high-quality, accurate, and relevant outputs from AI models. See [02-prompt-engineering.md](./02-prompt-engineering.md).

---

## R

**RAG (Retrieval-Augmented Generation)**
A technique where relevant documents are retrieved from a database and provided to the AI model as context, improving accuracy and grounding responses in real data.

**RLHF (Reinforcement Learning from Human Feedback)**
A training technique where human raters evaluate model outputs, and the model is adjusted to produce outputs that humans prefer. Used to make models more helpful and safe.

---

## S

**System Prompt**
Background instructions provided to an AI model that shape its behavior, persona, and constraints — typically set by the developer or platform, not visible to the end user.

**Sycophancy**
The tendency of AI models to agree with users or change their answers under pressure, even when the original answer was correct.

---

## T

**Temperature**
A parameter controlling the randomness of AI outputs. Low temperature (e.g., 0) = deterministic and repetitive. High temperature (e.g., 1+) = more varied and creative.

**Token**
The basic unit of text that language models process. Roughly equivalent to ¾ of a word in English. "The quick brown fox" is about 4 tokens. Model costs and context limits are measured in tokens.

**Training Data**
The large corpus of text (and other data) used to train an AI model. The quality and composition of training data significantly influence model capabilities and biases.

**Transformer**
The neural network architecture underlying most modern LLMs, introduced in the 2017 paper "Attention Is All You Need." Processes entire sequences in parallel using "attention mechanisms."

---

## Z

**Zero-Shot**
Asking an AI to perform a task without providing any examples. Contrast with few-shot (a few examples) or fine-tuning (training on many examples).

---

*For more context on how these concepts affect real usage, see [09-limitations-and-pitfalls.md](./09-limitations-and-pitfalls.md).*
