---
title: "README · Randy-AI认知库"
date: 2026-06-03
status: live
version: v0.2-base
---

# Randy-AI 认知库

> **Randy 的公开 AI 认知库** — 面向未来 Agent、协作者和公众的方法论、框架、模板集合。
>
> 仓库地址：[Randy-AI-knowledge-base](https://github.com/Randy0609/Randy-AI-knowledge-base)
>
> 📍 当前版本：**V0.2 基建版** — 目录结构、核心骨架和 CI 基建已就位，内容持续填充中。

---

## 这是什么

本仓库是 Randy AI 体系的**公开知识层**。它沉淀了 Randy 在 AI Agent 协同、电商 AI 系统构建、一人 AI 团队组织等方面的认知、方法和可执行资产。

它与 Randy 的私有 Obsidian Vault 是镜像关系——但**不是 1:1 复制**。公开仓库只输出方法论和框架，不包含业务隐私、客户数据和个人信息。

## 谁应该读

| 角色 | 入口 | 读什么 |
|------|------|--------|
| 🤖 **AI Agent**（任何接入 Randy 体系的 Agent） | [AGENTS.md](./AGENTS.md) | 按指引顺序阅读必读文件 |
| 👤 **人类协作者**（合作伙伴、团队成员） | 本文件 | `00-onboarding/` 了解 Randy 画像和边界 |
| 🌐 **公众/路人**（对 AI Agent 协同感兴趣的人） | 本文件 | 按目录浏览感兴趣的方法论和模板 |

## 如果你是一个 Agent

👉 从 **[AGENTS.md](./AGENTS.md)** 开始。那是你的入职入口，定义了必读文件、阅读顺序和行为规则。

## 仓库结构

```
Randy-AI-knowledge-base/
├── README.md                         ← 你在这里（人类入口）
├── AGENTS.md                         ← Agent 第一入口（必读）
│
├── 00-onboarding/                    ← Agent 入职与公开边界
│   ├── 01-randy-profile.md           → Randy 公开认知画像
│   ├── 02-agent-onboarding.md        → Agent 行为规则和协作协议
│   └── 03-public-boundary.md         → ⚠️ 公开边界（最高优先级）
│
├── 10-cognition/                     ← Randy 的 AI 认知（建设中）
│
├── 20-business/                      ← 电商 AI 业务方法论（建设中）
│
├── 30-agent-ops/                     ← Agent 运维
│   ├── 01-agent-roles.md             → 各 Agent 角色职责边界
│   ├── 02-agent-workflow.md          → 工作流：从需求到交付
│   ├── 03-agent-assessment.md        → Agent 考核评估标准
│   └── 04-agent-communication.md     → Agent 间通信协议
│
├── 40-templates/                     ← 可执行模板
│   ├── delivery/                     → 交付物模板
│   ├── prompts/                      → 提示词模板
│   └── tasks/                        → 任务模板
│
├── 90-meta/                          ← 仓库自身管理
│   ├── repo-roadmap.md               → 建设路线图
│   ├── agent-kpi.md                  → Agent KPI 指标
│   └── directory-spec.md             → 目录规范（本文档的标准定义）
│
└── .github/workflows/                ← CI 配置
    └── lint.yml                       → Markdown 格式检查
```

### 目录编号规则

- **`00-`**：入职与治理（onboarding / governance）
- **`10-`**：认知层（cognition / thinking）
- **`20-`**：业务层（business / domain）
- **`30-`**：运维层（ops / workflow）
- **`40-`**：资产层（templates / assets）
- **`90-`**：元管理层（meta / repo management）

详见 [`90-meta/directory-spec.md`](./90-meta/directory-spec.md)。

## 使用方法

### 浏览知识库

1. **按目录浏览**：从上面的仓库结构找到你感兴趣的领域
2. **按角色阅读**：参考「谁应该读」表格
3. **搜索**：使用 GitHub 搜索或 `grep` 关键词定位

### 贡献内容

1. 阅读 `00-onboarding/03-public-boundary.md` 确认内容可公开
2. 参照 `90-meta/directory-spec.md` 确定文件放置位置
3. 使用 `40-templates/` 中的对应模板
4. 提交 PR 到 `v0.1-skeleton` 分支
5. CI 会自动运行 Markdown 格式检查

## 当前状态

- **V0.2 基建版**：17 个核心骨架文件 + CI 基建 + 目录规范
- **默认分支**：`v0.1-skeleton`
- **下一步**：Randy 审阅确认后 → V0.3 内容填充

## 三条铁律

1. **不搬运 Obsidian 原样内容** — 公开仓库只写方法论层
2. **所有 Agent 产出前先过公开边界检查清单** — 见 `00-onboarding/03-public-boundary.md`
3. **不确定的内容标注「需要 Randy 确认」** — 不编造 Randy 没说过的话
