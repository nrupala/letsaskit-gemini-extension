# LetsAskIt, for Gemini CLI

A [Gemini CLI](https://geminicli.com) extension that wires the hosted
**LetsAskIt** MCP server into your terminal.

LetsAskIt is a creation-first AI content engine. You bring a spark — a
topic, brief, bullets, draft, transcript, or URL — and it returns finished
content for every platform that matters: LinkedIn posts, X threads,
newsletter sections, SEO articles, and summaries, all in your saved brand
voice. Every piece carries a visible quality gate (voice match, factual
flags, platform fit), and nothing publishes itself — a human reviews
before anything ships. Five tools: `create_pack`, `create_from_url`,
`create_from_transcript`, `list_voice_profiles`, `get_job_status`.

## Install

```bash
gemini extensions install https://github.com/nrupala/letsaskit-gemini-extension
```

On install, Gemini CLI prompts for your **LetsAskIt API key** (stored as
`LETSASKIT_API_KEY`). MCP access is a **Team-plan** feature — get a key
from the LetsAskIt operator (Team plan, $79/mo: 2,500 jobs/mo, 15 voice
profiles, REST + MCP). The free Studio tier is web-only, no key needed:
[letsaskit.com/studio](https://letsaskit.com/studio).

## What this repo is

This is a thin wrapper: it contains no server code. The extension manifest
(`gemini-extension.json`) points Gemini CLI at the hosted LetsAskIt MCP
server (`https://letsaskit.com/mcp`, Streamable HTTP, stateless) and sends
your key as an `Authorization: Bearer <key>` header on each call.

- Documentation: https://letsaskit.com/docs/mcp-setup.html
- Privacy policy: https://letsaskit.com/privacy/
- Terms: https://letsaskit.com/terms/
- Support: info@aimlds.org

## License

Apache-2.0. See `LICENSE`.

---
LetsAskIt is a product of 2351485 ALBERTA INC. · Built with Muse by Meta
