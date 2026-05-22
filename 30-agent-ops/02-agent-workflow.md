---
title: "Agent 协作工作流"
date: 2026-05-22
status: draft
version: v0.1-skeleton
---

# Agent 协作工作流

> ⚠️ **V0.1 骨架版**：工作流框架。详细操作手册待 Randy 确认后填充。

## 核心流程（5 步）

```
Randy 提需求
  → 1. 收束（大榕：理解意图 → 收束成清晰任务）
  → 2. 判断（Hermes：判断风险 → 路由 → 生成 brief）
  → 3. 执行（下游 Agent：接收 brief → 实现 → 自检）
  → 4. 验收（Hermes：对照 verifier 验收结果）
  → 5. 写回（结果、判断、教训写回 Obsidian / GitHub）
```

## 风险闸门

以下情况必须先暂停等 Randy 确认：
- 涉及公开发布
- 涉及客户承诺
- 涉及花钱
- 涉及线上服务变更
- 涉及品牌表达

## 验收标准

没有 verifier 的任务不接。
Verifier 类型：测试结果 / 文件变更 diff / 部署 URL / 日志截图 / Randy 确认

## Agent 间通信

见 `04-agent-communication.md`

## 异常处理

- Agent 无法完成 → 升级给 Randy
- Agent 间冲突 → Hermes 仲裁
- 需求模糊 → 退回大榕澄清

---

> 📋 **待 Randy 确认**：
> - 5 步流程是否准确反映实际协作方式？
> - 风险闸门是否完整？
> - 异常处理机制是否足够？
