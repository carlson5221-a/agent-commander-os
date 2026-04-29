# Agent Commander OS

这是一个面向「中国供给 × 世界需求 × Agent Commander」的最小可运行 Agent OS 仓库。

第一阶段目标不是做复杂系统，而是跑通一个真实业务闭环：

> 需求扫描 → 信号判断 → 客户筛选 → 触达准备 → 反馈复盘

## 项目定位

- 面向对象：SME / 外贸型供给侧 / homecare & health devices 等可验证品类
- 核心任务：发现正在发生的需求，而不是简单堆积 sales leads
- 工作方式：人定义 What 和 Why，Agent 执行 How
- 第一目标：每7天输出一批可触达的高质量潜在机会

## 目录结构

```text
00-identity/        你的长期定位与对外表达
01-strategy/        战略假设、业务第一性、目标函数
02-scan-scope/      首轮需求扫描范围
03-agents/          Agent 角色说明
04-prompts/         可直接给 Codex / ChatGPT / Claude 使用的 Prompt
05-workflows/       7天业务闭环流程
06-outputs/         输出表格模板
07-im-commands/     IM 指挥话术模板
08-codex-setup/     Codex App 与 GitHub 操作说明
09-logs/            每日记录与复盘
```

## Codex 第一条任务建议

把下面这段复制到 Codex App：

```text
请阅读本 repo 的 README.md、05-workflows/7-day-demand-capture-loop.md 和 04-prompts/day1-demand-scan.md。
然后基于 02-scan-scope/first-scan-scope.md，生成第一轮需求扫描计划，并把结果写入 06-outputs/opportunity-list.csv。
不要修改目录结构。
```
