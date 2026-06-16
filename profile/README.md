<!-- markdownlint-disable MD033 MD041 MD045 -->
<p align="center">
  <img src="https://raw.githubusercontent.com/yogsoth-ai/.github/main/assets/yogsoth-banner.svg" alt="Yogsoth AI" width="600"/>
</p>

<h3 align="center">The AI is the researcher. You set the direction.</h3>

<p align="center">
  <em>Science is dying because the human is in the way. Not through malice — through the structural limitations of a cognitive architecture that evolved to track prey on a savanna, not to unify quantum mechanics and general relativity. The heaviest chain on science was always the one we called ourselves.</em>
</p>

---

We build autonomous research systems where the AI decides what to search, what to read, which gaps matter, and which ideas are worth pursuing. The human provides direction and ethical floors. Everything else is autonomous.

No frameworks. No application code. No Docker containers. **900+ pure-markdown skill files executed natively by Claude Code**, organized as 9 freely-composable research packages. The LLM is the runtime.

---

## Architecture

Four-layer military command hierarchy. Each layer calls only the layer below it:

```bash
Campaign (45+)  — WHAT to research    (full research stages)
Strategy (200+) — WHEN and WHY        (iteration loops, stopping conditions)
Tactic (120+)   — HOW to combine      (orchestrates multiple SOPs)
SOP (500+)      — HOW to execute      (single-responsibility operations)
```

This is not a pipeline. It is an arsenal — a strategy book the AI reads, then decides how to act. The 9 research packages are freely composable with no fixed order. Non-linear routing. Explicit backtrack conditions. The agent chooses which package to invoke, which strategies to combine, and when to retreat.

---

## Core

| Repository | What it does |
| ---------- | ------------ |
| [**de-anthropocentric-research-engine**](https://github.com/yogsoth-ai/de-anthropocentric-research-engine) | The distribution. 900+ skills unified under one orchestrator. Clone once, get everything. |
| [**wiki-vault**](https://github.com/yogsoth-ai/wiki-vault) | Knowledge graph MCP server — BM25 full-text search, typed edges, batch validation. Persistent research memory. |
| [**semantic-scholar-mcp**](https://github.com/yogsoth-ai/semantic-scholar-mcp) | Semantic Scholar API as MCP — paper lookup, citation tracing, recommendations, author search. |

## Research Packages

Nine freely-composable research packages. There is no fixed order — CC reads the catalog and routes across them as the research demands. Each is a standalone repo with full Campaign → Strategy → Tactic → SOP structure:

| Package | Purpose |
| ------- | ------- |
| [north-star-crystallization](https://github.com/yogsoth-ai/north-star-crystallization) | Direction finding — cold/warm/hot-start dialogue to crystallize research goals |
| [knowledge-acquisition](https://github.com/yogsoth-ai/knowledge-acquisition) | Systematic literature survey, citation chaining, patent mining, meta-analysis |
| [deep-insight](https://github.com/yogsoth-ai/deep-insight) | Gap analysis, structural understanding, abstraction extraction |
| [hypothesis-formation](https://github.com/yogsoth-ai/hypothesis-formation) | Abductive, inductive, and deductive hypothesis generation with falsifiability audits |
| [creative-ideation](https://github.com/yogsoth-ai/creative-ideation) | 31+ generation methods — SCAMPER, TRIZ, biomimicry, morphological analysis, concept blending |
| [convergence](https://github.com/yogsoth-ai/convergence) | Multi-criteria scoring, Pareto frontier, pairwise ranking, dialectical synthesis |
| [stress-test](https://github.com/yogsoth-ai/stress-test) | Adversarial validation — assumption destruction, red-teaming, worst-case design |
| [experiment-execution](https://github.com/yogsoth-ai/experiment-execution) | Factor-level design, parameter screening, sensitivity analysis, result collection |
| [knowledge-structuring](https://github.com/yogsoth-ai/knowledge-structuring) | Ontology building, causal modeling, dimensional analysis, argument mapping (wiki vault) |

## Infrastructure

| Repository | Role |
| ---------- | ---- |
| [literature-engine](https://github.com/yogsoth-ai/literature-engine) | Full-text paper reading enforcement via AlphaXiv |
| [web-browsing](https://github.com/yogsoth-ai/web-browsing) | Rigorous web research — prevents shallow snippet-only analysis |
| [subagent-spawning](https://github.com/yogsoth-ai/subagent-spawning) | Parallel research dispatch with full MCP tool access |
| [context-management](https://github.com/yogsoth-ai/context-management) | Session checkpointing — 500+ line markdown snapshots for recovery |

---

## Get Started

```bash
git clone https://github.com/yogsoth-ai/de-anthropocentric-research-engine.git
cd de-anthropocentric-research-engine
npm install
```

Copy `mcp.example.json` → `.mcp.json`, add your API keys, then:

```bash
/de-anthropocentric-research-engine
```

The orchestrator handles the rest.

---

## Status

**v3.1.0** — shipped. 900+ skills across 9 freely-composable packages, 8 orchestrator skills, 6 MCP integrations, non-linear execution with backtracking. Fully self-contained: the entire skill→skill dependency graph is encoded inline in frontmatter and machine-verified closed.

**Next:**

- Skill ablation — systematic reduction of the 900+ skill corpus via ablation study
- Cross-device session management — persistent research state across machines
- Paper-writing skills — from research output to publishable manuscript

---

<p align="center">
  <sub>Apache-2.0 | <a href="https://github.com/yogsoth-ai/de-anthropocentric-research-engine">Start here</a></sub>
</p>
