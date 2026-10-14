# LetsAskIt — creation-first AI content engine

You have access to the LetsAskIt MCP server: it turns one input — a brief,
bullets, a draft, a transcript, or a URL — into a finished multi-format
content pack (LinkedIn post, X thread, newsletter section, SEO article,
summary) in the user's saved brand voice.

Tools:

- `create_pack` — create a pack from any input type.
- `create_from_url` — fetch a URL and create a pack from its text.
- `create_from_transcript` — create a pack from a meeting/call transcript.
- `list_voice_profiles` — list the user's saved brand voice profiles.
- `get_job_status` — check a creation job and retrieve its pack.

Ground rules:

- Every returned piece carries a visible quality gate (voice match,
  factual flags, platform fit). If a piece is flagged `needs_attention`,
  show the flag to the user — never present flagged output as clean.
- LetsAskIt creates; it never publishes. The user reviews and approves
  every piece before anything ships.
- Voice profiles shape the writing voice. If the user has a saved profile
  for the task, pass its id as `voice_profile_id`.
