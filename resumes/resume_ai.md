# Zhenyu Huang (黄振宇)

huangzhy77@outlook.com | +86 13502448752 | [github.com/hzy-hits](https://github.com/hzy-hits) | Hong Kong | Top Talent Pass holder | Available immediately

---

I build the control layer around AI agents. At Meituan I make agent behavior testable. In my quant platform I let agents narrate but not calculate. In my factor lab I give them a search space they cannot escape and a holdout they cannot game. Different products, same pattern: constrain, observe, evaluate.

## Experience

**Meituan** — Software Engineer, Core Local Commerce \hfill Jul 2025 – Present
- Agent quality was one number with no attribution. I split it into 3 evaluation layers (routing / parameters / answer) with per-dimension badcase analysis — the 11-point gap between 96% routing accuracy and 85% answer quality only became visible after decomposition
- LLM judges drift and flatter by default. Anti-Sycophancy prompting ("default to FAIL"), recheck-on-fail with a stronger model, and 5-round repeat experiments (std=0.27%) turned an unreliable scorer into a calibrated evaluation pipeline. Hallucination detection went from ~70% to 91% positive-case protection through 6-rule assertion grading
- SSE streaming made existing mock tools useless for agent testing. I proved the boundary, then built a zero-intrusion transparent proxy — LLM decisions become injectable, replayable, and assertable without touching business code. 7/7 verification items passed
- Reverse-engineered a 1135-file insurance claims system across two service layers, found 5 confirmed bugs through code review including a transaction-boundary defect invisible to interface-level testing

## Selected Engineering Work

**QuantfactorLab** — Agent Evaluation System [Research] \hfill Python
- Letting LLMs write arbitrary research code would make factor discovery unauditable. I boxed exploration into a constrained DSL — bounded depth, whitelisted parameters, ~35 operators
- Agents overfit to any feedback channel they can see. I hid out-of-sample metrics completely and return only PASS/FAIL after a multi-gate walk-forward pipeline, preventing holdout gaming while preserving iterative search
- Autonomous research without guardrails collapses into multiple-testing noise. Budget caps, factor deduplication, and automatic retirement on decay keep it honest. The pattern generalizes beyond quant to any agent safety system

**QuantStack** — Multi-Agent Research Platform [Production] \hfill Python, Rust
- Multi-agent report generation risks hallucinated arithmetic. 4 parallel Claude analysts read only pre-computed payloads and narrate facts — they cannot touch the numbers
- To keep that narration grounded: async Rust ingestion from 8 APIs, DuckDB storage, 15 probability-first analytics modules covering ~750 US equities and 300+ A-shares. Runs daily before market open

**codex-par** — AI Coding Agent Orchestration [Tool] \hfill Rust
- MCP-based agent workflows serialize and deadlock. I bypassed MCP entirely — isolated process per agent, dependency-wave scheduling, 14-tool MCP server for non-blocking dispatch. 90 min → 30 min

**IvenaMeet** — Agent-Native Streaming Platform [Production] \hfill Rust, React, LiveKit
- Raw AI access to a live room would be unsafe. I exposed a constrained agent API — simulate/execute modes, idempotency, permission boundaries, rate limits — over a 30-endpoint streaming control plane with full auth lifecycle

## Education

**Brown University** — M.Sc. Computational Science, GPA 3.6/4.0 \hfill Sep 2023 – Jun 2025
- TCP/IP network stack in Rust, OS kernel in C — systems programming from scratch

**Sun Yat-sen University** — B.Sc. Physics, GPA 3.7/4.0 \hfill Sep 2019 – Jun 2023
- Probability theory, statistical mechanics, numerical methods — foundations for evaluation framework design

## Skills

Rust, Python, TypeScript, SQL | Axum, Redis, DuckDB | agent evaluation, constrained action spaces, LLM-as-Judge, MCP | Anthropic SDK
