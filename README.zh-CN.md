# Computer Science Scientific Skills

![Curated Skills](https://img.shields.io/badge/Curated_Skills-34-2ea44f)
![Custom Skills](https://img.shields.io/badge/Custom_Skills-10-1f6feb)
![Public Skills](https://img.shields.io/badge/Public_Skills-44-8250df)
![Language](https://img.shields.io/badge/Language-Chinese--mirror-ffb000)
![Focus](https://img.shields.io/badge/Focus-CS_Research_Workflows-0969da)

一个面向计算机科研、学术写作、实验工作流与研究型软件工程的 curated skills 仓库。

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

这个仓库是一个**面向工作流的公开 skills 集合**，主要服务于：

- 计算机科研人员
- 计算机博士生
- research engineer
- 需要在论文、实验、代码与发布之间来回切换的 developer-researcher

它基于本地上游 skill 池构建，但**不是镜像仓库**，也不是一个泛科学技能大杂烩。公开目录只保留那些真正适合 CS 研究与编程工作的能力，例如：文献综述、论文写作、benchmark 设计、实验分析、模型工作流、agent 开发，以及 GitHub 发布前的仓库清理。

<a id="why-use-this-repo"></a>
## 为什么使用这个仓库

- **为 CS 工作流而策展**：关注的是计算机研究者反复会做的任务，而不是泛科学覆盖。
- **更少噪音，更高杠杆**：和你的方向弱相关或不适合公开发布的上游内容不会进入公开表面。
- **不仅有库技能，也有工作流技能**：补齐了 benchmark 设计、实验追踪、代码复现、reviewer response、release prep 等上游缺口。
- **更适合 agent 辅助工作**：帮助 coding / research agent 在论文、实验、代码和文档之间更稳定地切换。
- **更容易浏览与选择**：公开文档同时提供技能目录视图和任务入口视图。

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

- [`skills/curated/`](skills/curated/) 中有 `34` 个精选上游技能
- [`skills/custom/`](skills/custom/) 中有 `10` 个原创工作流技能
- 当前公开技能总数为 `44`

公开技能分成两类：

- **Curated**：从上游筛选并在需要时重写后的技能
- **Custom**：为了补齐真实 CS 研究工作流缺口而原创新增的技能

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

1. 先看 [`docs/skills-index.md`](docs/skills-index.md)，按分类、标签和用途找到相关 skills。
2. 如果你是从任务出发，例如写论文、做 benchmark 或清理 repo，就看 [`docs/usage-guide.md`](docs/usage-guide.md)。
3. 从 [`skills/curated/`](skills/curated/) 或 [`skills/custom/`](skills/custom/) 中挑出当前真正需要的少量 skills。
4. 只把这些 skill 文件夹复制到你的 agent 本地 skills 目录或项目级 skills 目录。

这个仓库面向的是那些能够在本地发现并使用 skill 文件夹的 coding / research agent 环境。

<a id="how-to-use-these-skills"></a>
## 如何使用这些 skills

一个 skill 本质上就是一个文件夹，里面至少包含 `SKILL.md`，也可能附带脚本、模板、参考资料和资源文件。实际使用时可以按下面的流程：

1. 先根据当前任务选出 `1-3` 个最相关的 skills。
2. 把这些 skill 文件夹复制到你的 agent skills 目录里。
3. 如果 agent 不会自动发现新 skills，就重启或重新加载它。
4. 正常向 agent 描述任务；如果你希望更可控，可以在 prompt 里直接点名要使用的 skill。

对于 Codex 风格的本地环境，常见目录是：

- 全局目录：`~/.codex/skills/`
- 项目级目录：`.codex/skills/`

安装示例：

```bash
mkdir -p ~/.codex/skills
cp -r skills/custom/research-planning ~/.codex/skills/
cp -r skills/curated/scientific-writing ~/.codex/skills/
```

Prompt 示例：

- `Use the literature-review, citation-management, and scientific-writing skills to turn these papers into a related-work outline.`
- `Use benchmark-design and experiment-tracking to define an evaluation plan for this repo.`
- `Use repo-cleanup and github-release-prep to make this project ready for public release.`

如果你使用的是其他支持 skills 的 agent，就把相同的 skill 文件夹复制到对应工具的 skills 目录即可。

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

## 这个仓库和上游有什么不同

- 它是**筛选后的集合**，不是镜像。
- 它围绕的是**CS 科研与编程工作流**，不是泛科学领域覆盖。
- 导入的 skills 在必要时会被**重写**，以更贴近 CS 场景。
- 公开集合中加入了**上游没有很好覆盖的原创工作流技能**。
- 文档结构围绕的是**任务选择与实用浏览**，而不是单纯的原始清单展示。

<a id="attribution-and-license-notes"></a>
## 来源与许可说明

这个公开仓库同时包含上游整理内容和原创补充内容。

- 来源追踪与归属说明：[ATTRIBUTION.md](ATTRIBUTION.md)
- 公开发布提醒与约束：[NOTICE.md](NOTICE.md)
- 仓库级 license：[LICENSE](LICENSE)

本仓库中由本项目原创的策展结构、文档与 custom skills 采用 MIT License。仓库中包含的上游整理内容与第三方材料，仍分别受其各自 license、notice 与 attribution 要求约束，具体以原始元数据和本仓库中的归属说明为准。

## 当前状态

目前这个公开仓库已经具备经过筛选的 skill 集合、面向工作流的 taxonomy、标准化 skills catalog，以及按任务组织的使用说明。当前主语言是英文，中文镜像已在本文件中提供。