# Computer Science LLM Agent Skills

![Skills](https://img.shields.io/badge/Skills-44-2ea44f)
![Focus](https://img.shields.io/badge/Focus-CS_LLM_Agent_Workflows-0969da)

一个面向 LLM agent 的计算机科研、学术写作、实验工作流与研究型软件工程 skills 仓库。

**语言：** [English](README.md) · **中文**

## 目录

- [这个仓库是什么](#repo-overview)
- [为什么使用这个仓库](#why-use-this-repo)
- [仓库包含什么](#whats-included)
- [如何开始](#getting-started)
- [如何使用这些 skills](#how-to-use-these-skills)
- [如何浏览](#how-to-browse)
- [典型使用场景](#example-use-cases)
- [来源与许可说明](#attribution-and-license-notes)

<a id="repo-overview"></a>
## 这个仓库是什么

这个仓库是一个面向工作流的公开 skills 集合，主要服务于：

- 计算机科研人员
- 计算机博士生
- research engineer
- 需要在论文、实验、代码与发布之间来回切换的 developer-researcher

它围绕计算机科研里反复出现的任务设计，例如：文献综述、论文写作、benchmark 设计、实验分析、模型工作流、agent 开发，以及 GitHub 发布前的仓库清理。

<a id="why-use-this-repo"></a>
## 为什么使用这个仓库

- **聚焦 CS 工作流**：面向计算机研究者和开发者真正反复会做的任务。
- **适合 agent 辅助工作**：这些 skills 的组织方式适合 coding / research agent 直接使用。
- **安装方式简单**：所有可安装的 skills 都直接放在一个 [`skills/`](skills/) 目录里。
- **浏览方式清晰**：既可以按目录看，也可以按任务看。
- **同时覆盖工具和工作流**：既有偏库和工具的技能，也有偏研究流程的技能。

## 适合谁

如果你的日常工作经常包含下面这些组合，这个仓库就是为你准备的：

- 文献阅读与 related work 整理
- 论文写作、改写、审稿与 rebuttal
- benchmark 设计与实验追踪
- 代码复现与结果分析
- ML、LLM、Graph、RL 或 agent 系统开发
- 仓库清理与 GitHub 公开发布准备

<a id="whats-included"></a>
## 仓库包含什么

- [`skills/`](skills/) 下共有 `44` 个公开 skills
- 一个可以直接整包复制的安装目录结构
- 一个记录每个 skill 的 `Primary Category`、`Task Tags` 和 `Type` 的公开索引

如果你关心某个 skill 属于 `Curated` 还是 `Custom`，可以直接看 [Skills Index](docs/skills-index.md)。

## 工作流覆盖范围

当前公开集合覆盖的核心工作流包括：

- 研究规划与任务拆解
- 文献综述与引用管理
- 论文写作、修改、审稿与 rebuttal
- benchmark、复现与实验运维
- 技术写作、markdown-first 文档与格式转换
- 数据工程、EDA、统计分析与可视化
- ML、LLM、Graph、RL 及相关计算工作流
- agent 系统与自动化开发
- slides、posters 与技术图示
- 仓库维护与开源发布准备

<a id="getting-started"></a>
## 如何开始

1. 如果你想用最简单的方式，直接把 [`skills/`](skills/) 里的全部内容复制到你的 agent skills 目录。
2. 如果你想用更精简的方式，先看 [`docs/skills-index.md`](docs/skills-index.md) 或 [`docs/usage-guide.md`](docs/usage-guide.md)，再只复制需要的 skills。
3. 如果 agent 不会自动发现新 skills，就重启或重新加载它。

<a id="how-to-use-these-skills"></a>
## 如何使用这些 skills

### 第一步：把全部 skills 复制到你的 skills 目录

把 [`skills/`](skills/) 里的文件夹复制到下面这些常见目录之一。你可以选择全局安装，也可以只在单个项目里安装。

**全局安装**（如果你希望所有项目都能直接用到这套 skills，推荐这种方式）：

| Tool | Directory |
| --- | --- |
| Cursor | `~/.cursor/skills/` |
| Claude Code | `~/.claude/skills/` |
| Codex | `~/.codex/skills/` |
| Gemini CLI | `~/.gemini/skills/` |

**项目级安装**（如果你希望 skills 只在一个项目中生效，推荐这种方式）：

| Tool | Directory |
| --- | --- |
| Cursor | `.cursor/skills/` |
| Claude Code | `.claude/skills/` |
| Codex | `.codex/skills/` |
| Gemini CLI | `.gemini/skills/` |

### 第二步：复制 `skills/` 里的全部内容

**示例：给 Cursor 做全局安装**

```bash
cp -r Computer-science-llm-agent-skills/skills/* ~/.cursor/skills/
```

**示例：给 Claude Code 做全局安装**

```bash
cp -r Computer-science-llm-agent-skills/skills/* ~/.claude/skills/
```

**示例：给 Codex 做全局安装**

```bash
cp -r Computer-science-llm-agent-skills/skills/* ~/.codex/skills/
```

**示例：给 Gemini CLI 做全局安装**

```bash
cp -r Computer-science-llm-agent-skills/skills/* ~/.gemini/skills/
```

**示例：项目级安装**

```bash
mkdir -p .codex/skills
cp -r /path/to/Computer-science-llm-agent-skills/skills/* .codex/skills/
```

如果你更想要一个精简安装，也可以只复制部分 skill 文件夹，而不是整个目录。

### 第三步：在 prompt 中使用这些 skills

安装好这些文件夹之后，正常向 agent 描述任务即可。如果你希望更明确地控制它调用哪些 skills，可以在 prompt 里直接点名。

Prompt 示例：

- `Use the literature-review, citation-management, and scientific-writing skills to turn these papers into a related-work outline.`
- `Use benchmark-design and experiment-tracking to define an evaluation plan for this repo.`
- `Use repo-cleanup and github-release-prep to make this project ready for public release.`
- `Use agent-coding and transformers to design a first version of this agent workflow.`

<a id="how-to-browse"></a>
## 如何浏览

建议先从这些公开文档开始：

1. [Skills Index](docs/skills-index.md)：标准公开目录，给出每个 skill 的 `Primary Category`、`Task Tags`、`Type` 和用途说明
2. [Usage Guide](docs/usage-guide.md)：从任务快速定位 skill 的最佳入口
3. [Task-to-Skills Mapping](docs/task-to-skills.md)：按任务组织的一组常用 skill 组合
4. [Taxonomy](docs/taxonomy.md)：整个公开仓库采用的分类体系

如果你还想看更完整的背景分析：

- [Skill Landscape](docs/skill-landscape.md)
- [Capability Gap Analysis](docs/capability-gap-analysis.md)

<a id="example-use-cases"></a>
## 典型使用场景

### 从文献综述走到 related-work 初稿

先使用 `literature-review`、`citation-management` 和 `pyzotero`，再接入 `scientific-writing`。
这条路径适合把论文检索、引用清理和 related work 起草串起来。

### 从 benchmark 设计走到实验追踪

先使用 `benchmark-design`、`statistical-analysis` 和 `get-available-resources`，再接入 `experiment-tracking`。
这条路径适合在实验开始前先把评价规则定清楚，并让后续结果更容易比较。

### 复现一篇 baseline paper

先使用 `code-reproduction`，再结合 `benchmark-design` 和 `experiment-tracking`。
这条路径适合重建环境、重跑结果，并记录哪里一致、哪里偏离。

### 设计一个 LLM 或 agent 工作流

先使用 `agent-coding`、`transformers` 和 `markdown-mermaid-writing`，如果涉及部署或云端执行，再补 `modal`。
这条路径适合从系统设计走到实现与评估规划。

### 在公开发布前清理 repo

先使用 `repo-cleanup`，再根据文档与整理需求补 `github-release-prep` 和 `markitdown`。
这条路径适合把一个混乱的研究仓库整理成更适合公开发布和长期维护的形式。

<a id="attribution-and-license-notes"></a>
## 来源与许可说明

这个仓库同时包含原创内容和整理改写后的内容。

- 来源追踪与归属说明：[ATTRIBUTION.md](ATTRIBUTION.md)
- 公开发布提醒：[NOTICE.md](NOTICE.md)
- 仓库级 license：[LICENSE](LICENSE)

本仓库中由本项目原创的策展结构、文档与仓库自带 skills 采用 MIT License。仓库中包含的改写内容与第三方材料，仍分别受其各自 license、notice 与 attribution 要求约束，具体以原始元数据和本仓库中的归属说明为准。

## 当前状态

目前这个公开仓库已经具备经过筛选的 skill 集合、面向工作流的 taxonomy、标准化 skills catalog，以及按任务组织的使用说明。当前主语言是英文，中文镜像已在本文件中提供。
