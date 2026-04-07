# Hi, I'm Zhenyu

I design systems where AI agents do useful work.

The pattern is always the same: give them **deterministic tools** and **clear boundaries**, and they find the answers. My role is never the explorer — I'm the one who builds the tools and defines what "good" looks like.

**Brown CS** (M.Sc.) / **Sun Yat-sen Physics** (B.Sc.) / **Hong Kong**

---

### The design philosophy

| Project | Deterministic tools | Boundaries | What the agent does |
|---|---|---|---|
| [**QuantStack**](https://github.com/hzy-hits/QuantStack) | Data pipelines, analytics modules | Probability framework, "narrate facts only" | Synthesizes daily research reports |
| [**QuantfactorLab**](https://github.com/hzy-hits/QuantfactorLab) | Factor DSL, backtest framework | Anti-overfit gates, hidden holdout, JEPA dedup | Discovers alpha factors autonomously |
| Meituan (work) | Mock server, eval framework | Zero intrusion, LLM-as-Judge rubrics | Gets tested and evaluated |
| [**codex-par**](https://github.com/hzy-hits/codex-par) | Process isolation, wave scheduler | Dependency graph, budget | Runs coding tasks in parallel |
| [**IvenaMeet**](https://github.com/hzy-hits/IvenaMeet) | Agent API endpoints | Permissions, rate limits, simulate mode | Controls a live streaming room |

Every project is a different instance of the same problem: **constrained action space + boundary optimization → AI finds useful answers.**

---

### What's running in production

**[QuantStack](https://github.com/hzy-hits/QuantStack)** — ~750 US equities twice daily, 300+ A-shares daily. Rust data ingestion from 8 market APIs, 15 Bayesian analytics modules, 4 parallel LLM analysts. Reports ship before market open. Python + Rust.

**[QuantfactorLab](https://github.com/hzy-hits/QuantfactorLab)** — LLM agents propose alpha factors in a constrained expression language. System validates with walk-forward backtesting and a 5-gate anti-overfit filter. Agent never sees holdout metrics — only pass/fail. Factors auto-retire on decay. Python.

**[IvenaMeet](https://github.com/hzy-hits/IvenaMeet)** — Private streaming platform. Rust control plane, React frontend, LiveKit WebRTC. 30 endpoints, full auth lifecycle, broadcast orchestration, agent API. 81 commits, daily use.

**[codex-par](https://github.com/hzy-hits/codex-par)** — AI coding agents through MCP serialize and deadlock. This bypasses MCP entirely — each agent gets its own isolated process, scheduled in dependency waves. 90 min → 30 min. 14-tool MCP server for dynamic dispatch. Rust.
