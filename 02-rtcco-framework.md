# Module 2: The RTCCO Prompting Framework

RTCCO structures natural language into machine-executable specification blocks for deterministic, high-fidelity software generation.

| Component | Structural Purpose | Execution Mechanics | Example |
|---|---|---|---|
| **Role** | Persona invariant | System prompt framing | "Act as a Lead Product Designer and Senior Full-Stack Engineer." |
| **Task** | Primary objective | Action execution statement | "Build an interactive retail application titled EcoShift Marketplace." |
| **Context** | Domain environment | In-context learning (ICL) | "Targeting eco-conscious consumers using clean earth tones and sustainable themes." |
| **Constraints** | Structural guardrails | Negative prompting rules | "Responsive mobile-first layout; clean off-white background; dark slate typography; no paid dependencies." |
| **Output Format** | Schema definition | Visual tree & database contract | "Include Hero Section, Product Grid with 4 items, slide-out Cart Drawer, and Impact Calculator slider." |

## Advanced Techniques

- **Sequential logic prompting** — instruct the model to construct backend schemas *before* UI bindings, preventing hydration errors.
- **Design system rule injection** — define precise Tailwind CSS utility tokens directly inside Constraints.
- **Negative constraint rules** — explicitly ban generic blue buttons, hardcoded cart totals, non-functional placeholders.

See [`prompts/rtcco-template-library.md`](../prompts/rtcco-template-library.md) for reusable templates.
