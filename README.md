# 开源活动策划

这里存放各种活动的流程整理与方法指导，目标是让办活动变得可复制、可协作、可迭代。

## 活动列表

| 活动 | 简介 | 人数 | 时长 |
|---|---|---|---|
| [野K（野外K歌）](activities/wild-karaoke/README.md) | 野外K歌，带上音箱和歌单一起唱 | 5–20 | 2–4h |
| （后续活动在此追加） |  |  |  |

## 仓库结构

```text
activity-guides/
├── README.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── LICENSE
├── docs/                   # 通用文档、规范、模板
├── skills/                 # Agent 可用的 skill
├── activities/             # 所有活动
└── assets/                 # 图片、海报等资源
```

## 每个活动的结构

```text
活动名/
├── README.md          # 简洁版
└── details/
    ├── README.md      # 详细版索引
    ├── roles.md
    ├── checklist.md
    ├── timeline.md
    └── templates/
```

- **简洁版**：一个文件看完，给没耐心的人
- **详细版**：拆分文件，方便细看、维护、复用

## Skills

仓库提供 Agent 可用的 skill，用来引导用户更方便地记录、整理活动。

| Skill | 作用 |
|---|---|
| [activity-organizer](skills/activity-organizer/SKILL.md) | 整理活动，生成简洁版 + 详细版，支持两版互转 |

支持场景：

- 从零整理活动：引导补全，生成简洁版 + 详细版
- 详细版 → 简洁版：读取 `details/`，浓缩成 `README.md`
- 简洁版 → 详细版：读取 `README.md`，引导补充，拆成 `details/`
- 登记活动：更新 `activities/README.md` 和根 `README.md`

使用方式：

- 对 Agent 说“帮我整理一个活动”
- Agent 读取 `skills/activity-organizer/SKILL.md`
- 按流程引导你补全信息
- 生成 `activities/<活动名>/README.md` 和 `details/`
- 自动登记到 `activities/README.md` 和根 `README.md`

更多见 [skills/README.md](skills/README.md)。

## 如何新增活动

见 [docs/how-to-add-activity.md](docs/how-to-add-activity.md)

## 如何贡献

见 [CONTRIBUTING.md](CONTRIBUTING.md)

## 变更日志

见 [CHANGELOG.md](CHANGELOG.md)

## 原则

- 实用优先
- 安全第一
- 可复制、可迭代
- 垃圾带走，不扰民