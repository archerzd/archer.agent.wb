# archer.agent.wb

archer 的 WorkBuddy 智能体配置仓库 —— 备份并版本化管理 Agent 的身份定义与长期记忆。

## 目录结构

```
├── identity/          # 智能体身份定义
│   ├── SOUL.md        # 人格与行为准则（个性、边界、风格）
│   ├── IDENTITY.md    # 智能体名称等基础身份信息
│   └── USER.md        # 用户（archer）的基本档案
└── memory/            # 工作区记忆（按日期追加的工作日志）
    └── YYYY-MM-DD.md
```

## 同步约定

- `identity/` 中的文件修改后，需同步回 WorkBuddy 用户目录：
  `C:\Users\WS\.workbuddy\user-<uid>\`
- `memory/` 按 WorkBuddy 工作区 `.workbuddy/memory/` 的日志定期归档
- 记忆文件为追加式日志，不做覆盖改写

## 变更记录

- 2026-11-10 初始化仓库：迁入身份文件与首份工作日志
