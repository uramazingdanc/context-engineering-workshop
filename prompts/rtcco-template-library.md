# RTCCO Prompt Template Library

Reusable RTCCO (Role, Task, Context, Constraints, Output Format) templates for common app types. Fill in the bracketed fields.

## Landing Page

```
Role: Act as a Lead Product Designer and Front-End Developer.
Task: Build a landing page for [PRODUCT/BRAND NAME].
Context: Targeting [AUDIENCE] with a [TONE/STYLE] aesthetic — [COLOR PALETTE].
Constraints: Mobile-first responsive layout; [FONT/STYLE RULES]; no
  generic stock button colors; no placeholder lorem ipsum text.
Output Format: Hero section with headline + CTA, feature grid
  ([N] items), testimonial section, footer with contact form.
```

## SaaS Dashboard

```
Role: Act as a Lead Product Designer and Full-Stack Developer.
Task: Build a [DOMAIN] dashboard called [APP NAME].
Context: Used by [USER TYPE] to [PRIMARY JOB TO BE DONE].
Constraints: Sidebar navigation; data tables must support sort/filter;
  no hardcoded sample totals once connected to the database; dark and
  light mode support.
Output Format: Sidebar nav, top metrics cards ([N] KPIs), main data
  table, detail drawer/modal for row inspection.
```

## CRUD Tool

```
Role: Act as a Full-Stack Developer.
Task: Build a [ENTITY] management tool for [USE CASE].
Context: Internal tool used by [TEAM/ROLE]; data model includes
  [FIELD LIST].
Constraints: Row Level Security enabled so users only see their own
  records; form validation on required fields; no delete without
  confirmation modal.
Output Format: List/table view, create/edit form, delete confirmation,
  Supabase table named [TABLE NAME] with matching columns.
```

## Tips

- Always define backend schema (Context/Constraints) *before* asking for UI polish — prevents hydration errors.
- State explicit negative constraints ("no generic blue buttons", "no hardcoded totals") to avoid default/placeholder output.
- Use single-line visual-edit prompts for styling tweaks instead of rewriting the whole system prompt.
