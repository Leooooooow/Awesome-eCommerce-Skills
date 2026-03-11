# Creator Skills Repository

Language:
- [English](#english)
- [中文](#中文)

---

## English

### Overview

A **continuously growing** skills collection for creators, sellers, and AI operators.

Goal: turn real ecommerce workflows into installable skills, validate demand fast,
and continuously convert winning skills into Creatop-native tools.

### Quick Start

- Browse skills map: [`skills/INDEX.md`](skills/INDEX.md)
- Programmatic registry: [`skills/manifest.json`](skills/manifest.json)
- Propose new demand: `New skill / use-case proposal` issue template
- Co-build link: https://qingjiu.me

### How to get more OpenClaw / agent calls

Important: automatic skill selection is primarily driven by each skill’s
`SKILL.md` frontmatter (`name` + `description`), not repository README alone.

Use this invocation format when calling from OpenClaw or other agents:

```text
Use <skill-slug> to <goal>.
Input: <data/source>
Constraints: <channel/risk/time>
Output: <format>
```

Copy-ready examples:

1. `Use creator-search-intent-radar to rank this week’s topics. Input: these 30 comments + TikTok trend notes. Output: top 10 topics with hooks and CTA.`
2. `Use short-video-hook-lab to improve first 3 seconds. Input: this draft script. Output: 5 ranked hooks with rationale.`
3. `Use creator-monetization-risk-checker to audit this script. Input: full script text. Output: risk flags + safer rewrites.`
4. `Use comment-to-content-recycler to convert audience feedback into backlog. Input: these comments/DM snippets. Output: intent clusters + priority list.`
5. `Use ugc-brief-to-script-engine to convert this sponsor brief into creator-native scripts. Output: 3 angle variants with shot list.`

### For creators & sellers

Use these skills to quickly improve:
- topic selection quality,
- short-video hooks,
- script compliance safety,
- outreach conversion, and
- weekly execution speed.

Recommended first 3:
1. `creator-search-intent-radar`
2. `short-video-hook-lab`
3. `creator-monetization-risk-checker`

### For developers

This repo is built as a rolling, test-driven skill lab:
- each skill has clear input/output contracts,
- demand capture is structured via issue forms,
- winning patterns are fed into Creatop product workflows.

### Current published skills (rolling list, currently 10)

| Skill | Core problem solved |
|---|---|
| `creator-search-intent-radar` | What to post next based on demand signals |
| `short-video-hook-lab` | How to improve first-3-second retention |
| `creator-deal-ops` | How to run sponsor deals with less friction |
| `cross-platform-recut-planner` | How to repurpose one idea across platforms |
| `creator-monetization-risk-checker` | How to reduce monetization/distribution risk |
| `ugc-brief-to-script-engine` | How to turn briefs into creator-native scripts |
| `creator-attribution-lite` | How to connect content actions to outcomes |
| `batch-content-sprint-os` | How to ship weekly without burnout |
| `creator-proof-portfolio-builder` | How to package proof for outreach |
| `comment-to-content-recycler` | How to convert comments into content pipeline |

### Next demand batch (staged release)

The following 10 skills are now in staged release (GitHub first, ClawHub in waves):

- `tiktok-shop-creator-fit-scorer`
- `review-defect-miner`
- `listing-gap-audit`
- `shopify-tracking-auditor`
- `price-gap-monitor`
- `refund-reason-cluster`
- `ugc-hook-analyzer`
- `checkout-friction-audit`
- `promo-calendar-optimizer`
- `creator-outreach-sequence-lab`

- `tiktok-live-objection-handler`

### Repository structure

```text
skills/               # SKILL.md folders + INDEX + manifest
research/             # validation and optimization reports
tests/smoke/          # smoke-test outputs
.github/ISSUE_TEMPLATE/ # structured demand intake templates
```

### Validation

- Baseline report: `research/creator-skills-validation-report-2026-03-11.md`
- Per-skill artifacts: `tests/smoke/*.md`

---

## 中文

### 项目概览

这是一个**持续增长**的技能集合，面向创作者、电商卖家与 AI 运营团队。

目标是把真实电商工作流做成可安装的技能，快速验证需求，并把高价值技能持续沉淀为 Creatop 原生工具能力。

### 快速开始

- 技能总览：[`skills/INDEX.md`](skills/INDEX.md)
- 程序化清单：[`skills/manifest.json`](skills/manifest.json)
- 提交需求：使用 `New skill / use-case proposal` 模板
- 共建入口：https://qingjiu.me

### 如何获得更多 OpenClaw / 其它 Agent 调用

关键点：Agent 的自动技能选择，主要看每个技能的 `SKILL.md` 前置元数据
（`name` + `description`），README 主要用于人类理解和转化。

建议统一使用下面这种调用格式：

```text
Use <skill-slug> to <目标>。
Input: <输入数据/来源>
Constraints: <限制条件>
Output: <输出格式>
```

可直接复制的示例：

1. `Use creator-search-intent-radar to rank this week’s topics. Input: 30条评论+趋势摘要. Output: Top10选题+hooks+CTA.`
2. `Use short-video-hook-lab to improve first 3 seconds. Input: 当前脚本. Output: 5个排序后的开头方案+原因.`
3. `Use creator-monetization-risk-checker to audit this script. Input: 完整脚本. Output: 风险点+安全改写.`
4. `Use comment-to-content-recycler to convert comments into backlog. Input: 评论和私信片段. Output: 意图聚类+优先级内容池.`
5. `Use ugc-brief-to-script-engine to convert sponsor brief to scripts. Output: 3个角度+分镜shot list.`

### 给创作者与卖家

这套技能主要帮助你提升：
- 选题质量
- 短视频前 3 秒表现
- 脚本合规性
- 外联转化
- 周度执行效率

建议先从这 3 个开始：
1. `creator-search-intent-radar`
2. `short-video-hook-lab`
3. `creator-monetization-risk-checker`

### 给开发者

这个仓库是滚动迭代、测试驱动的 skill lab：
- 每个技能都有明确输入/输出契约
- 通过 issue 模板结构化收集需求
- 把验证有效的模式回流到 Creatop 产品工作流

### 当前已发布技能（滚动更新，当前 10 个）

| Skill | 解决的核心问题 |
|---|---|
| `creator-search-intent-radar` | 下一条内容该发什么 |
| `short-video-hook-lab` | 如何提升前 3 秒留存 |
| `creator-deal-ops` | 如何更稳地管理品牌合作流程 |
| `cross-platform-recut-planner` | 如何把一个创意跨平台重剪 |
| `creator-monetization-risk-checker` | 如何降低变现/分发风险 |
| `ugc-brief-to-script-engine` | 如何把 brief 变成可拍脚本包 |
| `creator-attribution-lite` | 如何做轻量归因和结果回看 |
| `batch-content-sprint-os` | 如何周更不断更且不过载 |
| `creator-proof-portfolio-builder` | 如何整理案例证明提升合作转化 |
| `comment-to-content-recycler` | 如何把评论/私信变成选题池 |

### 下一批需求技能（分批发布）

以下 10 个技能已进入分批发布（先 GitHub，后 ClawHub 分波次）：

- `tiktok-shop-creator-fit-scorer`
- `review-defect-miner`
- `listing-gap-audit`
- `shopify-tracking-auditor`
- `price-gap-monitor`
- `refund-reason-cluster`
- `ugc-hook-analyzer`
- `checkout-friction-audit`
- `promo-calendar-optimizer`
- `creator-outreach-sequence-lab`

### 仓库结构

```text
skills/               # SKILL.md 目录 + INDEX + manifest
research/             # 验证与优化报告
tests/smoke/          # smoke 测试输出
.github/ISSUE_TEMPLATE/ # 结构化需求模板
```

### 验证材料

- 基线报告：`research/creator-skills-validation-report-2026-03-11.md`
- 单技能测试结果：`tests/smoke/*.md`

---

## Build with me / 一起共建

Hi, I’m **Leroy (Razestar)**. I’m building AI-native growth systems for ecommerce creators.

你好，我是 **Leroy（Razestar）**，在做面向电商创作者的 AI 增长系统。

If you want to co-build new skills, propose high-value workflows, or collaborate:

如果你想一起共建技能、提出高价值工作流、或发起合作，欢迎联系：

👉 https://qingjiu.me

---

## License & commercial use

Copyright (c) 2026 **Razestar**.

This bundle is licensed for public community use under
**CC BY-NC-SA 4.0 (Attribution-NonCommercial-ShareAlike)**.

- Non-commercial use: allowed (with attribution to Razestar)
- Adaptations: allowed under same license
- Commercial use: requires separate paid commercial license

See `LICENSE`, `NOTICE`, `COMMERCIAL.md`, `TRADEMARKS.md`.
