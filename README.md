# Hunter Mix

**AI systems and automation engineer.** I build agent infrastructure that runs unattended, then I ship it and keep it running.

Based in Sandpoint, Idaho. Remote. Founder of [Magimatix](https://magimatix.com), where I build custom AI tooling, workflow automation, and production websites for small businesses.

Open to remote AI and automation engineering work.

---

## Things I have shipped

### [D.A.T.A](https://github.com/huntermixhunter/D.A.T.A) &nbsp;·&nbsp; `Python` `JavaScript`
A self-hosted, local-first AI operations dashboard, packaged and shipped as a real desktop product people download and install. Free and open source under Apache 2.0, with a name-your-price checkout.

- **92,000+ lines** across 150 commits: 53k Python, 20k JavaScript, plus the front end
- A single service layer exposing **120+ HTTP endpoints**, backed by a persistent agent with a large tool surface
- **Specialist subagents**, persistent cross-session memory with full-text search, and cron-scheduled autonomous jobs
- **The agent ships features to itself.** A scheduled job implements a dashboard improvement on its own branch, runs the checks, and opens a pull request. It never self-merges. 38 opened, 7 merged after human review, [31 queued at the gate by design](https://github.com/huntermixhunter/D.A.T.A/blob/main/AUTONOMOUS_BUILD_LOOP.md)
- Browser control over the Chrome DevTools Protocol, desktop control, and MCP server integration
- Cross-platform release pipeline: Windows installer and macOS DMGs built on hosted runners, with private configuration structurally excluded from the distributable
- Runs entirely on the user's machine. No account required, no telemetry

### [autocut](https://github.com/huntermixhunter/autocut) &nbsp;·&nbsp; `Python` `FFmpeg`
A local-first pipeline that turns long-form video into captioned vertical clips, with no paid API anywhere in the loop. It transcribes audio locally, scores sentence-aligned windows, picks passages that stand on their own, and renders them as 1080x1920 MP4s with synchronized word captions.

- Runs entirely on local hardware: `faster-whisper` for transcription, FFmpeg for rendering. No API keys, no accounts, no per-minute billing
- Every stage writes a durable artifact, so any stage can be re-run, inspected or hand-edited without repeating the one before it
- Selection is rule-based and transparent on purpose. The headline is not allowed to borrow a stronger claim from later in the clip, and it returns fewer clips rather than weaker ones
- 20 tests and 10 subtests covering render output, caption timing, source boundaries and packaging

### [magimatix.com](https://github.com/huntermixhunter/magimatix-site) &nbsp;·&nbsp; `TypeScript` `Next.js` `Stripe`
The production site and digital storefront for my studio. Not a brochure template: a marketing site and a working one-time-purchase storefront in the same application, with payment, delivery and transactional email wired end to end.

- Live: **[magimatix.com](https://magimatix.com)**
- Next.js 16 App Router, React 19, TypeScript and Tailwind 4 on Vercel, across 100 commits
- Stripe embedded checkout, with a webhook that verifies the Stripe signature before trusting any payload, then records the sale and triggers fulfilment
- Release assets sit behind a stable redirect, so download links emailed months ago still resolve when a new version ships
- Markdown blog with generated hero images, dynamic Open Graph images, and sitemap and robots generated at build time

### [Curve Lab](https://github.com/huntermixhunter/curvelab) &nbsp;·&nbsp; `TypeScript` `Next.js`
Simulate and compare Meteora Dynamic Bonding Curves before launching on one, with verified mainnet replays.

- Live: **[curvelab-lake.vercel.app](https://curvelab-lake.vercel.app)**
- Next.js and TypeScript, deployed on Vercel, with a Vitest suite covering simulation, mainnet replay, integrity and preset-catalog logic
- Replays a curve against a demand flow and surfaces the tradeoff operators currently cannot see: graduation point, fees earned, and demand that arrives after graduation and never touches the curve

### Client work
Production sites I built and maintain, including [dusk2dawnlighting.com](https://dusk2dawnlighting.com) and [truesumbookkeeping.com](https://truesumbookkeeping.com).

---

## Stack

**Languages** &nbsp; Python · JavaScript · TypeScript · SQL · Bash · PowerShell · HTML/CSS

**AI and agents** &nbsp; Multi-agent orchestration · tool and function calling · MCP servers · retrieval and persistent memory · prompt engineering · Claude, OpenAI and Gemini APIs · local models via Ollama

**Automation** &nbsp; n8n · cron and scheduled jobs · OAuth integrations · REST API design · browser automation (Chrome DevTools Protocol, Playwright)

**Infrastructure** &nbsp; Linux VPS (DigitalOcean) · Vercel · Next.js · Docker · Git and GitHub Actions · Cloudflare · SQLite · Postgres

**Tools I build with** &nbsp; Claude Code · Codex · Cursor

---

## Reach me

[magimatix.com](https://magimatix.com) &nbsp;·&nbsp; hunterthomasmix@gmail.com
