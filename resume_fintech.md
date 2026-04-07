# Zhenyu Huang (黄振宇)

huangzhy77@outlook.com | +86 13502448752 | [github.com/hzy-hits](https://github.com/hzy-hits) | Hong Kong | Top Talent Pass holder | Available immediately

---

I ship production Rust services that keep their invariants under concurrency, external APIs, and real users. A streaming control plane with full auth and broadcast lifecycle. A dual-market financial data platform pulling 8 APIs on a daily schedule. Both in production, both mine.

## Experience

**Meituan** — Software Engineer, Core Local Commerce \hfill Jul 2025 – Present
- Agent workflows were impossible to test without changing product code. I intercepted model API traffic and rerouted it to a mock server, making tool-calling deterministic under live business flows
- Manual QA couldn't scale with agent iteration speed. I replaced it with an LLM-as-Judge pipeline for automated output scoring

## Selected Engineering Work

**IvenaMeet** — Private Streaming Platform [Production] \hfill Rust (Axum), React, LiveKit
- Real-time room state breaks easily under joins, retries, and privilege changes. I wrote a Rust control plane with 30 HTTP endpoints covering room lifecycle, broadcast orchestration, durable chat, and profile management
- Broadcast and invite flows are security problems as much as API problems. TOTP host login, scoped token rotation, Redis Lua-backed invite redemption, and per-route rate limits keep state consistent under concurrent actions
- To make the platform operable instead of demo-only: agent API with dry-run semantics, systemd deployment, cron maintenance, reverse proxy topology, validated avatar upload pipeline

**QuantStack** — Financial Data Platform [Production] \hfill Python, Rust
- Daily dual-market reporting means 8 external APIs, rate limits, and schema drift can break freshness at any point. Async Rust fetcher with pacing, retries, and idempotent DuckDB persistence across ~748 US equities and 300+ A-shares
- 15 analytics modules turn raw data into daily probability reports. 4 parallel LLM analysts synthesize the output — constrained to summarize pre-computed facts. Delivered before market open

**Hyperliquid Trading** \hfill Python
- Trading scaffold on Hyperliquid DEX — API integration, order management, position tracking against on-chain order books

**codex-par** — Parallel Task Runner [Tool] \hfill Rust
- MCP-based multi-agent work serialized and stalled. Dependency-wave scheduling with process isolation, live dashboard, and runtime dispatch. 90-minute workflows → 30

## Education

**Brown University** — M.Sc. Computational Science, GPA 3.6/4.0 \hfill Sep 2023 – Jun 2025
- TCP/IP network stack in Rust, OS kernel in C — systems programming from scratch

**Sun Yat-sen University** — B.Sc. Physics, GPA 3.7/4.0 \hfill Sep 2019 – Jun 2023

## Skills

Rust, Python, TypeScript, SQL | Axum, Tokio, Redis, SQLite, DuckDB, LiveKit/WebRTC, systemd | Anthropic SDK
