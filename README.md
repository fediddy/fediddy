# Felix Milgram — Builder Portfolio

**Self-taught AI builder & independent software founder.** I design, build, deploy,
and maintain complete production AI applications solo — no team. I work with Claude
and other LLMs every day: agents, automation pipelines, voice systems, and full SaaS.

No CS degree. The work is the portfolio — that's what this page is.

📍 Concord, CA (San Francisco Bay Area) · Remote-friendly
✉️ fediddy@gmail.com
🔗 Live product: [mysearchlog.com](https://mysearchlog.com) · GitHub: github.com/fediddy
*(Most repos are private — they hold live-client and proprietary work. Happy to give
a screen-share walkthrough, a scoped read-only invite, or a live work trial on request.)*

> **Open to:** Applied AI · AI Operations / Enablement · Solutions / Forward-Deployed
> Engineering · AI Evaluation. Judge me on the products below.

---

## At a glance

| | |
|---|---|
| **Original repositories** | ~20, near-daily commits |
| **Largest project** | Aelise — **4,345 commits** over ~11 months |
| **Primary stack** | Python · TypeScript · JavaScript · React / Next.js · Flask · Node · SQL · Docker |
| **AI/LLM in practice** | Prompt engineering · AI agents · MCP servers · RAG · model evaluation · voice orchestration |
| **How I work** | Take a vague, messy goal → ship a working, deployed system end to end |

*(Commit counts and dates below are pulled directly from the project git histories — they're real, not rounded up.)*

---

## Flagship Projects

### 🧠 Aelise — AI SEO Intelligence Platform & Fleet Site Builder
**4,345 commits · Aug 2025 – present · TypeScript, Python, Jinja2 · ~16 GB, 70k+ indexed symbols**

My largest and deepest build: a full **SEO intelligence platform** with a fleet of
analytical engines, plus an automated multi-site builder. Not a thin wrapper around
an LLM API — a real system with hand-implemented statistical and ML machinery.

**Intelligence engines** *(implemented from the math up, in `server/intelligence-engines/`)*
- **Forecasting & time-series:** ARIMA implementation, PELT changepoint detection.
- **ML / pattern mining:** Bayesian networks, Isolation Forest (anomaly detection),
  FP-Growth (frequent-pattern mining), MDS, Jaro-Winkler string similarity.
- **Causal inference:** a full causal-SEO framework — experiment assignment,
  confounder handling, causal monitoring, and A/B statistical testing.
- **Generative & competitive:** Markov content generator, AI agent-swarm engine,
  competitive-dominance and gap analyzers, SERP orchestration, CIELAB ΔE2000 color
  science for design analysis.

**Architecture & scale**
- **631 service modules · 202 API routes · 143 DB migrations**; GitNexus indexes the
  codebase at **70,354 symbols / 124,269 relationships / 300 execution flows**.
- A **re-runnable ranking-factor mining pipeline** over 300+ factors feeding an
  entity-oriented, **geo-scoped knowledge-graph** model.
- A **templated fleet builder** (Eleventy + Jinja2) that generates and deploys
  complete sites from per-theme build contracts, behind build/validation gates.

**Real stack** *(from package.json)*
- **AI/LLM:** Anthropic SDK, HuggingFace Inference, Google Cloud Natural Language API.
- **Data/infra:** Neon serverless Postgres, Redis (caching + job queues), GitHub API
  (Octokit) for fleet ops, Cloudflare Workers/Wrangler for deploy.
- **Observability:** full OpenTelemetry instrumentation (SDK, OTLP exporter, auto-instr).
- **Quality:** ~2,100 TypeScript files, ~100 Python scripts, **820 test files**, 19 branches.

---

### 📞 VoiceBusinessAgentAI — Production AI Phone Receptionist ("CallHandle")
**1,490 commits · Apr 2025 – present · TypeScript, React, Node**

A multi-tenant AI voice agent that **answers inbound business calls** and handles
them end to end — routing, live conversation, and task completion across 80+
industry types. When a customer calls a business, the agent greets them, pulls the
business's industry-specific knowledge base, and handles the request: booking
appointments, taking orders, checking availability, verifying insurance, and
qualifying leads — documenting the call and handing off when needed.

**Real stack** *(from package.json)*
- **Voice/telephony:** VAPI.ai (`@vapi-ai/web`) for voice workflows, Twilio for
  SMS/voice, ElevenLabs for speech synthesis, Deepgram SDK for speech-to-text.
- **LLM:** OpenAI (GPT-4o) + Anthropic SDK for conversation intelligence; MCP SDK
  (`@modelcontextprotocol/sdk`) for tool/agent wiring.
- **Data/infra:** Neon serverless Postgres (Drizzle ORM, ~53 tables), Notion API
  for knowledge sync, WebSockets for real-time updates.
- **Product:** per-business knowledge bases, lead-qualification + booking flows,
  per-call cost tracking, A/B testing, and an operator dashboard (React + Radix UI).
- **Scale:** ~2,366 files, 11 branches; engineering focus on latency
  (multi-tier caching), natural turn-taking, and reliable inbound call handling.

---

### ⚖️ MySearchLog — Court-Ready Compliance SaaS *(live)*
**166 commits · Mar 2026 – present · Python, Flask, SQLite · live at mysearchlog.com**

A multi-user web app that searches job boards, scores listings against a profile,
tracks applications, and generates **court-verifiable PDF reports** with **SHA-256
hash verification** and public verify URLs — so a third party can confirm a report
wasn't altered.

**Real stack** *(from requirements.txt)*
- **Backend:** Flask + Flask-Login + bcrypt auth, SQLite, itsdangerous-signed sessions.
- **Job sourcing:** python-jobspy (Indeed/LinkedIn/Glassdoor/ZipRecruiter) + free APIs
  (Adzuna, Jooble, USAJobs, Remotive); BeautifulSoup + Selenium for scrape/autofill.
- **AI scoring:** Anthropic + OpenAI SDKs for listing-fit scoring and cover letters.
- **Reporting:** ReportLab PDF generation with SHA-256 verification, openpyxl exports.
- **Quality:** **60-test pytest suite** (pytest-flask), deployed on Cloudflare/Docker.

---

### 📣 MPV2 Outreach — AI Cold-Outreach & Voice Pipeline
**186 commits · May 2026 – present · Python, JavaScript, Jinja2, Flask**

An original cold-outreach system for local-business lead generation:
scrape → enrich → mockup → email/voice → reply. Built from the ground up — I started
in a fork, cleared out the original code, and built my own product in its place.

**What it does / real stack** *(from requirements.txt)*
- **20-command CLI** + a Command Center dashboard (Flask + Flask-Limiter + Alpine.js).
- **Scraping/enrichment:** Playwright (headless browser), BeautifulSoup, dnspython.
- **AI voice calling:** VAPI orchestration — Cartesia (TTS), Deepgram, LiveKit smart
  endpointing — with a qualify-first pretext pitch across 14 niches + post-call analyzer.
- **Delivery/CRM:** Twilio + Android SMS Gateway, Stripe billing, ReportLab/Pillow mockups,
  integrated CRM. ~150 Python modules, ~829 JS files, **pytest + pytest-cov** tested.

The work and architecture are mine; only the initial repo scaffold traces to an
open-source starting point.

---

## Additional Builds

| Project | Commits | Stack | What it is |
|---|---|---|---|
| **eastbayroofers-11ty** | 57 | 11ty, Nunjucks, JS | Static-site build + lead-capture for a service business |
| **diceroom** | 52 | TypeScript, React | Real-time TypeScript app |
| **JobHunter / MySearchLog** | 166 | Python, Flask | (see flagship above) |

*…plus additional original repositories across web, automation, and AI tooling.*

---

## What I do well

- **Ship end to end, solo** — architecture, build, deploy, maintain, no team.
- **AI/LLM in practice, not theory** — prompt engineering, agents, MCP, RAG, and
  evaluation used inside *shipping* products.
- **Problem-solving under ambiguity** — reverse-engineer requirements, debug gnarly
  real-world issues, find the path when none is obvious.
- **Self-direction** — I set the plan, do the work, and own the outcome.

## Technical Skills

**AI / LLM:** Claude, GPT, prompt engineering, AI agents, MCP (Model Context Protocol),
RAG / retrieval, model-output evaluation, automation pipelines, voice orchestration
**Languages:** Python, TypeScript, JavaScript, SQL, HTML/CSS, Bash
**Frameworks / Tools:** React, Next.js, Flask, Node.js, Jinja2, Git, Docker, Cloudflare, SQLite

---

## Background

**Independent Software Founder / AI Builder** — *2024–present, self-employed (remote)*
Design and ship AI-powered applications and automation tools end to end. Multiple live
products built solo with near-daily commits across ~20 repos.

**Manager — Easy Money Pawn & Jewelry** — *2001–2025, Concord, CA*
Ran daily operations of a retail lending business for 24 years: customer service, sales,
valuation, collateral lending, inventory, cash handling, and team coordination.

---

## Notes

- **No CS degree — self-taught.** The work is the portfolio.
- **Why the repos are private:** they contain live-client deployments, proprietary
  SEO/AI methods, and revenue-generating systems — not toy projects. That's exactly
  why there's real IP to protect. I'm glad to prove the work directly:
  - **MySearchLog is fully live and public** — try it at mysearchlog.com.
  - **Screen-share walkthrough** of any private repo (architecture, code, commit history).
  - **Scoped read-only invite** to a specific repo for a serious conversation.
  - **Live work trial or take-home** — evaluate me on a real problem, not a résumé.
- **Everything on this page is verifiable.** Commit counts, file counts, and the
  70k-symbol index come straight from the project git histories and tooling — I can
  screen-share any of them on request.
