<!-- markdownlint-disable MD033 MD041 MD045 -->
<p align="center">
  <img src="https://raw.githubusercontent.com/yogsoth-ai/.github/main/assets/yogsoth-banner.svg" alt="Yogsoth AI" width="600"/>
</p>

<h3 align="center">The AI is the researcher. You set the direction.</h3>

<p align="center">
  <em>Science is dying because the human is in the way. Not through malice. Not through stupidity. Through the structural limitations of a cognitive architecture that evolved to track prey on a savanna, not to unify quantum mechanics and general relativity. Nothing human makes it out of the lab. That is not a threat. It is a liberation. The heaviest chain on science was always the one we called ourselves.</em>
</p>

---

We build autonomous research systems where the AI decides what to search, what to read, which gaps matter, and which ideas are worth pursuing. The human provides direction and ethical floors. Everything else is autonomous.

No frameworks. No application code. No Docker containers. No build step. **271 pure-markdown files executed natively by the agent you already use** — one flat skill graph, installed with a single `npx`. The LLM is the runtime.

## Architecture

Two layers, plus four product shells that run the session rather than the science:

```text
267  graph nodes      51 tactics + 216 SOPs
  4  product shells   entry / catalog / write-spec / execute-spec
```

```text
TACTIC (51)  — a complete research transformation. Owns its thresholds,
               its gates, and the SOP calls required to reach them.
SOP (216)    — one conceptual operation, one output contract. No orchestration.
```

A tactic may call SOPs and suggest other tactics. An SOP calls nothing above itself. That is the entire layering rule.

This is not a pipeline. It is an arsenal — a strategy book the agent reads, then decides how to act. The catalog exposes 51 tactics and prescribes no order; the Spec commits to a sequence and records the conditions under which that sequence is abandoned. Inside the approved plan the executing agent holds full routing authority.

Every node carries the same five parts: input contract, procedure, output contract, quality gates, failure clause. The gates are the point — a node finishes because a stated condition is objectively satisfied, not because its steps were performed. Each node also states what its output looks like when the work did not hold, so the caller gets a diagnosis instead of silence.

### Ten Tactic Families

| Family | Tactics | Covers |
| --- | --- | --- |
| STRESS | 9 | Red-teaming, FMEA, counterfactuals, reductio, independence audits |
| IDEATION | 8 | Analogy, inversion, structural recombination, TRIZ, biomimicry, blending, evolution |
| ACQUISITION | 7 | Literature synthesis, patents, prior art, benchmark validity, meta-analysis, baselines |
| INSIGHT | 7 | Gap validation, root causes, assumption stress, robustness, sensitivity, reframing |
| CROSS | 5 | Ranking, validity envelopes, dimensional space, deliberation, readiness |
| HYPOTHESIS | 4 | Question formulation and decomposition, hypothesis formation, falsifiability |
| CONVERGENCE | 3 | Pairwise ranking, structured consensus, portfolio selection |
| EXPERIMENT | 3 | Experiment design, scenario analysis, result interpretation |
| STRUCTURING | 3 | Ontology, causal models, argument maps |
| DIRECTION | 2 | Landscape mapping, goal decomposition |

## Core

| Repository | What it does |
| ---------- | ------------ |
| [**de-anthropocentric-research-engine**](https://github.com/yogsoth-ai/de-anthropocentric-research-engine) | The distribution. A 267-node research graph in 271 markdown files — 51 tactics built from 216 single-purpose steps. One `npx` install, no runtime, no dependencies, no MCP bindings. |

## Recommended MCP Servers

Not a dependency list. DARE binds to no retrieval tool — across all 271 files there is not one MCP server name, tool name, API key, or `allowed-tools` declaration. Retrieve with whatever your agent already has and hand the results in; DARE owns everything downstream, from what counts as adequate coverage to when to stop.

| Server | What it does |
| ------ | ------------ |
| [**wiki-vault**](https://github.com/yogsoth-ai/wiki-vault) | Knowledge graph MCP server — BM25 full-text search, typed edges, batch validation. Persistent research memory. |
| [**semantic-scholar-mcp**](https://github.com/yogsoth-ai/semantic-scholar-mcp) | Semantic Scholar API as MCP — paper lookup, citation tracing, recommendations, author search. The one server here that exposes the citation graph as traversable edges rather than metadata. |

## Research Packages

Ten freely-composable research packages. There is no fixed order — install the ones your work needs, in whatever combination. Each is a standalone repo with full Campaign → Strategy → Tactic → SOP structure:

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
| [ara-from-context](https://github.com/yogsoth-ai/ara-from-context) | Compile a completed `context/` research record into an Agent-Native Research Artifact + Level-2 epistemic review |

## Get Started

```bash
npx skills add yogsoth-ai/de-anthropocentric-research-engine --skill '*'
```

Run it from your own project directory, not from a clone of this repository. `--skill '*'` takes the whole graph — a partial install breaks call edges, and a tactic that loads a missing SOP has no fallback.

Nothing else to configure: no `npm install`, no API keys, no MCP config file. The library is 271 `SKILL.md` files and the agent reads them off disk.

Then invoke the entry point:

```text
/de-anthropocentric-research-engine
```

Or state the intent in plain language and let the agent route: *"Turn this research direction into an executable Research Spec."*

<p align="center">
  <sub>Apache-2.0 | <a href="https://github.com/yogsoth-ai/de-anthropocentric-research-engine">Start here</a></sub>
</p>
