# Computer Science LLM Agent Skills

![Skills](https://img.shields.io/badge/Skills-44-2ea44f)
![Focus](https://img.shields.io/badge/Focus-CS_LLM_Agent_Workflows-0969da)

A curated collection of reusable skills for LLM agents working on computer science research, academic writing, experiment workflows, and research-oriented software engineering.

**Language:** **English** · [中文](README.zh-CN.md)

## Table of Contents

- [What This Repository Is](#what-this-repository-is)
- [Why Use This Repository](#why-use-this-repository)
- [What's Included](#whats-included)
- [Getting Started](#getting-started)
- [How to Use These Skills](#how-to-use-these-skills)
- [How to Browse](#how-to-browse)
- [Example Use Cases](#example-use-cases)
- [Attribution and License Notes](#attribution-and-license-notes)

## What This Repository Is

This repository is a workflow-first public skill collection for:

- computer science researchers
- PhD students
- research engineers
- developer-researchers who move between papers, experiments, code, and releases

It is designed around recurring CS work such as literature review, paper writing, benchmark design, experiment analysis, model workflows, agent development, and GitHub-ready repository cleanup.

## Why Use This Repository

- **Focused on CS workflows**: it targets the tasks CS researchers and builders actually repeat.
- **Ready for agent-assisted work**: the skills are organized for practical use in coding and research agents.
- **Simple to install**: all installable skills live directly under one [`skills/`](skills/) folder.
- **Easy to browse**: the docs provide both a catalog view and a task-first view.
- **Covers both tools and workflows**: the collection includes library-oriented skills and workflow-oriented skills in the same installable set.

## Who It Is For

Use this repository if your work regularly involves combinations of:

- literature review and related-work synthesis
- paper drafting, revision, review, and rebuttal
- benchmark design and experiment tracking
- code reproduction and result analysis
- ML, LLM, graph, RL, or agent system development
- repository cleanup and public GitHub release preparation

## What's Included

- `44` public skills under [`skills/`](skills/)
- one installable folder layout so users can copy everything at once
- a public index that records each skill's `Primary Category`, `Task Tags`, and `Type`

If you care about provenance, the [Skills Index](docs/skills-index.md) marks which skills are `Curated` and which are `Custom`.

## Workflow Coverage

The current public set covers these workflow areas:

- research planning and task decomposition
- literature review and reference management
- paper writing, revision, review, and rebuttal
- benchmarking, reproducibility, and experiment operations
- technical writing, markdown-first documentation, and format conversion
- data engineering, EDA, statistics, and visualization
- ML, LLM, graph, RL, and supporting compute workflows
- agent systems and automation-oriented development
- slides, posters, and technical diagrams
- repository maintenance and open-source release preparation

## Getting Started

1. If you want the simplest setup, copy everything in [`skills/`](skills/) into your agent's skills directory.
2. If you want a smaller setup, browse [`docs/skills-index.md`](docs/skills-index.md) or [`docs/usage-guide.md`](docs/usage-guide.md) first and copy only the skills you need.
3. Restart or reload your agent if it does not detect new skills automatically.

## How to Use These Skills

### Step 1: Copy all skills to your skills directory

Copy the folders inside [`skills/`](skills/) to one of the supported skill directories below. You can install skills globally or per-project.

**Global installation** (recommended if you want the full skill set available everywhere):

| Tool | Directory |
| --- | --- |
| Cursor | `~/.cursor/skills/` |
| Claude Code | `~/.claude/skills/` |
| Codex | `~/.codex/skills/` |
| Gemini CLI | `~/.gemini/skills/` |

**Project-level installation** (recommended if skills should stay inside one repo):

| Tool | Directory |
| --- | --- |
| Cursor | `.cursor/skills/` |
| Claude Code | `.claude/skills/` |
| Codex | `.codex/skills/` |
| Gemini CLI | `.gemini/skills/` |

### Step 2: Copy the contents of `skills/`

**Example: global install for Cursor**

```bash
cp -r Computer-science-llm-agent-skills/skills/* ~/.cursor/skills/
```

**Example: global install for Claude Code**

```bash
cp -r Computer-science-llm-agent-skills/skills/* ~/.claude/skills/
```

**Example: global install for Codex**

```bash
cp -r Computer-science-llm-agent-skills/skills/* ~/.codex/skills/
```

**Example: global install for Gemini CLI**

```bash
cp -r Computer-science-llm-agent-skills/skills/* ~/.gemini/skills/
```

**Example: project-level install**

```bash
mkdir -p .codex/skills
cp -r /path/to/Computer-science-llm-agent-skills/skills/* .codex/skills/
```

If you prefer a smaller setup, copy only selected skill folders instead of the whole directory.

### Step 3: Use the skills in your prompt

After the folders are installed, ask your agent to work normally. If you want more control, mention the skill names explicitly.

Example prompts:

- `Use the literature-review, citation-management, and scientific-writing skills to turn these papers into a related-work outline.`
- `Use benchmark-design and experiment-tracking to define an evaluation plan for this repo.`
- `Use repo-cleanup and github-release-prep to make this project ready for public release.`
- `Use agent-coding and transformers to design a first version of this agent workflow.`

## How to Browse

Start with these public docs:

1. [Skills Index](docs/skills-index.md): the canonical public catalog with `Primary Category`, `Task Tags`, `Type`, and `Use for`
2. [Usage Guide](docs/usage-guide.md): the fastest path from a workflow need to the right skills
3. [Task-to-Skills Mapping](docs/task-to-skills.md): a task-first map of which skills are commonly used together
4. [Taxonomy](docs/taxonomy.md): the category system used throughout the public repository

If you want more context after that:

- [Skill Landscape](docs/skill-landscape.md)
- [Capability Gap Analysis](docs/capability-gap-analysis.md)

## Example Use Cases

### Literature review to related-work draft

Start with `literature-review`, `citation-management`, and `pyzotero`, then bring in `scientific-writing`.
This path helps you move from paper discovery and citation cleanup to a usable related-work section.

### Benchmark design to experiment tracking

Start with `benchmark-design`, `statistical-analysis`, and `get-available-resources`, then add `experiment-tracking`.
This helps you define fair evaluation rules before runs start and keep later comparisons interpretable.

### Code reproduction for a baseline paper

Start with `code-reproduction`, then combine it with `benchmark-design` and `experiment-tracking`.
This path helps you rebuild the environment, rerun results, and record where your outcomes match or diverge.

### LLM or agent workflow design

Start with `agent-coding`, `transformers`, and `markdown-mermaid-writing`, then add `modal` if deployment or cloud execution matters.
This supports moving from system design to implementation and evaluation planning.

### Repo cleanup before public release

Start with `repo-cleanup`, then use `github-release-prep` and `markitdown` where documentation or formatting cleanup is needed.
This path helps turn a messy research repo into something public-facing and easier to maintain.

## Attribution and License Notes

This repository includes both original materials and adapted materials.

- Source tracking and provenance: [ATTRIBUTION.md](ATTRIBUTION.md)
- Public release notices: [NOTICE.md](NOTICE.md)
- Repository license: [LICENSE](LICENSE)

The repository's original curation work, documentation, and repository-authored skills are released under the MIT License. Adapted and third-party materials included in this repository remain subject to their own licenses, notices, and attribution requirements as documented in their source metadata and in this repository's attribution files.

## Current Status

The public repository now has a screened skill set, a workflow-first taxonomy, a canonical skills catalog, and a task-oriented usage guide. English is the primary release language, and a structured Chinese mirror is available at `README.zh-CN.md`.
