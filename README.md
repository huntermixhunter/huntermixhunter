# Hunter Mix

**AI systems and automation builder.** I direct AI coding agents to design, test, and ship real software, then I keep it running.

Based in Sandpoint, Idaho. Remote. Founder of [Magimatix](https://magimatix.com), where I build custom AI tooling, workflow automation, and production websites for small businesses.

Open to remote AI and automation work.

**How I build:** I do not write the code myself. I write the requirements, direct AI coding agents (Claude Code and Codex), review and test what comes back, and ship it. Everything below was built that way, and the code is public so you can judge it.

---

## Things I have shipped

### [D.A.T.A](https://github.com/huntermixhunter/D.A.T.A) &nbsp;·&nbsp; `Python` `JavaScript`
A self-hosted, local-first AI operations dashboard, packaged and shipped as a desktop product that anyone can download and install. Free and open source under Apache 2.0, with an optional name-your-price tip.

- **About 50,000 lines** of first-party Python and JavaScript, written by AI coding agents under my direction, across **150+ commits**, with **280+ Python tests**
- A single service layer exposing **120+ HTTP endpoints**, backed by a persistent agent with **40+ tools**
- **10 specialist subagents**, persistent cross-session memory with **hybrid search** (SQLite FTS5 plus local embeddings, merged with reciprocal rank fusion), and scheduled jobs
- **A human gate on the agent's own work.** A scheduled job implements a dashboard improvement on a separate branch, runs the checks, and opens a pull request. It never merges its own work, so nothing it writes ships without human approval. 38 opened, 7 merged after human review, [31 waiting for review](https://github.com/huntermixhunter/D.A.T.A/blob/main/AUTONOMOUS_BUILD_LOOP.md)
- Browser control over the Chrome DevTools Protocol, desktop control, and MCP server integration
- Release pipeline: Windows installer built locally, Intel and Apple Silicon macOS DMGs built on GitHub-hosted runners, SHA-256 checksums published, and private configuration structurally excluded from the distributable
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

### Client work
Production sites I built and maintain, including [dusk2dawnlighting.com](https://dusk2dawnlighting.com) and [truesumbookkeeping.com](https://truesumbookkeeping.com).

---

## What the projects are built with

The code is written by AI coding agents under my direction. I am listing the stack so you know what you are reading, not as a claim that I type it.

**Languages in the repos** &nbsp; Python · JavaScript · TypeScript · SQL · Bash · PowerShell · HTML/CSS

**AI and agents** &nbsp; Multi-agent orchestration · tool and function calling · MCP servers · retrieval and persistent memory · Claude, OpenAI and Gemini APIs · local models via Ollama

**Automation** &nbsp; scheduled jobs · OAuth integrations · REST APIs · browser automation (Chrome DevTools Protocol, Playwright)

**Infrastructure** &nbsp; Linux VPS (DigitalOcean) · Vercel · Next.js · Git and GitHub Actions · Cloudflare · SQLite

**Tools I direct** &nbsp; Claude Code · Codex

---

## Reach me

[magimatix.com](https://magimatix.com) &nbsp;·&nbsp; hunterthomasmix@gmail.com
