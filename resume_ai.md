# Zhenyu Huang (黄振宇)

huangzhy77@outlook.com | +86 13502448752 | [github.com/hzy-hits](https://github.com/hzy-hits) | Hong Kong | Top Talent Pass holder | Available immediately

---

> AI infrastructure engineer building reliable agent systems: deterministic testing, evaluation pipelines, constrained action spaces, and multi-agent orchestration.

## Experience

**Meituan** — Software Engineer, Core Local Commerce \hfill Jul 2025 – Present
- Designed a zero-intrusion proxy for LLM agent testing: intercepted model API domains via AOP and redirected traffic to a mock server, enabling deterministic validation of tool-calling behavior without modifying product code
- Built an LLM-as-Judge evaluation pipeline for insurance and local-services workflows, scoring agent outputs against structured rubrics through internal LLM APIs
- Automated regression checks for AI-driven workflows, reducing behavioral drift risk across prompt, model, and toolchain changes

## Selected Projects

**Light Orchestra (codex-par)** — Parallel AI Coding Agent Orchestrator \hfill Rust | 8,000+ LOC
- Built a Rust task runner that bypasses MCP serialization by spawning isolated `codex exec --json` processes, cutting multi-task agent workflows from serial execution into dependency-wave parallelism
- Solved MCP half-duplex deadlock with process-group isolation and graceful multi-stage shutdown, ensuring no zombie processes or orphaned agent workers
- Exposed a 14-tool MCP server for dynamic dispatch, shared facts, live progress monitoring, and chunked output/stderr reads for Claude-driven orchestration

**QuantfactorLab** — Agent Evaluation System for Alpha Research \hfill Python | 10,000+ LOC
- Designed a constrained factor DSL so LLM agents can only propose formulas within a bounded action space: ~35 operators, expression length and depth limits, whitelisted lookback windows
- Implemented hidden-holdout evaluation where agents never see out-of-sample metrics and receive only binary PASS/FAIL feedback, preventing reverse-engineering of the test set
- Added a 5-gate anti-overfit pipeline with bootstrap significance testing and automatic factor retirement on performance decay

**QuantStack** — Multi-Agent Research Platform \hfill Python, Rust | 40,000+ LOC
- Orchestrated 4 parallel Claude API analyst agents that synthesize daily research reports from pre-computed analytics across ~748 US equities and 300+ Chinese A-shares
- Kept agents strictly narrational: the validation layer computes all numbers, and agents are only allowed to summarize facts rather than mutate outputs
- Unified the platform around explicit probability outputs, Bayesian updating, and regime detection so agent-generated commentary stays grounded in auditable model outputs

**IvenaMeet** — Agent-Native Control Plane \hfill Rust, React, LiveKit | 18,000+ LOC
- Shipped an agent API layer (`/agent/v1/context|events|commands`) for room-state retrieval, event streaming, and idempotent command execution with `simulate|execute` modes
- Designed low-risk command patterns such as `refresh_session`, `send_message`, and `issue_invite`, making the system safe to operate programmatically

## Education

**Brown University** — M.Sc. Computational Science, GPA 3.6/4.0 \hfill Sep 2023 – Jun 2025
- Built a TCP/IP network stack in Rust and a Weenix OS kernel in C

**Sun Yat-sen University** — B.Sc. Physics, GPA 3.7/4.0 \hfill Sep 2019 – Jun 2023

## Skills

**AI Infrastructure:** agent orchestration, deterministic agent testing, LLM-as-Judge, hidden-holdout evaluation, constrained action spaces, MCP protocol
**Languages:** Rust, Python, TypeScript, SQL
**Systems:** Tokio, Axum, Redis, DuckDB, SQLite, process isolation, systemd
**LLM Integration:** Anthropic SDK, evaluation pipeline design, multi-agent orchestration
