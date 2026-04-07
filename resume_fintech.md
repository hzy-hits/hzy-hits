# Zhenyu Huang (黄振宇)

huangzhy77@outlook.com | +86 13502448752 | [github.com/hzy-hits](https://github.com/hzy-hits) | Hong Kong | Top Talent Pass holder | Available immediately

---

I ship production Rust services. My streaming platform has 30 endpoints, full auth, and runs daily. My data platform pulls from 8 financial APIs across two markets. I build systems that work, stay up, and handle real users.

## Experience

**Meituan** — Software Engineer, Core Local Commerce \hfill Jul 2025 – Present
- Transparent proxy for deterministic LLM agent testing — intercepts API calls, reroutes to mock server, no product code changes
- LLM-as-Judge pipeline for automated quality scoring of agent outputs at scale

## Selected Engineering Work

**IvenaMeet** — Private Streaming Platform [Production] \hfill Rust (Axum), React, LiveKit
- Self-hosted video platform, 30 HTTP endpoints. Full auth lifecycle: TOTP login, 6 token types with TTL rotation, invite-redeem with atomic Redis Lua scripts, per-operation rate limiting. 81 commits, daily use
- Agent API lets AI operators observe room state, execute commands, dry-run actions before committing. Deployed with systemd, cron cleanup, reverse proxy

**QuantStack** — Financial Data Platform [Production] \hfill Python, Rust
- ~748 US equities and 300+ A-shares. Async Rust fetcher integrating 8 financial APIs into DuckDB with rate limiting, retries, idempotent scheduling
- 15 analytics modules producing daily probability reports. 4 parallel LLM analysts synthesize output, delivered before market open

**Hyperliquid Trading** \hfill Python
- Trading scaffold on Hyperliquid DEX — API integration, order management, position tracking against on-chain order books

**codex-par** — Parallel Task Runner [Tool] \hfill Rust
- Parallel runner for AI coding agent tasks — dependency-wave scheduling instead of serial execution. 90-minute workflows finish in 30

## Education

**Brown University** — M.Sc. Computational Science, GPA 3.6/4.0 \hfill Sep 2023 – Jun 2025
- TCP/IP network stack in Rust, OS kernel in C — systems programming from scratch

**Sun Yat-sen University** — B.Sc. Physics, GPA 3.7/4.0 \hfill Sep 2019 – Jun 2023

## Skills

Rust, Python, TypeScript, SQL | Axum, Redis, DuckDB, LiveKit/WebRTC, systemd | Anthropic SDK
