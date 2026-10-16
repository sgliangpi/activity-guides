# 贡献指南

感谢你愿意为这个仓库做贡献。这里的目标是把办活动变成一件可复制、可协作、可迭代的事。

## 可以贡献什么

- 新增活动类型
- 优化已有活动流程
- 补充检查清单、模板、经验
- 修正错误、补充安全提示
- 改进文档结构、命名规范

## 新增活动

见 [docs/how-to-add-activity.md](docs/how-to-add-activity.md)

简要步骤：

1. 复制 `docs/activity-template/` 到 `activities/你的活动名/`
2. 修改简洁版 `README.md`
3. 修改详细版 `details/`
4. 在 `activities/README.md` 表格中追加一行
5. 在根 `README.md` 活动列表中追加链接
6. 提交 PR

## 提交方式

1. Fork 仓库
2. 新建分支，如 `feat/add-picnic-guide`
3. 提交改动
4. 发起 PR，说明改了什么、为什么

## 提交信息建议

```text
feat: 新增野餐活动指南
fix: 修正野K预算说明
docs: 补充命名规范
```

## 如何更新 CHANGELOG

`CHANGELOG.md` 用来记录仓库的重要变更，方便别人快速了解改了什么。

### 什么时候更新

- 新增活动
- 活动流程大改
- 新增 skill
- 结构调整
- 模板更新
- 重要修复

小改动可以攒一攒，发版本时一起写。

### 怎么更新

1. 在 `## [Unreleased]` 下按分类加一条：
   - `### Added`：新增
   - `### Changed`：修改
   - `### Fixed`：修复
   - `### Removed`：删除
2. 发版本时，把 `## [Unreleased]` 改成具体版本号，如 `## [0.2.0] - 2026-11-01`
3. 在上面新开一个空的 `## [Unreleased]`

### 版本号怎么定

语义化版本 `MAJOR.MINOR.PATCH`：

| 变化 | 版本 |
|---|---|
| 不兼容的大改 | MAJOR +1 |
| 新增活动、skill、功能 | MINOR +1 |
| 修复、小改 | PATCH +1 |

### 示例

```markdown
## [Unreleased]

### Added
- 新增野餐活动指南

### Changed
- 优化野K预算说明

### Fixed
- 修正野K详细版链接
```

## 原则

- 实用优先
- 安全第一
- 可复制、可迭代
- 环保：垃圾带走，不破坏场地