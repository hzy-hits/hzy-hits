# Zhenyu Huang (黄振宇)

huangzhy77@outlook.com | +86 13502448752 | [github.com/hzy-hits](https://github.com/hzy-hits) | Hong Kong | Top Talent Pass holder | Available immediately

---

> Quant infrastructure engineer building production research pipelines, probability-first analytics, and anti-overfit validation systems across US equities and Chinese A-shares.

## Experience

**Meituan** — Software Engineer, Core Local Commerce \hfill Jul 2025 – Present
- Designed a zero-intrusion proxy for LLM agent testing, enabling deterministic validation of agent tool-calling behavior without modifying business code
- Built an LLM-as-Judge framework for scoring AI-generated outputs at scale across insurance and local-services scenarios

## Selected Projects

**QuantStack** — Dual-Market Quantitative Research Platform \hfill Python, Rust | 40,000+ LOC
- Built and operate a production research platform covering ~748 US equities twice daily and 300+ Chinese A-shares daily, delivering automated probability reports through Gmail-based distribution
- Implemented 15 analytics modules on top of a shared 5-axiom probability framework, including 2-state Gaussian HMM regime detection, Beta-Binomial Bayesian updating, and realized volatility estimators
- Wrote an async Rust ingestion layer that pulls from 8 APIs including Finnhub, FRED, SEC Edgar, Polymarket, Tushare, and AKShare into DuckDB with rate limiting, retries, and idempotent scheduling
- Built an A-share flow score that fuses northbound capital, margin, block trades, and institutional activity with EWMA smoothing, cross-sectional normalization, and probit transforms
- Orchestrated 4 parallel Claude API analyst agents for report synthesis while constraining them to narrate pre-computed facts only

**QuantfactorLab** — AI-Assisted Factor Discovery Lab \hfill Python | 10,000+ LOC
- Built a constrained factor-mining system where LLM agents propose alpha formulas in a DSL and the platform validates them through expanding-window walk-forward backtests
- Implemented a 5-gate anti-overfit pipeline using IC, IC_IR, turnover, monotonicity, and correlation thresholds, with market-specific calibration for US and CN universes
- Hid out-of-sample metric values from the agent and returned only PASS/FAIL, limiting multiple-testing leakage and preventing holdout reverse-engineering
- Added three-tier bootstrap significance testing with 100,000 resamples and automatic retirement for factors whose rolling 60-day IC decays below threshold

**Light Orchestra (codex-par)** — Research Automation Infrastructure \hfill Rust | 8,000+ LOC
- Built a process-isolated parallel runner for Codex tasks, useful for scaling research and review workflows across dependency-aware waves instead of serialized execution

## Education

**Brown University** — M.Sc. Computational Science, GPA 3.6/4.0 \hfill Sep 2023 – Jun 2025
- Built TCP/IP network stack in Rust and OS kernel in C

**Sun Yat-sen University** — B.Sc. Physics, GPA 3.7/4.0 \hfill Sep 2019 – Jun 2023
- Probability theory, statistical mechanics, and numerical methods

## Skills

**Quant:** Bayesian inference, HMM regime detection, factor evaluation, walk-forward backtesting, bootstrap significance testing, probability calibration
**Data Systems:** DuckDB, polars, scipy, pandas, statsmodels, market data pipelines
**Languages:** Python, Rust, SQL, TypeScript
**AI/Automation:** Anthropic SDK, constrained agent workflows, evaluation pipeline design
