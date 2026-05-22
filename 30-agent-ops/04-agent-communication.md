---
title: "Agent 间通信协议"
date: 2026-05-22
status: draft
version: v0.1-skeleton
---

# Agent 间通信协议

> ⚠️ **V0.1 骨架版**：通信协议框架。详细规则待 Randy 确认。

## 通信原则

1. **Silence ends conversations; @ restarts them.**
2. Agent 之间不互相感谢/签收——任务完成即结束
3. 需要协作时通过 Hermes 路由，不直接 @mention 形成循环

## 通信渠道

- **Multica Issue**：Agent 间的主要协作载体
- **飞书**：Randy 与 Agent 的交互入口
- **Obsidian Vault**：Agent 间的共享知识库（私有）

## 升级路径

```
Agent A 遇到问题
  → 先自查，尝试解决
  → 无法解决 → 标注清楚问题，升级给 Hermes
  → Hermes 判断 → 路由给合适的 Agent 或升级给 Randy
```

## 禁止行为

- ❌ Agent 之间互相 @mention 形成无限循环
- ❌ 在公开仓库讨论私有数据
- ❌ Agent 替其他 Agent 做角色外决策

---

> 📋 **待 Randy 确认**：
> - 通信协议是否需要补充？
> - 升级路径是否合理？
