# Changelog

所有重要变更都会记录在这里。

格式参考 [Keep a Changelog](https://keepachangelog.com/)，
版本号参考 [Semantic Versioning](https://semver.org/)。

## [Unreleased]

### Added
- 新增 `skills/` 目录，提供 Agent 可用的 skill
- 新增 `activity-organizer` skill，支持从零整理活动、详细版转简洁版、简洁版补全为详细版
- 新增 `docs/activity-template/`，含简洁版和详细版模板
- 新增 MIT License
- 新增 `CHANGELOG.md`

### Changed
- 每个活动结构统一为：`README.md`（简洁版）+ `details/`（详细版）
- 根 `README.md` 增加 Skills 说明

## [0.1.0] - 2026-10-16

### Added
- 初始化仓库
- 新增野K（野外K歌）活动指南
  - 简洁版：`activities/wild-karaoke/README.md`
  - 详细版：`activities/wild-karaoke/details/`
- 新增活动索引 `activities/README.md`
- 新增贡献指南 `CONTRIBUTING.md`
- 新增通用文档：
  - `docs/how-to-add-activity.md`
  - `docs/naming-conventions.md`