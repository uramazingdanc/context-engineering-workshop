# Module 1: Context Engineering Foundations

## Prompt Engineering vs. Context Engineering

| Dimension | Traditional Prompt Engineering | Systemic Context Engineering |
|---|---|---|
| **Core objective** | Generating text or isolated single-file code snippets | Compiling full-stack, multi-component web apps in an integrated runtime |
| **Memory & state** | Short-term conversational history, prone to cumulative drift | Explicitly bounded system prompts, state variables, visual design rules |
| **Output artifact** | Plain text, unstyled HTML, disconnected scripts | Modular React component trees, dynamic DB schemas, deployment bundles |
| **Error handling** | Manual prompt rewriting, repetitive unguided iteration | One-key automated error-fixing loops, direct point-and-click editing |
| **Boundary enforcement** | Implicit model defaults → token dilution, hallucination | Explicit negative constraints, schema contracts, design tokens |

## System Degradation Vectors

Predictable failure modes when a model runs without explicit context boundaries:

- **Token dilution** — irrelevant/conversational tokens crowd out essential instruction tokens.
- **Context rot & hallucination loops** — without structural invariants, multi-turn iteration causes cumulative drift: broken UIs, dropped routing logic, invented API endpoints.
- **Vague structural boundaries** — ambiguous instructions force the model to infer visual hierarchy, producing inconsistent components.

## Key Takeaway

Context engineering treats the LLM context window as a dynamic execution environment — system roles, domain constraints, memory states, user intent, and structural schemas are programmatically assembled, rather than left to conversational chance.
