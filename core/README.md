# core｜前端入口

与 `personal_os`、`finance_os`、`health_os` 同级。用户日常不必打开仓库，只聊天口述。本目录由 jason（示例角色）维护，是晨报和当日任务的前端。

全局规则见仓库根目录 `AGENTS.md`。开始使用时，请将 `state.template.md` 复制为 `state.md` 再填写。

| 文件 | 用途 |
|------|------|
| `state.md` | 当前状态（课程进度、复习排期、开放债、作息）。jason 每天晨间更新 |
| `state.template.md` | 空白状态结构，复制为 `state.md` 后使用 |
| `news.md` | 晨间简报（可选；用户说停就停） |
| `inbox.md` | 白天碎片；晨间 jason 归档后清空或移到已归档 |
| `oral_review_3line.md` | 晚间口述三行的提示：硬块 / 花费 / 一句 |
| `today_task.md` | 当日任务。jason 晨间按用户前一晚口述生成 |
| `today_task_template.md` | 日任务结构 |
| `weekly_YYYY-MM-DD.md` | 周报前端 |
| `Weekly_Report_Template.md` | 周报模板（趋势 + 债 + 三重点） |

## 节奏

1. 白天碎片进 `inbox.md`，或口头告诉 jason，晨间再归档。用户不必自己改 `today_task.md`。
2. 晚上（示例：约 22:30）口述三行和明天计划，发给 jason。不必打开本页。
3. jason **晨间**（示例：约 07:30）：清空 inbox → 归档昨天到 `05_Daily/`（按 `Daily_Template.md`）→ 更新 `state.md` → 生成**当天** `today_task.md` → 如仍启用则更新 `news.md`。聊天晨报不能代替仓库留档。
4. **周日晚（示例：约 21:00）**：周报进 `core/`，后端另存 `06_Review/`。聊天展示摘要。

## 生成约束（给 jason）

- 新页按模板字段写。硬块按用户前一晚口述；没给计划就写「计划未给」，不自己编一套。
- **开放债最多三条**，每条只写当前状态一行，不把多日历史整段粘贴进 today_task。
- 晨间清空 `inbox.md` 的待处理：归档后移到「已归档」或删掉。inbox 不写长复盘。
- 花费 / 收入 / 三餐钩子必须保留，供金融之狼与健康导师摘录。
- 勾选只在导师回【已练】之后。空白 ≠ 完成。

## 防冲突

- Path A（本机在线）先拉取再改。不把 Obsidian 工作区或未同步的财务草稿打进同一提交。详见根目录 `AGENTS.md` 第 10 节。
