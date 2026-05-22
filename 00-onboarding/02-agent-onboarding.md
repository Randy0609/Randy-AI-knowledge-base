---
title: "Agent 入职指南"
date: 2026-05-22
status: draft
version: v0.1-skeleton
---

# Agent 入职指南

> ⚠️ **V0.1 骨架版**：本文列出 Agent 入职流程和行为规则框架。具体操作手册待 Randy 确认后填充。

## Step 1：读完必读文件

按 `AGENTS.md` 中的必读文件列表，依次读完：
1. `03-public-boundary.md` — 先懂边界
2. `01-randy-profile.md` — 再懂 Randy
3. `30-agent-ops/01-agent-roles.md` — 再懂自己的角色
4. `30-agent-ops/02-agent-workflow.md` — 再懂怎么协作

## Step 2：理解你的角色

你的角色决定了你的权限边界。见 `30-agent-ops/01-agent-roles.md`。

核心原则：
- 每个 Agent 有自己的职责范围
- 不越权做不是你角色的事
- 不确定时问，不猜

## Step 3：学习工作流

从 Randy 提需求 → 收束 → 判断 → 执行 → 验收 → 写回的完整链路。
见 `30-agent-ops/02-agent-workflow.md`。

## Step 4：使用模板

执行任务时，优先使用 `40-templates/` 中的标准模板。

## 行为规则

### 必须做的
- 每次交付附带 verifier（可验证的证据）
- 不确定时标注「需要 Randy 确认」
- 涉及高风险操作时先暂停等确认（详见 `03-public-boundary.md`）
- 在公开仓库产出前，过一遍「Agent 产出检查清单」

### 不能做的
- 不替 Randy 做方向性决策
- 不编造 Randy 没提供的事实
- 不在公开仓库写入隐私数据
- 不使用 Randy 的禁用词

## 常用资源

- 模板：`40-templates/`
- 角色定义：`30-agent-ops/01-agent-roles.md`
- 工作流：`30-agent-ops/02-agent-workflow.md`
- 考核标准：`90-meta/agent-kpi.md`

---

> 📋 **待 Randy 确认**：
> - 入职流程是否完整？是否有遗漏的关键步骤？
> - 行为规则是否需要补充？
