# Workflow Fit

A web app for mapping how work gets done (who coordinates with whom, and what happens in what order) and recording agreed decisions about where AI belongs and in what form.

**Status:** MVP in development. Tracked in Linear (team WF, project "Workflow Fit MVP").

## Docs

- [Product requirements](docs/Workflow-Fit-MVP-PRD.md)
- [Technical spec and blueprint](docs/Workflow-Fit-Tech-Spec-Blueprint.md)

The spec is the source of truth for architecture, data model, and security. Change it when decisions change.

## Stack

- Frontend: Vite, React, TypeScript, Tailwind, React Flow, Zustand, TanStack Query
- Backend: Supabase (Postgres with row-level security, Auth, Realtime, one Edge Function)
- Hosting: Vercel (frontend), Supabase (backend)

## Getting started

Requires Node (LTS), the Supabase CLI, and Docker for the local database.

```bash
npm install
supabase start          # local Postgres, Auth, Realtime
cp .env.example .env    # add the local Supabase URL and anon key
npm run dev
```

## Common tasks

| Task | Command |
| --- | --- |
| Run tests | `npm test` |
| Database tests (RLS) | `supabase test db` |
| End-to-end tests | `npm run test:e2e` |
| New migration | `supabase migration new <name>` |
| Regenerate types | `npm run gen:types` |

## How we work

- One Linear issue at a time; branch names include the issue ID (`wf-12-handoffs`).
- Schema changes only through migrations, never in the Supabase dashboard.
- Every pull request must pass CI, including the row-level security tests.
- Only the owner merges.

## Security

Client data is isolated per workspace by row-level security in the database. The service key is used only in the invite Edge Function and must never reach the browser. No client content is sent to third-party AI services.

## Ownership

Copyright © 2026 [OWNER]. All rights reserved. Proprietary and confidential.
