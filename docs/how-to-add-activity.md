# 如何新增一个活动

## 步骤

1. 复制 `docs/activity-template/` 到 `activities/你的活动名/`
2. 修改 `README.md`（简洁版）
3. 修改 `details/` 下详细版文件
4. 在 `activities/README.md` 表格中追加一行
5. 在根 `README.md` 活动列表中追加链接
6. 提交 PR

## 两份文档的关系

- `README.md`：简洁版，主入口，给没耐心的人看
- `details/`：详细版，给需要细看、维护、复用的人看

两份内容可以重复，但简洁版要能独立看懂。

## 两版互转

可以使用 `skills/activity-organizer/`：

- 详细版 → 简洁版：读取 `details/`，浓缩成 `README.md`
- 简洁版 → 详细版：读取 `README.md`，引导补充，拆成 `details/`

## 原则

- 每个活动必须有简洁版 `README.md`
- 详细版推荐有，但不强制
- 安全、合规、环保内容必须写
- 命名用小写英文，单词间用 `-`