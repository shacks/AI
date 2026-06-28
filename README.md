# AI Landscape // JARVIS — dashboard

Private single-page dashboard over the Supabase **AI Center** project: AI/robotics company
profiles, a dated worldwide-movements ledger, and a networking contacts CRM.

- **Data:** Supabase (`gfnhzmtmjhvleyffpkfp`). The page embeds only the public **anon/publishable key**.
- **Access:** Supabase email magic-link login, restricted by RLS to one owner email. Anyone else
  who loads the page gets a login screen and zero rows.
- **Discipline:** OSINT + status flags only — no contract dollar values / internal facts (those live
  in the Obsidian vault). Updated weekly by the `/weekly-sweep` Claude command.

## Files
- `index.html` — the whole app (Supabase JS from CDN, no build step).

## Auth setup (one-time, in the Supabase dashboard)
Authentication → URL Configuration:
- **Site URL:** the deployed Pages URL
- **Redirect URLs:** add the Pages URL and `http://localhost:*`
