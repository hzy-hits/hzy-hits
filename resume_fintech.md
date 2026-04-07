# Zhenyu Huang (黄振宇)

huangzhy77@outlook.com | +86 13502448752 | [github.com/hzy-hits](https://github.com/hzy-hits) | Hong Kong | Top Talent Pass holder | Available immediately

---

> Systems engineer building production Rust and Python platforms: real-time control planes, financial data infrastructure, and operationally reliable backend services.

## Experience

**Meituan** — Software Engineer, Core Local Commerce \hfill Jul 2025 – Present
- Designed a zero-intrusion proxy for LLM agent testing, intercepting model API traffic and redirecting it to a mock server for deterministic validation without business-code changes
- Built an LLM-as-Judge evaluation framework for large-scale quality assessment of AI-generated outputs

## Selected Projects

**IvenaMeet** — Private Streaming Platform \hfill Rust (Axum), React, LiveKit | 18,000+ LOC
- Built a production-style WebRTC control plane with 30 HTTP endpoints covering room join, host auth, session refresh, invite lifecycle, moderation, broadcast orchestration, chat, and profile management
- Implemented distributed state and security controls with Redis Lua scripts, TOTP host authentication, invite-redeem atomicity, and six scoped token types with TTL-based rotation
- Added per-operation rate limiting and safe lifecycle checks for high-risk actions such as broadcast start, plus durable chat persistence with retry-safe message writes
- Deployed the system with systemd services, cron-based maintenance, reverse-proxy topology, and an avatar upload pipeline with validation and server-side transcoding

**QuantStack** — Financial Data and Analytics Platform \hfill Python, Rust | 40,000+ LOC
- Built a dual-market financial data platform covering ~748 US equities and 300+ Chinese A-shares, with scheduled reporting pipelines and DuckDB-backed storage
- Wrote an async Rust fetcher integrating 8 external APIs with rate limits, backoff, and persistence into 15+ tables per pipeline
- Implemented analytics modules for momentum, volatility, macro, options, flow, and event-driven research, then packaged outputs into automated daily analyst-style reports

**Hyperliquid Trading** — DEX Trading Scaffold \hfill Python
- Built automated trading scaffold connecting to Hyperliquid's decentralized derivatives exchange API with order management and position tracking on on-chain order books

**Light Orchestra (codex-par)** — Process-Isolated Task Runner \hfill Rust | 8,000+ LOC
- Built a parallel task runner that launches isolated workers and schedules them into dependency waves, with a live dashboard and MCP server for non-blocking dispatch

## Education

**Brown University** — M.Sc. Computational Science, GPA 3.6/4.0 \hfill Sep 2023 – Jun 2025
- Built a TCP/IP network stack in Rust and a Weenix OS kernel in C

**Sun Yat-sen University** — B.Sc. Physics, GPA 3.7/4.0 \hfill Sep 2019 – Jun 2023

## Skills

**Languages:** Rust, Python, TypeScript, SQL
**Backend & Systems:** Tokio, Axum, Redis, SQLite, DuckDB, systemd, process isolation
**Fintech/Data:** exchange and DEX API integration, market data pipelines, DuckDB OLAP, automated reporting
**AI Integration:** Anthropic SDK, LLM evaluation frameworks, agent orchestration
