---
layout: research
title: Multi-Agent Reinforcement Learning
permalink: /research/multi-agent-rl/
banner_color: teal
nav: false
---

Many modern AI systems are not a single agent but a **network of agents** — LLM assistants that call one another, tool-using services, swarms of robots — each acting on its own, talking only to a few neighbours, with no central controller. My research studies how such agents can **keep learning and adapting together without breaking down**.

## Why partial observability is the hard part

In a single-agent problem, the agent eventually sees enough of the world to act well. In a **network of agents**, that stops being true — and the reason is *partial observability*.

Picture agents sitting on the nodes of a communication graph. Each one talks only to its immediate neighbours, and messages arrive **late**. So an agent never sees the whole system; it sees:

- its **own local state**, right now, and
- a **delayed, second-hand** picture of everyone else, relayed hop by hop.

The further away something happens, the more stale the news of it is by the time it arrives — the lag grows roughly with **graph distance × delay**. If the thing the team is trying to track keeps changing, distant agents are always chasing an out-of-date target. We call this the **information-arrival wall**: coordination degrades not because the agents are weak, but because *the information needed to coordinate physically arrives too late*.

This makes the problem fundamentally different from standard reinforcement learning, which assumes a stable, fully-observed target to converge to. Here there may be **no single fixed "best" behaviour** to settle on: every agent's best move depends on what the others are doing, and everyone is adapting at once. The research question becomes **stability** — can each agent learn a policy that stays bounded and well-behaved under a realistic compute and communication budget — rather than convergence to an (ill-posed) optimum.

## What we build

A small, readable, **decentralized** test-bench for exactly this setting: N agents on a graph, each with its **own local policy**, seeing others only through delayed messages, each running its **own independent learner**. It lets us measure, cleanly, how coordination collapses as the network grows, as messages get staler, and as the target drifts — and to compare learning algorithms (policy-gradient methods, trust-region methods, and recurrent/belief methods) against the best achievable performance.

<div class="repo-grid">
<div class="repo-card">
  <a href="https://github.com/krm9c/coadapt-marl" target="_blank" class="repo-link">
    <div class="repo-header">
      <i class="fab fa-github"></i>
      <h3>coadapt-marl</h3>
    </div>
    <p class="repo-path">krm9c/coadapt-marl</p>
  </a>
  <p class="repo-desc">Decentralized multi-agent RL harness under partial observability (JAX). Per-agent solvers: REINFORCE, PPO, GRPO, TRPO, recurrent.</p>
  <a href="https://krm9c.github.io/coadapt-marl/" target="_blank" class="repo-view-btn">Documentation &amp; code &rarr;</a>
</div>
</div>

## Publications

- [Who Gets the Reward, Who Gets the Blame? Evaluation-Aligned Training Signals for Multi-LLM Agents](https://arxiv.org/abs/2511.10687) - *arXiv 2025*
- [SWARM+: Scalable and Resilient Multi-Agent Consensus for Decentralized Data-Aware Workload Management](https://arxiv.org/abs/2603.19431) - *arXiv 2026*
- [SWARM: Reimagining Scientific Workflow Management Systems in a Distributed World](https://doi.org/10.1177/10943420251339317) - *Int. J. High Performance Computing Applications 2025*
