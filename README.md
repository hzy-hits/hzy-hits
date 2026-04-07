<h1 align="center">
  <a href="https://github.com/hzy-hits">
    <img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=600&size=28&duration=3200&pause=900&color=58A6FF&center=true&vCenter=true&random=false&width=760&lines=Programs+compute.+Agents+narrate.;Constrain.+Observe.+Evaluate.;Rust+systems+and+AI+control+layers." alt="Typing SVG" />
  </a>
</h1>

<p align="center">
  <strong>Zhenyu Huang</strong>&ensp;·&ensp;Shanghai → Hong Kong (Top Talent Pass)
</p>

<p align="center">
  I build systems that keep AI useful by giving it explicit tools, hard boundaries, and feedback it cannot game.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/-Rust-000000?style=flat-square&logo=rust" />
  <img src="https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/-DuckDB-FEF000?style=flat-square&logo=duckdb&logoColor=black" />
  <img src="https://img.shields.io/badge/-Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/-Axum-111111?style=flat-square" />
</p>

---

## Work

I care about systems where failure modes matter:

- AI agents that should be useful without becoming untestable or ungovernable
- research pipelines where polished output is cheap but statistical honesty is expensive
- backend control planes that must preserve invariants under concurrency, retries, auth, and real users

Across all three, I keep coming back to the same pattern:

- **Constrain** the action space so the system stays legible
- **Observe** execution while it is happening, not only after it finishes
- **Evaluate** with feedback the system cannot game

## Selected Systems

**[QuantStack](https://github.com/hzy-hits/QuantStack)** `Python` `Rust`  
Dual-market quant research platform covering ~750 US equities and 300+ Chinese A-shares. The core rule is simple: the program computes, the agent narrates. Async Rust ingestion pulls from 8 APIs into DuckDB, 15 analytics modules emit explicit `P(event | conditions)`, and LLM analysts write reports without ever touching the arithmetic.

**[QuantfactorLab](https://github.com/hzy-hits/QuantfactorLab)** `Python`  
Autonomous factor discovery is useful only if it is hard to fool. I boxed agent search into a constrained DSL, hid holdout metrics completely, and required every candidate to survive walk-forward validation, anti-overfit gates, and post-promotion decay checks.

**[IvenaMeet](https://github.com/hzy-hits/IvenaMeet)** `Rust` `React` `LiveKit`  
Private meeting-room control plane with 30 endpoints, full auth lifecycle, durable chat, and broadcast orchestration. The interesting part is not WebRTC itself; it is keeping room state, permissions, and automation safe under retries and concurrent actions.

**[codex-par](https://github.com/hzy-hits/codex-par)** `Rust`  
Parallel runtime for coding agents. I built it because MCP made multi-agent execution too serialized, too opaque, and too deadlock-prone to trust. The fix was to move parallelism back to process isolation, dependency-wave scheduling, and live runtime visibility.

## Current Themes

- deterministic agent testing and evaluation
- probability-first systems instead of black-box scoring
- runtime observability, cancellation, and failure handling
- Rust services that stay honest under operational pressure

## More

Role-specific resume variants:
[AI / Agent Infrastructure](resume_ai.md) ·
[Quant / Research Infrastructure](resume_quant.md) ·
[Backend / Fintech Systems](resume_fintech.md)
