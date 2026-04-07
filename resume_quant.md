# Zhenyu Huang (黄振宇)

huangzhy77@outlook.com | +86 13502448752 | [github.com/hzy-hits](https://github.com/hzy-hits) | Hong Kong | Top Talent Pass holder | Available immediately

---

Physics to CS. I build quant research infrastructure in Rust and Python — data pipelines, Bayesian probability models, and anti-overfit validation. I run a production platform covering US equities and A-shares daily; the AI proposes strategies inside a constrained action space, my system validates which ones hold up out-of-sample.

## Experience

**Meituan** — Software Engineer, Core Local Commerce \hfill Jul 2025 – Present
- Transparent proxy intercepts LLM agent API calls and reroutes to a mock server — deterministic agent testing without modifying product code
- LLM-as-Judge pipeline scores agent outputs against structured rubrics, replacing manual review
- Regression testing for AI-driven insurance workflows — catches behavioral drift across prompt and model changes

## Selected Engineering Work

**QuantStack** — Dual-Market Research Platform [Production] \hfill Python, Rust
- ~748 US equities twice daily, 300+ A-shares daily. Rust data layer pulls from 8 financial APIs (Finnhub, FRED, SEC Edgar, Tushare, AKShare, Polymarket) into DuckDB with rate limiting, retries, and idempotent scheduling
- 15 analytics modules each output a conditional probability with credible interval and sample size — HMM regime detection, Beta-Binomial Bayesian updating, realized volatility estimators (Yang-Zhang, Garman-Klass)
- A-share flow score fusing 6 orthogonal signals: northbound capital, margin, block trades, institutional flow, insider activity, tape abnormality — EWMA smoothed, cross-sectionally normalized
- 4 LLM analysts run in parallel to synthesize reports. They narrate pre-computed facts — cannot modify numbers. Reports delivered automatically before market open

**QuantfactorLab** — Factor Discovery with Anti-Overfit Validation [Research] \hfill Python
- LLM agents propose alpha factors in a constrained expression language (~35 operators, bounded depth, whitelisted lookback windows). System validates each through expanding-window walk-forward backtesting
- 5-gate anti-overfit filter: IC, IC_IR, turnover, monotonicity, correlation — calibrated separately for US and CN markets. Agent never sees holdout metrics — only pass/fail
- Bootstrap significance testing with 100k resamples. Factors auto-retire when rolling 60-day IC decays. Deduplication in high-dimensional feature space catches "different formula, same signal" redundancy — physics-inspired geometric approach to factor similarity

**codex-par** — Research Automation [Tool] \hfill Rust
- Parallel runner for AI coding agent tasks. Schedules into dependency waves instead of serial execution — 90-minute workflows finish in 30

## Education

**Brown University** — M.Sc. Computational Science, GPA 3.6/4.0 \hfill Sep 2023 – Jun 2025
- TCP/IP network stack in Rust, OS kernel in C — systems programming from scratch

**Sun Yat-sen University** — B.Sc. Physics, GPA 3.7/4.0 \hfill Sep 2019 – Jun 2023
- Statistical mechanics, probability theory, numerical methods — the math toolkit behind my quant infrastructure

## Skills

Rust, Python, SQL | DuckDB, polars, scipy, statsmodels | Bayesian inference, HMM, walk-forward backtesting, bootstrap testing | Anthropic SDK
