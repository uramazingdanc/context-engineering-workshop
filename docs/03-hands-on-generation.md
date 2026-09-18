# Module 3: Hands-On Web Generation with Lovable

## Architecture Notes

Lovable functions as a visual compiler for open web standards (not a closed proprietary engine):

- **Frontend runtime** — modular React components in TypeScript, built on Vite, styled with Tailwind CSS.
- **Backend infrastructure** — native Supabase integration: managed Postgres, auth, storage buckets, serverless Edge Functions.
- **Automated database migrations** — prompting for data storage writes SQL migration files to `supabase/migrations/`, executes schema updates, regenerates TypeScript client types.
- **Security rules** — Supabase Row Level Security (RLS) policies restrict read/write access based on auth state.

## Iterative "Vibe Coding" Mechanics

1. **Visual Selection Mode** — click DOM elements directly on the preview canvas to adjust spacing, color, or placement without typing a prompt.
2. **Automated Error Self-Healing** — pressing **F** captures the browser's stack trace on a runtime/compile error, passes it back to the model, and applies an immediate fix.
3. **Agent Mode Execution** — processes multi-step tasks asynchronously: independent codebase navigation, visual iteration, automated problem-solving.

## Live Exercise

Run the [master workshop prompt](../prompts/master-workshop-prompt.md) to build **EcoShift Marketplace**, then:

1. Select the Hero CTA button on canvas and restyle it via a one-line visual edit prompt.
2. Add a category filter dropdown via chat, wired to product state.
3. Trigger and auto-fix a compilation error with the **F** shortcut.
