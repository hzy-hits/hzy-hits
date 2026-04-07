# Hi, I'm Zhenyu

I build the infrastructure that makes AI agents useful in production — then I point them at hard problems.

Right now that problem is quantitative research. I built the data pipelines, the evaluation framework, and the anti-overfit guardrails. The AI proposes strategies. My system decides which ones survive.

**Brown CS** (M.Sc.) / **Sun Yat-sen Physics** (B.Sc.) / **Hong Kong**

---

### The pattern across my work

| I build the... | So that AI agents can... | Project |
|---|---|---|
| Constrained expression language + walk-forward backtesting + hidden holdout | Discover alpha factors without overfitting | [**QuantStack**](https://github.com/hzy-hits/QuantStack) | 
| Multi-gate anti-overfit filter + bootstrap significance testing | Propose and get validated — never seeing the test set | [**QuantfactorLab**](https://github.com/hzy-hits/QuantfactorLab) |
| Mock proxy + LLM-as-Judge pipeline | Be tested deterministically in production | Meituan (work) |
| Process isolation + wave scheduling + MCP server | Run in parallel without deadlocking | [**codex-par**](https://github.com/hzy-hits/codex-par) |
| Agent API with simulate/execute modes | Control a live streaming room safely | [**IvenaMeet**](https://github.com/hzy-hits/IvenaMeet) |

---

### What's running in production

**[QuantStack](https://github.com/hzy-hits/QuantStack)** — delivers daily probability reports across ~750 US equities and 300+ A-shares. Async Rust fetcher pulling 8 market data APIs into DuckDB, 15 Bayesian analytics modules, 4 parallel Claude analysts synthesizing the output. Ships an email every morning before market open.

**[IvenaMeet](https://github.com/hzy-hits/IvenaMeet)** — private streaming platform I use daily. Rust control plane, React frontend, LiveKit for WebRTC. 30 endpoints, TOTP auth, invite lifecycle, broadcast orchestration. 81 commits and counting.

**[codex-par](https://github.com/hzy-hits/codex-par)** — I got mass-parallelism for AI coding agents by bypassing MCP entirely. Each task gets its own process with `setpgid` isolation, scheduled in dependency waves. Live dashboard, 14-tool MCP server for dynamic dispatch.

---

`Rust` `Python` `TypeScript` `Axum` `Tokio` `DuckDB` `Redis` `LiveKit` `Claude API` `MCP`
