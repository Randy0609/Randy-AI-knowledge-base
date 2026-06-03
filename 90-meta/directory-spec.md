---
title: "目录规范"
date: 2026-06-03
status: live
version: v1.0
---

# 目录规范

> 本文件定义 `Randy-AI-knowledge-base` 仓库的目录结构标准。所有贡献者（人类和 Agent）在新增文件或目录前，必须参照本规范。

---

## 一、编号体系

所有一级目录使用 `NN-category-name` 格式：

| 编号范围 | 用途 | 示例 |
|----------|------|------|
| `00-` | 入职与治理（onboarding / governance） | `00-onboarding/` |
| `10-` | 认知层（cognition / thinking） | `10-cognition/` |
| `20-` | 业务层（business / domain） | `20-business/` |
| `30-` | 运维层（ops / workflow） | `30-agent-ops/` |
| `40-` | 资产层（templates / assets） | `40-templates/` |
| `90-` | 元管理层（meta / repo management） | `90-meta/` |

### 规则

- 编号必须是 `NN-` 格式（两位数字 + 连字符）
- 编号不可重复
- 新增一级目录时，选择尚未使用的对应范围编号
- `90-` 保留给仓库自身管理文件，不用于业务内容

## 二、一级目录说明

### `00-onboarding/` — 入职与治理

**用途**：Agent 首次接入时的必读材料，以及仓库治理规则。

**包含**：
- Randy 公开画像
- Agent 入职指南
- 公开边界定义
- 行为规则和协作协议

**读者**：所有 Agent（必读）、人类协作者

### `10-cognition/` — 认知层

**用途**：Randy 的 AI 认知、思维方式、核心信念的结构化表达。

**包含**：
- AI Agent 体系认知框架
- 电商 AI 方法论
- 决策原则和思维模型

**读者**：需要理解 Randy 决策逻辑的 Agent 和协作者

### `20-business/` — 业务层

**用途**：具体业务领域的方法论和案例分析。

**包含**：
- 电商 AI 落地方法论
- 私域运营框架
- 品牌 AI 转型案例（脱敏）

**读者**：执行业务任务的 Agent、业务协作者

### `30-agent-ops/` — 运维层

**用途**：Agent 体系的运作规则。

**包含**：
- Agent 角色定义和职责边界
- 工作流和交付标准
- 考核评估方法
- Agent 间通信协议

**读者**：所有 Agent（必读）

### `40-templates/` — 资产层

**用途**：可复用的模板资产。

**子目录**：
- `delivery/` — 交付物模板（报告、方案文档）
- `prompts/` — 提示词模板（Agent 提示词、GPTs 配置）
- `tasks/` — 任务模板（需求描述、Bug 报告）

**读者**：执行类 Agent

### `90-meta/` — 元管理层

**用途**：仓库自身的维护和管理文档。

**包含**：
- 建设路线图
- Agent KPI 指标
- 目录规范（本文件）
- 违规记录

**读者**：仓库维护者、管理者 Agent

## 三、文件命名规范

### Markdown 文件

- 使用 `NN-short-name.md` 格式（如 `01-randy-profile.md`）
- 编号表示推荐阅读顺序
- 文件名使用小写英文 + 连字符（kebab-case）
- 不使用空格、中文、特殊字符

### 目录内 README

- 每个一级目录和二级目录**必须**包含 `README.md`
- 内容为所在目录的导航和说明
- 列出该目录下所有文件的简要描述

### 模板文件

- 模板文件使用描述性名称（如 `feature-request.md`）
- 不强制编号

## 四、Frontmatter 规范

每个 Markdown 文件必须在开头包含 YAML frontmatter，至少包含以下字段：

```yaml
---
title: "文件标题"
date: YYYY-MM-DD
status: draft | review | live | archived
version: vX.Y
---
```

### 字段说明

| 字段 | 必填 | 说明 |
|------|------|------|
| `title` | ✅ | 文件标题，用于自动索引 |
| `date` | ✅ | 创建或最后更新日期 |
| `status` | ✅ | `draft`（草稿）、`review`（待审）、`live`（生效中）、`archived`（归档） |
| `version` | ✅ | 语义化版本号 |
| `priority` | 可选 | 仅 `00-onboarding/` 中关键文件使用（如 `critical`） |

## 五、新增内容流程

1. **确定归属**：根据内容类型选择对应的一级目录
2. **检查边界**：对照 `00-onboarding/03-public-boundary.md` 确认内容可公开
3. **命名文件**：按本规范的命名规则命名
4. **添加 frontmatter**：按规范填写
5. **更新 README**：在所属目录的 `README.md` 中添加条目
6. **提交 PR**：提交到 `v0.1-skeleton` 分支，等待 CI 通过

## 六、禁止事项

- ❌ 不在一级目录下直接放大量文件（应使用二级目录或 README 导航）
- ❌ 不跳过编号规则自行命名一级目录
- ❌ 不在文件名中使用空格或中文
- ❌ 不删除或移动他人的核心骨架文件（除非有明确的 Randy 确认）
- ❌ 不在公开仓库放置二进制大文件（图片、PDF 等应外链）
