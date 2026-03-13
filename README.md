# Creator Skills Repository

Language:
- [English](#english)
- [中文](#中文)

---

## English

### Vision

This repo is not just a prompt collection.
It is an **ecommerce skill infrastructure** for creators, sellers, affiliates, and operator teams.

We turn real commercial workflows into installable skills, then use usage feedback to decide what deserves productization inside **Creatop**.

### What this repository is building

A reusable skill layer for high-frequency ecommerce work:

1. discover demand
2. produce content faster
3. improve conversion quality
4. reduce policy/risk mistakes
5. standardize creator operations

This is our long-term flywheel:

**skills → usage signals → validated demand → product modules (Creatop)**

### Skill System Map

- **Market Intelligence**
  - trend sensing, topic selection, review mining, demand clustering
- **Content Production**
  - hooks, script generation, angle generation, variant planning
- **Conversion Ops**
  - comment replies, live objection handling, checkout/revenue friction analysis
- **Creator Collaboration**
  - creator selection, outreach, follow-up, brief quality control
- **Risk & Compliance**
  - monetization risk checks, claim-safe rewrites, policy-safe wording
- **Performance & Measurement**
  - attribution-lite, ROI checks, tracking and pricing diagnostics

### Latest shipped skills (recent wave)

- `affiliate-offer-angle-tester`
- `product-angle-ideas`
- `tiktok-content-ideas-refresh`
- `creator-brief-checker`
- `tiktok-live-reply-scripts` (renamed to plain-language style)
- `tiktok-comment-reply-templates` (renamed to plain-language style)
- `ugc-variants-generator`
- `creator-collab-checklist`
- `tiktok-claim-rewriter`
- `retention-drop-checker`
- `creator-payment-terms-template`
- `tiktok-affiliate-roi-calculator`
- `product-image-upscaler`
- `audio-to-text-caption`

Full catalog:
- Skills map: [`skills/INDEX.md`](skills/INDEX.md)
- Machine-readable registry: [`skills/manifest.json`](skills/manifest.json)

### Why this matters for ecommerce teams

Most ecommerce teams do not fail because they lack tools.
They fail because execution is fragmented:

- data and content teams speak different languages
- creator briefs are inconsistent
- conversion scripts are not reusable
- feedback loops are too slow

This repository provides a standardized skill layer to reduce that fragmentation.

### Quick Start

- Browse all skills: [`skills/INDEX.md`](skills/INDEX.md)
- Parse all metadata: [`skills/manifest.json`](skills/manifest.json)
- Propose demand: open issue with `New skill / use-case proposal`
- Co-build: https://qingjiu.me

### Invocation pattern (for OpenClaw / agents)

```text
Use <skill-slug> to <goal>.
Input: <data/source>
Constraints: <channel/risk/time>
Output: <format>
```

Examples:

1. `Use product-angle-ideas to generate 10 content angles for this product. Input: product facts + audience pain points. Output: ranked angles + hooks + test order.`
2. `Use tiktok-content-ideas-refresh to refresh next-week topics. Input: last 14 days post topics + comments. Output: 10 new topics + opening lines + 7-day plan.`
3. `Use creator-brief-checker to improve this campaign brief. Input: original brief + must-say points + restrictions. Output: risk list + copy-ready revised brief.`

### Release and quality principles

- One skill solves one concrete problem
- Plain-language naming beats jargon naming
- Every skill must have:
  - clear input/output contract
  - copy-ready template
  - risk boundaries (no fabricated claims)
- GitHub-first asset quality, ClawHub-second distribution cadence

### Repository structure

```text
skills/                    # skill folders + INDEX + manifest
research/                  # validation and optimization reports
tests/smoke/               # smoke artifacts
.github/ISSUE_TEMPLATE/    # structured demand intake
```

### Validation artifacts

- Baseline: `research/creator-skills-validation-report-2026-03-11.md`
- Smoke outputs: `tests/smoke/*.md`

---

## 中文

### 项目定位

这个仓库不是“提示词合集”，而是一个面向电商行业的 **Skills 基础设施**。

目标用户：
- TikTok 创作者
- 电商卖家与运营
- Affiliate 团队
- 需要标准化工作流的内容团队

我们把真实业务动作封装成可安装 skills，再用安装与使用反馈去验证需求，最终沉淀到 **Creatop** 产品能力里。

### 我们在做的事情

围绕电商高频工作流，持续建设技能层：

1. 需求洞察
2. 内容生产
3. 转化优化
4. 风险合规
5. 达人协作
6. 效果评估

长期飞轮：

**skills 发布 → 使用信号 → 需求验证 → Creatop 工具化**

### 技能体系地图

- **市场洞察（Market Intelligence）**
  - 趋势/选题/评论洞察/需求聚类
- **内容生产（Content Production）**
  - hook、脚本、角度、变体
- **转化运营（Conversion Ops）**
  - 评论回复、直播异议处理、转化漏损诊断
- **达人协作（Creator Collaboration）**
  - 达人筛选、触达、跟进、brief 质检
- **风控合规（Risk & Compliance）**
  - 违规表达检查、安全改写、变现风险控制
- **数据评估（Performance & Measurement）**
  - 轻量归因、ROI 预检、定价/追踪诊断

### 最近上线（最新一波）

- `affiliate-offer-angle-tester`
- `product-angle-ideas`
- `tiktok-content-ideas-refresh`
- `creator-brief-checker`
- `tiktok-live-reply-scripts`（已改为更口语化命名）
- `tiktok-comment-reply-templates`（已改为更口语化命名）

完整清单：
- 技能索引：[`skills/INDEX.md`](skills/INDEX.md)
- 机器可读清单：[`skills/manifest.json`](skills/manifest.json)

### 为什么这套 skills 对电商有意义

电商团队经常不是“不会做”，而是“无法稳定复用”：

- 数据和内容团队断层
- brief 标准不统一
- 回复脚本不可复用
- 反馈回路太慢

这个仓库在做的，就是把这些动作标准化、模块化、可复用化。

### 快速开始

- 看技能地图：[`skills/INDEX.md`](skills/INDEX.md)
- 看程序化清单：[`skills/manifest.json`](skills/manifest.json)
- 提需求：使用 `New skill / use-case proposal` issue 模板
- 共建入口：https://qingjiu.me

### Agent 调用格式建议

```text
Use <skill-slug> to <目标>
Input: <输入数据/来源>
Constraints: <限制条件>
Output: <输出格式>
```

示例：

1. `Use product-angle-ideas to generate 10 content angles...`
2. `Use tiktok-content-ideas-refresh to refresh next-week topics...`
3. `Use creator-brief-checker to improve this campaign brief...`

### 发布与质量规则

- 一个 skill 只解决一个明确问题
- 命名优先“大白话可搜索”，不堆术语
- 每个 skill 必须具备：
  - 输入输出契约
  - 可直接复用模板
  - 风险边界说明（不造假、不夸大）
- GitHub 先沉淀质量，ClawHub 按节奏分发

### 仓库结构

```text
skills/                    # SKILL 目录 + INDEX + manifest
research/                  # 验证与优化报告
tests/smoke/               # smoke 测试产物
.github/ISSUE_TEMPLATE/    # 结构化需求入口
```

### 验证材料

- 基线报告：`research/creator-skills-validation-report-2026-03-11.md`
- 测试结果：`tests/smoke/*.md`

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
