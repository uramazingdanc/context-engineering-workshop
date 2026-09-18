# Low-Code AI Platform Comparison

| Capability | Lovable | Vercel v0 | Streamlit | Bolt.new |
|---|---|---|---|---|
| **Primary output** | Full-stack React + TypeScript + Vite | React / UI component code | Python application scripts | Full-stack Node/React (WebContainer) |
| **Database integration** | Native Supabase (Postgres) | External / manual wiring | Local session state / custom DB | Manual WebContainer filesystem |
| **Authentication** | Natural-language Supabase Auth | Manual configuration | External auth wrappers | Manual configuration |
| **Schema migrations** | Automated SQL migrations & types | Not supported | Not supported | Manual scripting |
| **Version control sync** | Bi-directional (GitHub/GitLab) | Export to GitHub / copy code | Git-based Community Cloud | Single Git export |
| **Visual canvas editing** | Native point-and-click direct styling | Partial visual editing | None (pure code output) | Code/preview toggle |
| **Enterprise security** | SOC 2 Type II, ISO 27001, SAML/SSO | Vercel Enterprise Suite | Snowflake architecture | Basic SaaS standard |

## When to Use What

- **Lovable** — full-stack, exportable React app backed by a real Postgres database.
- **Vercel v0** — isolated, polished UI components you'll wire up yourself.
- **Streamlit** — quick Python data dashboards/internal tools.
- **Bolt.new** — full-stack Node/React prototyping in a WebContainer sandbox.
