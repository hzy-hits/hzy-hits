# Zhenyu Huang (黄振宇)

huangzhy77@outlook.com | +86 13502448752 | [github.com/hzy-hits](https://github.com/hzy-hits) | Hong Kong | Top Talent Pass holder | Available immediately

---

I design systems where AI agents do useful work: I give them deterministic tools and clear boundaries, and they find the answers. At Meituan I make agents testable. In my quant platform I constrain and orchestrate them. In my factor lab I evaluate them with hidden holdouts they can't game. Every project is the same pattern.

## Experience

**Meituan** — Software Engineer, Core Local Commerce \hfill Jul 2025 – Present
- Transparent proxy intercepts LLM agent API calls via AOP and reroutes to a mock server. The mock is the deterministic tool; "don't touch product code" is the boundary. Agent tool-calling becomes reproducible and testable
- LLM-as-Judge: LLM scores agent outputs against structured rubrics across insurance and life-service workflows. AI evaluating AI — automated replacement for manual review
- Regression testing for AI workflows — catches behavioral drift across prompt, model, and toolchain changes

## Selected Engineering Work

**QuantfactorLab** — Agent Evaluation System [Research] \hfill Python
- The clearest instance of the pattern: LLM agents explore inside a constrained expression language (~35 operators, bounded depth, whitelisted parameters — the deterministic tool). A multi-gate anti-overfit filter and hidden holdout are the boundary — agent only gets pass/fail, can't reverse-engineer the test set
- Factors auto-retire on performance decay. Budget cap per session limits multiple-testing risk. Deduplication catches factors that look different but capture the same signal — using high-dimensional feature space similarity rather than raw correlation
- The architecture generalizes beyond quant: constrained action space + hidden evaluation + binary feedback is a pattern for any agent safety system

**QuantStack** — Multi-Agent Research Platform [Production] \hfill Python, Rust
- 4 parallel LLM analysts synthesize daily reports across ~750 US equities and 300+ A-shares. Agents get pre-computed analytics and can only narrate facts — they cannot modify numbers. The constraint is the boundary
- Underneath: Rust data layer pulling from 8 financial APIs, 15 Bayesian analytics modules, anti-overfit validation. Runs in production daily, delivering reports before market open

**codex-par** — AI Coding Agent Orchestration [Tool] \hfill Rust
- MCP serializes and deadlocks multi-agent workflows. Bypassed it entirely — each agent gets its own isolated process, scheduled in dependency waves. Ships 14-tool MCP server for dynamic dispatch. 90 min → 30 min

**IvenaMeet** — Agent-Native Streaming Platform [Production] \hfill Rust, React, LiveKit
- Production streaming platform (30 endpoints, full auth, 81 commits) with an agent API — deterministic tools (API endpoints with simulate/execute modes) and clear boundaries (permissions, rate limits) let AI operators control a live room safely

## Education

**Brown University** — M.Sc. Computational Science, GPA 3.6/4.0 \hfill Sep 2023 – Jun 2025
- TCP/IP network stack in Rust, OS kernel in C — systems programming from scratch

**Sun Yat-sen University** — B.Sc. Physics, GPA 3.7/4.0 \hfill Sep 2019 – Jun 2023
- Probability theory, statistical mechanics, numerical methods — foundations for evaluation framework design

## Skills

Rust, Python, TypeScript, SQL | Axum, Redis, DuckDB | agent evaluation, constrained action spaces, LLM-as-Judge, MCP | Anthropic SDK
