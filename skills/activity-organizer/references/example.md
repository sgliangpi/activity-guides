# 示例：用 activity-organizer 整理野K

## 示例一：从零整理活动

### 用户输入

“我想整理一个野外K歌的活动流程。”

### Agent 引导

1. 活动名称：野K（野外K歌）
2. 英文目录名：wild-karaoke
3. 一句话：找个不扰民、天气好、有厕所的地方，带上音箱和歌单，一起唱歌。
4. 人数：5–20 人
5. 时长：2–4 小时
6. 核心原则：不扰民、安全、低门槛、尽兴、垃圾带走

### 生成结果

```text
activities/wild-karaoke/
├── README.md          # 简洁版
└── details/
    ├── README.md
    ├── roles.md
    ├── checklist.md
    ├── timeline.md
    └── templates/
        ├── signup.md
        └── song-list.md
```

### 登记

- `activities/README.md` 追加一行
- 根 `README.md` 活动列表追加链接

---

## 示例二：详细版 → 简洁版

### 用户输入

“把野K的详细版浓缩成简洁版。”

### Agent 操作

1. 读取 `activities/wild-karaoke/details/`
2. 提取活动定位、快速流程、分工、提前准备、当天流程、安全、复盘
3. 生成或更新 `activities/wild-karaoke/README.md`
4. 顶部保留指向 `details/` 的链接
5. 提示用户确认

---

## 示例三：简洁版 → 详细版

### 用户输入

“根据野K的简洁版，帮我补一份详细版。”

### Agent 操作

1. 读取 `activities/wild-karaoke/README.md`
2. 识别缺失信息，向用户提问：
   - 分工是否要细化？
   - 检查清单是否要逐项列出？
   - 时间线是否要按阶段拆？
   - 是否需要报名模板、歌单模板？
3. 生成或更新 `activities/wild-karaoke/details/`
4. 在 `details/README.md` 顶部保留指向简洁版的链接
5. 提示用户确认

---

## 示例四：登记活动

### 用户输入

“把野K登记到活动列表。”

### Agent 操作

1. 更新 `activities/README.md`
2. 更新根 `README.md`
3. 提示用户确认