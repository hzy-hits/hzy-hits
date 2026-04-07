# Zhenyu Huang

Systems engineer building infrastructure that makes AI agents reliable in production — evaluation frameworks, constrained action spaces, orchestration, and deterministic testing.

Brown University M.Sc. (Computational Science) + Sun Yat-sen University B.Sc. (Physics). Based in Hong Kong.

## Featured Projects

### [QuantStack](https://github.com/hzy-hits/QuantStack) — Quantitative Research Platform
Production platform covering ~748 US equities (2x daily) and 300+ Chinese A-shares. 15 analytics modules with a Bayesian probability framework, async Rust data ingestion from 8 APIs, and 4 parallel Claude API analyst agents for automated report synthesis. AI explores the strategy space; the system validates.

`Python` `Rust` `DuckDB` `Claude API`

### [QuantfactorLab](https://github.com/hzy-hits/QuantfactorLab) — AI-Driven Factor Discovery
LLM agents propose alpha factors in a constrained expression language. Walk-forward backtesting with multi-gate anti-overfit validation. Agent never sees out-of-sample metrics — only binary pass/fail. Bootstrap significance testing with GPU acceleration. Auto-retirement on performance decay.

`Python` `DuckDB`

### [IvenaMeet](https://github.com/hzy-hits/IvenaMeet) — Private Streaming Platform
Production self-hosted video platform. Rust control plane with 30 API endpoints: auth, session management, invite lifecycle, broadcast orchestration, real-time chat, and an agent API for programmatic room control.

`Rust (Axum)` `React` `LiveKit` `Redis` `SQLite`

### [codex-par](https://github.com/hzy-hits/codex-par) — Parallel AI Agent Orchestration
Runs multiple Codex tasks in parallel, solving MCP serialization and deadlock. Dependency-based wave scheduling, live TUI dashboard, and MCP server with 14 tools for dynamic dispatch.

`Rust` `Tokio` `MCP`

### [voice2blog](https://github.com/hzy-hits/voice2blog) — Speech to Markdown
Rust CLI that records technical speech, transcribes via Whisper, and generates structured Markdown with code blocks and headings.

`Rust`
