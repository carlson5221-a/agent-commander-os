# IM 指挥话术模板

这些话术可以用于 Slack、飞书、企业微信，或直接复制到 Codex App。

## Day 1 指令

```text
请阅读 02-scan-scope/first-scan-scope.md 和 04-prompts/day1-demand-scan.md。
根据当前范围，生成第一轮需求扫描计划。不要开始写代码，先输出扫描策略和关键词。
```

## Day 2 指令

```text
请作为 Demand Scanner Agent 执行第一轮扫描。
目标是找到 100 个与 homecare/sleep/health devices 相关的动态需求信号。
请把结果写入 06-outputs/opportunity-list.csv。
```

## Day 3 指令

```text
请作为 Signal Analyst Agent，读取 06-outputs/opportunity-list.csv。
按 timing、fit、decision、value、accessibility 五个维度打分。
筛出 Top 20，写入 06-outputs/top20-targets.csv。
```

## Day 5 指令

```text
请作为 Trust Content Agent，读取 06-outputs/top20-targets.csv。
为每个对象生成 LinkedIn DM、Email 和 Website form 三种触达文案。
写入 06-outputs/outreach-messages.csv。
```

## Day 7 指令

```text
请作为 Review & Learning Agent，读取本周所有 outputs 和 logs。
总结哪些信号最有效、哪些客户类型最值得继续、下一轮应该调整什么。
写入 09-logs/week1-review.md。
```
