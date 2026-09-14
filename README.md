# The Playoff Pickoff

A mobile-first, three-player NFL prediction competition for the 2026 season. Picks are persisted in Supabase and live NFL standings are synchronized hourly by a Netlify Function.

## Scoring

- Division winner: 3 points (1 if selected team makes the playoffs as a wild card)
- Wild card: 3 points (1 if selected team wins its division)
- Conference finalist: 3 points per team
- Super Bowl participant: 5 points per team
- Super Bowl champion: 5 bonus points
- Perfect total: 69 points

## Local development

Run `npm install`, then `npx netlify dev`. The sync function requires `SUPABASE_URL`, `SUPABASE_KEY`, and `NFL_SYNC_SECRET` environment variables.
