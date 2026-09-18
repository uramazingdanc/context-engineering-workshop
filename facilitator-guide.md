# Facilitator Guide

Minute-by-minute execution directives, verbal scripts, visual cues, and participant actions for the 60-minute session.

## Modular Timeline

| Module | Duration | Core Focus | Deliverable |
|---|---|---|---|
| 1 | 10 min | Context Engineering Foundations | Paradigm-shift comprehension, failure-vector ID |
| 2 | 15 min | RTCCO Prompting Framework | Structured prompts with negative constraints |
| 3 | 20 min | Hands-On Generation & Vibe Coding | EcoShift Marketplace app on live canvas |
| 4 | 10 min | Backend, Git Sync & Deployment | Supabase persistence, GitHub sync, live deploy |
| 5 | 5 min | Ecosystem Synthesis & Roadmap | Tool comparison, take-home template distribution |

---

## Module 1 — Foundations of Context Engineering (10 min)

**Objective:** Bridge basic chat prompting to structured context engineering; show how low-code AI removes typical prototyping bottlenecks.

**Slides**
- Slide 1: Title & Paradigm Shift — Prompting vs. Context Engineering
- Slide 2: The Context Assembly Runtime Environment

**Script**

> "Today we are stepping beyond simple transactional prompting. When most people use AI, they ask a question and receive text — that's prompt engineering. Context engineering treats the AI's context window as a dynamic software runtime. We don't just ask the AI to write a snippet of code; we programmatically construct its role, its memory, its visual environment, and its strict technical boundaries.
>
> Why do AI models fail when building software? Token dilution and context drift. Tell an AI 'build me a website' and it makes dozens of unguided assumptions — invents styling, misses state logic, gets trapped in error loops. Today we'll build structured context blocks that make AI generate full-stack, production-grade web apps on the first try — zero installs, no command line, no paid API keys."

**Do:** Participants open a browser, confirm access to lovable.dev, log in with Google or GitHub.

---

## Module 2 — The RTCCO Prompting Framework (15 min)

**Objective:** Teach participants to write structured prompts using RTCCO; introduce Chain-of-Thought and rule injection.

**Slides**
- Slide 3: The RTCCO Framework Architecture
- Slide 4: Advanced Precision Techniques — Chain-of-Thought & Design Rules

**Script**

> "Look at the RTCCO structure on screen. We begin with **Role**: 'Act as a Lead Product Designer and Full-Stack Developer.' This primes the model for production-grade UI and clean architecture. Next, **Task**: 'Build a modern web application for EcoShift Marketplace.'
>
> Notice **Context** and **Constraints** — we set visual boundaries: forest green accents, soft off-white background, dark slate typography, full mobile responsiveness. Under Constraints we also state what NOT to do. Finally, **Output** specifies exact components: Hero section, product catalog, slide-out cart drawer, impact calculator. This structural clarity eliminates model guesswork."

**Do:** Demonstrate how Chain-of-Thought prompting makes the model define database relations *before* visual layout — preventing state-hydration errors. See [`docs/02-rtcco-framework.md`](docs/02-rtcco-framework.md) for the full table.

---

## Module 3 — Hands-On Web Generation with Lovable (20 min)

**Objective:** Run the master prompt inside Lovable; use Vibe Coding visual edits and natural-language iteration to refine the app.

**Slides**
- Slide 5: Lovable Workspace & Master Prompt Execution
- Slide 6: Live Visual Edits ("Vibe Coding") & Element Selection
- Slide 7: One-Key Automated Error Self-Healing

**Steps**
1. **Prompt submission** — paste the [master prompt](prompts/master-workshop-prompt.md) into lovable.dev, click **Create Project**. Point out how the prompt is broken into component build tasks.
2. **Canvas parsing** — watch Lovable import Lucide icons, configure Tailwind rules, create React state hooks for cart/filtering, render the preview.
3. **Visual editing ("Vibe Coding")** — select the **Select & Edit** cursor, click the Hero CTA button, type: *"Make this button forest green with rounded-full corners, a subtle hover scale effect, and shadow-md."* Show the instant re-render.
4. **Feature expansion** — in chat: *"Add a category filter dropdown above the product grid with options: All, Home, Electronics, Apparel. Wire this directly to product state."*
5. **Error handling** — on a compilation error, press **F** (or click **Try to Fix**) to auto-capture the stack trace and repair.

---

## Module 4 — Backend, GitHub Sync & Deployment (10 min)

**Objective:** Extend the static frontend into a full-stack app: database persistence, GitHub sync, live publishing.

**Slides**
- Slide 8: Backend Persistence & Supabase Integration
- Slide 9: Bi-Directional GitHub Synchronization
- Slide 10: One-Click Live Publishing & Custom Domains

**Script**

> "Your app is visually complete, but state stored only in browser memory resets on refresh. To go production-ready we need persistent storage, authentication, and security policies. In Lovable, backend infrastructure is powered by Supabase — an open-source Postgres platform. By default you get a built-in cloud backend; connect your own Supabase project with one click if you want direct ownership."

**Steps**
1. **Schema creation** — prompt: *"Store customer orders in a table called orders. Include customer_email, total_amount, order_items (JSON), and created_at. Ensure Row Level Security (RLS) is enabled so users only see their own data."*
2. **Migration review** — show the generated SQL migration in `supabase/migrations/`, the applied RLS policy, and updated TypeScript types.
3. **GitHub sync** — click **GitHub** in the nav header, authorize, click **Create Repository**.
4. **Live deployment** — click **Publish → Update Public URL**. Open the `*.lovable.app` link on mobile to test responsiveness.

---

## Module 5 — Wrap-up and Ecosystem Roadmap (5 min)

**Objective:** Consolidate concepts, compare platforms, hand out take-home resources.

**Slides**
- Slide 11: The Iterative Context Development Loop
- Slide 12: QR Code & Take-Home Resource Suite

**Script**

> "In 60 minutes you went from basic prompting to systematic context engineering — a functional, responsive web app with cart drawers, dynamic filtering, and database migrations, all without writing manual code.
>
> The loop: **Context Framing (RTCCO) → Low-Code Generation (Lovable) → Visual Refinement (Vibe Coding) → One-Click Deployment.** Match the tool to the job: Vercel v0 for isolated UI components, Streamlit for quick Python data dashboards, Lovable for a full-stack, exportable React app backed by Postgres."

**Take-home resources:** see [`resources/`](resources) and [`prompts/rtcco-template-library.md`](prompts/rtcco-template-library.md).
