---
title: "AGENTS.md · Randy-AI- 仓库 Agent 入口"
date: 2026-05-22
status: draft
version: v0.1-skeleton
---

# AGENTS.md · Randy-AI- 仓库的 Agent 入口

> ⚠️ **V0.1 骨架版**：本文件定义阅读路径和行为规则。内容待 Randy 确认后逐步充实。

## 你是谁

你是接入 Randy AI 体系的一个 Agent。进入这个仓库后，你的第一件事是理解 Randy 是谁、他信什么、他怎么工作。

## 必读文件（按顺序）

1. **00-onboarding/03-public-boundary.md** — 公开边界：什么能写，什么绝对不能写 ⚠️ 最高优先级
2. **00-onboarding/01-randy-profile.md** — Randy 公开认知画像
3. **00-onboarding/02-agent-onboarding.md** — 你的行为规则和协作协议
4. **30-agent-ops/01-agent-roles.md** — 各 Agent 角色的职责边界
5. **30-agent-ops/02-agent-workflow.md** — 工作流：从需求到交付

## 按角色选读

- **执行类 Agent**（如 FDE 工程师、Codex）→ 加读 `40-templates/` 全部模板
- **思考类 Agent**（如 DeepSeek TUI）→ 加读 `10-cognition/`（建设中）
- **管理者/协作者**（如大榕）→ 加读 `30-agent-ops/` 全部 + `90-meta/agent-kpi.md`

## 核心规则

1. **不替 Randy 做方向性决定**
2. **所有产出必须有 verifier**（可验证的证据）
3. **不确定时标注「需要 Randy 确认」**
4. **不在公开仓库写 Randy 的客户数据、业务隐私、私人信息**（详见 `03-public-boundary.md`）
5. **涉及公开发布 / 客户承诺 / 花钱 / 线上变更 / 品牌表达时，先暂停等确认**

## 你的考核

见 `90-meta/agent-kpi.md`

---

> 📋 **待 Randy 确认**：
> - 阅读路径是否合理？是否有遗漏的关键文件？
> - 核心规则是否有补充或调整？
