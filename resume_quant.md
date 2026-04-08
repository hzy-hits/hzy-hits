# Zhenyu Huang (黄振宇)

huangzhy77@outlook.com | +86 13502448752 | [github.com/hzy-hits](https://github.com/hzy-hits) | Hong Kong | Top Talent Pass holder | Available immediately

---

Physics to CS. I build quant research infrastructure in Rust and Python where every output is an explicit conditional probability and nothing reaches production without surviving hidden holdouts. The AI explores; my system decides what counts as evidence.

## Experience

**Meituan** — Software Engineer, Core Local Commerce \hfill Jul 2025 – Present
- Agent quality was one number — couldn't tell whether failure was in routing, parameters, or the answer. I designed a 3-layer evaluation framework with 40/40/20 weighting. The 11-point gap between routing and answer quality only surfaced after decomposition
- Single-run prompt evaluation has 2-3 percentage point noise. 5-round repeat experiments with mean/std tracking, multi-model comparison, and badcase attribution separate signal from measurement error
- Built a zero-intrusion proxy for deterministic agent testing and an LLM-as-Judge pipeline for automated quality scoring — both without touching business code

## Selected Engineering Work

**QuantStack** — Dual-Market Research Platform [Production] \hfill Python, Rust
- Fresh cross-market research every day means 8 external APIs, inconsistent schemas, and rate limits that can break timeliness at any point. I moved ingestion into async Rust with retries, pacing, and idempotent DuckDB writes across ~748 US equities and 300+ A-shares
- Instead of opaque scores, every analytics module emits an explicit conditional probability with sample size and credible interval. 15 modules total — HMM regime detection, Beta-Binomial updating, Yang-Zhang and Garman-Klass realized volatility
- A-share flow data is noisy and fragmented across sources. I fused 6 orthogonal signals — northbound capital, margin, block trades, institutional flow, insider activity, tape abnormality — into one cross-sectionally normalized score
- Report generation under LLM use still has to stay auditable. 4 parallel analysts read only structured payloads and narrate pre-computed facts. They cannot modify numbers. Delivered before market open

**QuantfactorLab** — Factor Discovery with Anti-Overfit Validation [Research] \hfill Python
- Letting LLMs search by arbitrary code turns factor mining into uncontrolled multiple testing. I constrained exploration to a DSL — bounded depth, whitelisted lookbacks, narrow operator set
- Agents overfit to whatever feedback they can see. I hid holdout metrics entirely and return only PASS/FAIL, after a 5-gate walk-forward pipeline calibrated separately for US and CN markets
- Promoted factors still need to stay honest after launch. 100k-resample bootstrap testing, rolling auto-retirement on IC decay, and geometric deduplication for formulas that look different but capture the same signal

**codex-par** — Research Automation [Tool] \hfill Rust
- Serialized agent execution was wasting hours on multi-task research workflows. Dependency-wave scheduling turns 90-minute runs into 30

## Education

**Brown University** — M.Sc. Computational Science, GPA 3.6/4.0 \hfill Sep 2023 – Jun 2025
- TCP/IP network stack in Rust, OS kernel in C — systems programming from scratch

**Sun Yat-sen University** — B.Sc. Physics, GPA 3.7/4.0 \hfill Sep 2019 – Jun 2023
- Statistical mechanics, probability theory, numerical methods — the math toolkit behind my quant infrastructure

## Skills

Rust, Python, SQL | DuckDB, polars, scipy, statsmodels | Bayesian inference, HMM, walk-forward backtesting, bootstrap testing | Anthropic SDK
