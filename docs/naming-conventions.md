# 命名规范

## 目录

- 活动目录：英文小写，单词间用 `-`，如 `wild-karaoke`
- 详细版目录：统一叫 `details`
- 模板目录：统一叫 `templates`
- 资源目录：统一叫 `assets`，按活动名再分一层

## 文件

- 简洁版：`README.md`
- 详细版索引：`details/README.md`
- 详细版文件：`roles.md`、`checklist.md`、`timeline.md`
- 模板：`signup.md`、`song-list.md` 等
- 图片：英文小写，单词间用 `-`

## 活动目录标准结构

```text
活动名/
├── README.md          # 简洁版
└── details/
    ├── README.md      # 详细版索引
    ├── roles.md
    ├── checklist.md
    ├── timeline.md
    └── templates/
        ├── signup.md
        └── song-list.md
```

## 提交信息

```text
feat: 新增野餐活动指南
fix: 修正野K预算说明
docs: 补充命名规范
```