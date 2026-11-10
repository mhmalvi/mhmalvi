# Muhammad H.M. Alvi

**AI engineer. I build and run production LLM systems, browser automation and the infrastructure under them.**

Founding AI Engineer at [Aethon Automation Solutions](https://aethonautomation.com). I've worked in tech for 15+ years. Today my work is hands-on engineering: routing LLM calls between local and cloud models, agents with human approval gates, unattended browser automation over the Chrome DevTools Protocol, Postgres job queues, and a self-hosted server that recovers on its own after a power cut. Based in Dhaka, Bangladesh. Open to remote roles.

📫 info@aethonautomation.com · [LinkedIn](https://www.linkedin.com/in/mdhmalvi) · [muhammadhmalvi.com](https://muhammadhmalvi.com)

---

## Flagship projects

| Project | What it is | Stack |
|---|---|---|
| [**Nexus-AIOS**](https://github.com/mhmalvi/Nexus-AIOS) | An AI operating-system shell. The agent streams tool calls into a human-in-the-loop approval gate. It works with any OpenAI-compatible model provider, and the API key stays on the server. | TypeScript · React · Vite · Node · Vitest |
| [**aethon-ai-router**](https://github.com/mhmalvi/aethon-ai-router) | A local-first LLM routing layer used by every pipeline on the server. Each task class goes to local Ollama or to cloud models through a LiteLLM gateway. Employer-facing text fails closed, and every call lands in a shared cost ledger. | Python · LiteLLM · Ollama · OpenRouter · SQLite |
| [**apex-job-engine**](https://github.com/mhmalvi/apex-job-engine) | An autonomous job discovery and application engine. It has pluggable sources, deterministic gates, résumé tailoring with a provenance guard, and a raw-CDP browser lane. An application only counts as sent when there is proof it was submitted. | Python · CDP · Chrome MV3 · SQLite · systemd |
| [**epic-ai-email**](https://github.com/mhmalvi/epic-ai-email) | An AI email assistant SaaS on self-hosted Supabase. A triage gate runs before the LLM, an LLM drafts replies, and campaign sending has a bounce circuit breaker and sender pinning. | TypeScript · Supabase · Deno · Postgres |
| [**media-pipeline-engine**](https://github.com/mhmalvi/media-pipeline-engine) | Media pipelines built on a Postgres job queue. Claims are fact-checked before a video is rendered. Providers are routed by capability behind circuit breakers, and clips are reframed to 9:16 by tracking faces. | Python · PostgreSQL · ffmpeg · Blender · OpenCV |
| [**self-hosted-ai-infra**](https://github.com/mhmalvi/self-hosted-ai-infra) | A single-server Docker estate behind Cloudflare Tunnel and Caddy. Backups are encrypted and the offsite upload can resume. The server recovers from power cuts, the crontab repairs itself, and disaster recovery runs in phases. | Docker · Caddy · systemd · Bash · rclone |
| [**detached-build-driver**](https://github.com/mhmalvi/detached-build-driver) | Builds software phase by phase with headless coding agents. A phase only counts with a new commit and a passing test suite. It pauses when usage quotas run out, and its state survives a power cut. | Bash · Python · git · cron |

Each showcase README covers the problem, the architecture, the hard engineering decisions and the evidence. It also includes sanitized code excerpts with their own tests. The production source is private.

## Stack

- **Languages:** Python, TypeScript, JavaScript, SQL (PostgreSQL), Bash
- **AI / LLM:** LLM application engineering (Claude, OpenRouter, Gemini APIs; OpenAI-compatible endpoints), LiteLLM, Ollama, RAG, multi-agent systems, LLM evaluation and quality gates, MCP servers, PyTorch / Hugging Face fine-tuning, speech (faster-whisper, Kokoro TTS)
- **Backend & data:** FastAPI, PostgreSQL (SKIP LOCKED job queues), Supabase (RLS, pg_cron, Edge Functions), SQLite (WAL, FTS), Redis, REST and webhooks, gRPC, Google Workspace APIs, Telegram Bot API
- **Automation:** Chrome DevTools Protocol, Playwright, Selenium, Chrome MV3 extensions, n8n, ATS integrations (Greenhouse, Ashby, Lever, Workday, Workable)
- **Frontend:** React, Next.js, Vite, Tailwind / shadcn, TanStack Query
- **Infra:** Docker & Compose, Linux (Ubuntu), systemd services and timers, Caddy, Cloudflare Tunnel, Tailscale, rclone + GnuPG backups, Uptime Kuma, Langfuse
- **Media:** ffmpeg (NVENC, RTMP), Blender (headless bpy), OpenCV
- **Testing:** pytest (test-first), Vitest, Deno.test

## How I work

- I test first, and I don't count work as done until there is evidence: a passing suite, a commit, a log line.
- Gates fail closed. An outage should show up as an alert, not look like a quiet day.
- I run what I build, on my own server, with systemd timers, ledgers and health checks.

## Earlier work

Before 2025 I delivered LMS, CRM and web platforms for training-sector and business clients, including a microservice CRM (leads, users, orgs, payments, notifications, chat, file and mail services). Some of that client-delivery code is public on this profile, for example [nexus-crm-client](https://github.com/mhmalvi/nexus-crm-client) and [nexus-crm-leads](https://github.com/mhmalvi/nexus-crm-leads).
