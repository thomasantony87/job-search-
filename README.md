# Job Search Engine

Personal opportunity engine for finding, tracking, and applying to job, consulting, contract, advisor, and fractional opportunities.

## Product Goal

Build one system that remembers the user's profile, target roles, companies, leads, outreach, applications, and session decisions so every work session continues from the previous one.

## Core Services

- GitHub: source code and project history
- Supabase: database, durable memory, application pipeline, future auth
- Vercel: web app hosting and environment variables

## Supabase Project

- Project name: job search engine
- Project ID: hvghhwnssvngoeqnzusw
- Region: ap-northeast-1

## Database Memory Tables

The initial Supabase migration created:

- profile_memory
- target_roles
- companies
- contacts
- opportunities
- applications
- messages
- decisions
- session_summaries

## Required Environment Variables

Public frontend variables:

```env
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=
```

Private server-side variables:

```env
SUPABASE_SERVICE_ROLE_KEY=
```

Never expose `SUPABASE_SERVICE_ROLE_KEY` in browser/client code.

## Planned App Stack

- Next.js
- TypeScript
- Supabase JS client
- Server-side API routes for private database writes
- Vercel deployment from GitHub

## First Product Modules

1. Profile memory
2. Target role strategy
3. Opportunity tracker
4. Application pipeline
5. Outreach/message drafts
6. Session memory summaries
7. LinkedIn/manual import workflow
