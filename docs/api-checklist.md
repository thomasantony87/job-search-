# API Checklist

## Already Connected

- Supabase project: `job search engine`
- Supabase project ID: `hvghhwnssvngoeqnzusw`
- GitHub repo read access: `thomasantony87/job-search-`
- Vercel team: `Thomas' projects`

## Still Needed

### GitHub

Codex can read repo metadata, but GitHub write access is blocked by the integration.

Required action:

- Authorize the GitHub app/connector for `thomasantony87/job-search-`
- Or install Git locally so code can be pushed from this machine

### Supabase

Add these to Vercel environment variables:

```env
NEXT_PUBLIC_SUPABASE_URL=https://hvghhwnssvngoeqnzusw.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=
SUPABASE_SERVICE_ROLE_KEY=
```

Use the service role key only on the server.

Status:

- Project URL confirmed
- Publishable key received, not committed
- Secret key received, not committed

### Vercel

The Vercel connector sees the team, but no project is listed yet.

Required action:

- Confirm the Vercel project is under `Thomas' projects`
- Connect it to `thomasantony87/job-search-`
- Add Supabase environment variables in Vercel

## Later APIs

- OpenAI API for profile analysis, matching, summaries, and drafts
- Gmail API or Gmail connector for outreach tracking
- Google Calendar for interview/follow-up reminders
- Search API such as Tavily or SerpAPI for broader opportunity discovery
