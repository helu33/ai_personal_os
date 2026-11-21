# 财务 OS

个人财务信息与记账空间，由「金融之狼」（示例角色）维护。

全局规则见仓库根目录 `AGENTS.md`。真实账本、资产和收入数据请留在私有处，不要公开。

## 结构

- `profile.template.md` — 复制为 `profile.md` 后填写收入、存款、负债、偏好（宜私有）
- `fixed-costs.template.md` — 复制为 `fixed-costs.md` 后填写固定月支出
- `assets.template.md` — 复制为 `assets.md` 后填写资产摘要
- `ledger/` — 日常流水（按月）
- `goals/` — 大额消费与储蓄目标
- `advice/` — 阶段性建议归档

数据来源：用户口头报花费（日常不必打开仓库）。jason（示例角色）写入 `../core/today_task` 后，金融之狼按日期 / 金额 / 用途记账。

约定：本目录只记账本与建议，不改 `core/today_task`。
