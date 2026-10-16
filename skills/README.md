# Skills

这里存放可供 Agent 使用的 skill，用来引导用户更方便地记录、整理、归档活动。

## 已有 Skill

| Skill | 作用 | 目录 |
|---|---|---|
| activity-organizer | 引导用户整理活动，生成简洁版 + 详细版，支持两版互转 | [activity-organizer/](activity-organizer/SKILL.md) |

## 什么是 Skill

Skill 是一份给 Agent 看的说明文档，通常包含：

- 何时使用
- 目标
- 工作流程
- 输出规范
- 注意事项

Agent 读取 skill 后，可以按固定流程引导用户，减少来回沟通成本。

## 目录规范

```text
skills/
└── skill-name/
    ├── SKILL.md          # 主文件，必须
    └── references/       # 参考资料，可选
        └── example.md
```

## 如何新增 Skill

1. 在 `skills/` 下新建目录，如 `skills/activity-organizer/`
2. 新建 `SKILL.md`，按下面结构写：

```markdown
---
name: skill-name
description: 一句话说明这个 skill 做什么、何时使用。
---

# Skill 名称

## 何时使用

## 目标

## 能力

## 工作流程

## 输出规范

## 注意事项
```

3. 如有参考资料，放到 `references/`
4. 在本文件表格中追加一行
5. 提交 PR

## 现有 Skill 说明

### activity-organizer

支持四种场景：

| 场景 | 说明 |
|---|---|
| 从零整理活动 | 引导补全，生成简洁版 + 详细版 |
| 详细版 → 简洁版 | 读取 `details/`，浓缩成 `README.md` |
| 简洁版 → 详细版 | 读取 `README.md`，引导补充，拆成 `details/` |
| 登记活动 | 更新 `activities/README.md` 和根 `README.md` |

输出结构：

```text
activities/<活动名>/
├── README.md          # 简洁版
└── details/
    ├── README.md      # 详细版索引
    ├── roles.md
    ├── checklist.md
    ├── timeline.md
    └── templates/
```

详细说明见 [activity-organizer/SKILL.md](activity-organizer/SKILL.md)。