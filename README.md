# Computer Science Scientific Skills

![Curated Skills](https://img.shields.io/badge/Curated_Skills-34-2ea44f)
![Custom Skills](https://img.shields.io/badge/Custom_Skills-10-1f6feb)
![Public Skills](https://img.shields.io/badge/Public_Skills-44-8250df)
![Language](https://img.shields.io/badge/Language-English--first-ffb000)
![Focus](https://img.shields.io/badge/Focus-CS_Research_Workflows-0969da)

A curated collection of reusable skills for computer science research, academic writing, experiment workflows, and research-oriented software engineering.

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

This repository is a **workflow-first public skill collection** for:

- computer science researchers
- PhD students
- research engineers
- developer-researchers who move between papers, experiments, code, and releases

It is built from a local upstream skill pool, but it is **not a mirror** and not a general science bundle. The public set is curated for recurring CS work: literature review, paper writing, benchmark design, experiment analysis, model workflows, agent development, and GitHub-ready repository cleanup.

## Why Use This Repository

- **Curated for CS workflows**: it focuses on the actual tasks CS researchers repeat, not generic scientific coverage.
- **Less noise, more leverage**: weak-fit or irrelevant upstream material is kept out of the public surface.
- **Workflow skills, not only library skills**: original additions cover gaps such as benchmark design, experiment tracking, code reproduction, reviewer response, and release prep.
- **Built for agent-assisted work**: the repository helps a coding or research agent operate more reliably across papers, experiments, code, and documentation.
- **Easy to browse**: the public docs give you both a skill catalog view and a task-first workflow view.

## Who It Is For

Use this repository if your work regularly involves combinations of:

- literature review and related-work synthesis
- paper drafting, revision, review, and rebuttal
- benchmark design and experiment tracking
- code reproduction and result analysis
- ML, LLM, graph, RL, or agent system development
- repository cleanup and public GitHub release preparation

## What's Included

- `34` curated upstream-derived skills in [`skills/curated/`](skills/curated/)
- `10` original custom skills in [`skills/custom/`](skills/custom/)
- `44` public skills total

The public inventory is split into:

- **Curated**: upstream-derived skills that survived CS-focused screening and, when necessary, rewriting
- **Custom**: original workflow skills added to cover gaps that matter in real CS research and engineering practice

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

1. Browse [`docs/skills-index.md`](docs/skills-index.md) to find relevant skills by category, tags, and use case.
2. Use [`docs/usage-guide.md`](docs/usage-guide.md) if you want to start from a task such as paper writing, benchmark design, or repo cleanup.
3. Pick a small set of relevant skills from [`skills/curated/`](skills/curated/) or [`skills/custom/`](skills/custom/).
4. Copy only those skill folders into your agent's local skills directory or project-level skills directory.

This repository is designed for skill-aware coding and research agent environments where local skill folders can be discovered and used during work.

## How to Use These Skills

### Step 1: Choose the skills you need

Start by picking a small set of skills that match your current workflow.

- Use [`docs/skills-index.md`](docs/skills-index.md) if you want to browse by category, tags, and use case.
- Use [`docs/usage-guide.md`](docs/usage-guide.md) if you want to start from a task such as paper writing, benchmark design, or repo cleanup.
- In most cases, `1-3` skills are enough for a single task.

### Step 2: Copy skills to your skills directory

Copy the individual skill folders from [`skills/curated/`](skills/curated/) or [`skills/custom/`](skills/custom/) to one of the common skill directories below. You can install skills globally or per-project.

**Global installation** (recommended for skills you use across projects):

| Tool | Directory |
| --- | --- |
| Cursor | `~/.cursor/skills/` |
| Claude Code | `~/.claude/skills/` |
| Codex | `~/.codex/skills/` |
| Gemini CLI | `~/.gemini/skills/` |

**Project-level installation** (recommended when skills should stay inside one repo):

| Tool | Directory |
| --- | --- |
| Cursor | `.cursor/skills/` |
| Claude Code | `.claude/skills/` |
| Codex | `.codex/skills/` |
| Gemini CLI | `.gemini/skills/` |

If your agent uses a different directory convention, copy the same skill folders into that tool's configured skills directory.

### Step 3: Copy the specific skills you want

**Example: global install for Cursor**

```bash
cp -r Computer-science-scientific-skills/skills/curated/literature-review ~/.cursor/skills/
cp -r Computer-science-scientific-skills/skills/curated/scientific-writing ~/.cursor/skills/
```

**Example: global install for Claude Code**

```bash
cp -r Computer-science-scientific-skills/skills/custom/benchmark-design ~/.claude/skills/
cp -r Computer-science-scientific-skills/skills/custom/experiment-tracking ~/.claude/skills/
```

**Example: global install for Codex**

```bash
cp -r Computer-science-scientific-skills/skills/custom/research-planning ~/.codex/skills/
cp -r Computer-science-scientific-skills/skills/curated/scientific-writing ~/.codex/skills/
```

**Example: global install for Gemini CLI**

```bash
cp -r Computer-science-scientific-skills/skills/custom/repo-cleanup ~/.gemini/skills/
cp -r Computer-science-scientific-skills/skills/custom/github-release-prep ~/.gemini/skills/
```

**Example: project-level install**

```bash
mkdir -p .codex/skills
cp -r /path/to/Computer-science-scientific-skills/skills/custom/agent-coding .codex/skills/
cp -r /path/to/Computer-science-scientific-skills/skills/curated/transformers .codex/skills/
```

### Step 4: Use the skills in your prompt

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

## How This Repo Differs from Upstream

- It is **screened**, not mirrored.
- It is organized around **CS research and programming workflows**, not broad scientific domain coverage.
- Imported skills are **rewritten when necessary** to match CS use cases more closely.
- The public set includes **original workflow-native skills** that upstream did not cover well.
- The docs are structured for **task selection and practical browsing**, not just raw inventory listing.

## Attribution and License Notes

This public repository includes both upstream-derived material and original additions.

- Source tracking and provenance: [ATTRIBUTION.md](ATTRIBUTION.md)
- Public release reminders and constraints: [NOTICE.md](NOTICE.md)
- Repository license: [LICENSE](LICENSE)

The repository's original curation work, documentation, and custom-added materials are released under the MIT License. Upstream-derived and third-party materials included in this repository remain subject to their own licenses, notices, and attribution requirements as documented in their source metadata and in this repository's attribution files.

## Current Status

The public repository now has a screened skill set, a workflow-first taxonomy, a canonical skills catalog, and a task-oriented usage guide. English is the primary release language, and a structured Chinese mirror is now available at `README.zh-CN.md`.