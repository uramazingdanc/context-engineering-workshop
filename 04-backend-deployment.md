# Module 4: Backend Integration, GitHub Sync, and Deployment

## Why It Matters

State stored only in browser memory resets on refresh. Production readiness requires persistent database storage, authentication, and security policies.

## Step-by-Step

1. **Database schema creation** — prompt: *"Store customer orders in a database table called orders. Include columns for customer_email, total_amount, order_items (JSON), and created_at. Ensure Row Level Security (RLS) is enabled so users only see their own data."*
2. **Migration review** — Lovable creates a SQL migration in `supabase/migrations/`, executes it, applies RLS policies, updates TypeScript interfaces.
3. **GitHub sync** — click **GitHub** in the nav header → authorize access → **Create Repository**. All React, Tailwind, and TypeScript code syncs to a private or public repo.
4. **Live deployment** — click **Publish → Update Public URL**. The app builds and deploys to a `*.lovable.app` domain within seconds. Test on mobile for responsive layout.

## Code Ownership & Sync

- **Bi-directional GitHub sync** — clone the repo, edit locally in VS Code, push changes back into the Lovable visual canvas.
- **Deployment versatility** — publish to `lovable.app`, or build and host externally on Netlify, Vercel, Cloudflare Pages, AWS, or self-hosted Docker.
