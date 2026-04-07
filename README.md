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

## What I Build

- Agent control layers: deterministic testing, constrained action spaces, hidden-holdout evaluation
- Quant research infrastructure: probability-first analytics, anti-overfit validation, daily production pipelines
- Backend systems: Rust control planes that keep invariants under concurrency, retries, auth, and real users

At Meituan, that means making agent behavior testable and reviewable. In my own systems, it means the same pattern shows up in different forms: agents can explore, but they don't get to escape the guardrails.

## Operating Model

<p align="center">
  <img src="architecture.svg" alt="Tools -> Boundaries -> Agent" width="85%" />
</p>

The pattern is consistent across projects:

<table>
<tr>
<td width="20%"><strong>Project</strong></td>
<td width="30%"><strong>System tension</strong></td>
<td width="25%"><strong>Boundary / design choice</strong></td>
<td width="25%"><strong>Result</strong></td>
</tr>
<tr>
<td><a href="https://github.com/hzy-hits/QuantStack"><b>QuantStack</b></a></td>
<td>LLMs can write polished reports faster than they can reason about numbers safely</td>
<td>The program computes; agents narrate pre-computed payloads only</td>
<td>Daily reports across ~750 US equities and 300+ Chinese A-shares</td>
</tr>
<tr>
<td><a href="https://github.com/hzy-hits/QuantfactorLab"><b>QuantfactorLab</b></a></td>
<td>Autonomous factor search tends to overfit any feedback channel it can see</td>
<td>Constrained DSL, 5-gate walk-forward validation, hidden holdout, budget cap</td>
<td>Agents can search aggressively without seeing or gaming the test set</td>
</tr>
<tr>
<td><a href="https://github.com/hzy-hits/codex-par"><b>codex-par</b></a></td>
<td>MCP serializes parallel work and can deadlock when both sides block</td>
<td>Process isolation plus dependency-wave scheduling outside MCP</td>
<td>Representative 3-task workflows shrink from ~90 minutes to ~30</td>
</tr>
<tr>
<td><a href="https://github.com/hzy-hits/IvenaMeet"><b>IvenaMeet</b></a></td>
<td>Live room state breaks easily under retries, permissions, and concurrent actions</td>
<td>Scoped tokens, Redis-backed checks, rate limits, and `simulate|execute` agent commands</td>
<td>Safe control plane for a private streaming room with durable chat and broadcast orchestration</td>
</tr>
</table>

## Selected Systems

**[QuantStack](https://github.com/hzy-hits/QuantStack)** `Python` `Rust`

Dual-market quant research platform running daily in production. Async Rust ingestion pulls from 8 APIs into DuckDB, 15 analytics modules emit explicit `P(event | conditions)`, and 4 parallel LLM analysts generate reports without ever touching the arithmetic.

**[QuantfactorLab](https://github.com/hzy-hits/QuantfactorLab)** `Python`

Factor discovery system built around a simple rule: agents are good at generating hypotheses and bad at judging themselves. Search happens inside a DSL; promotion happens only after walk-forward validation, hidden holdouts, and anti-overfit gates.

**[IvenaMeet](https://github.com/hzy-hits/IvenaMeet)** `Rust` `React` `LiveKit`

Private meeting-room control plane with 30 endpoints, full auth lifecycle, durable chat, broadcast orchestration, and an agent API designed to be automatable without being reckless.

**[codex-par](https://github.com/hzy-hits/codex-par)** `Rust`

Parallel task runner for coding agents. Built because MCP made multi-agent execution too serialized, too opaque, and too deadlock-prone to trust at scale.

## Resume Variants

- [AI / Agent Infrastructure](resume_ai.md)
- [Quant / Research Infrastructure](resume_quant.md)
- [Backend / Fintech Systems](resume_fintech.md)
