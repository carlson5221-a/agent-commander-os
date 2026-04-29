# Codex App 操作步骤

## 第一步：重新创建 GitHub repo

建议 repo 名称：

```text
agent-commander-os
```

这个名字比 sleep-agent-os 更适合长期战略，因为它不是绑定某一个品类，而是代表你的长期工作方式。

## 第二步：上传文件

最简单路径：

1. 下载本项目 zip
2. 解压
3. 打开 GitHub
4. 创建新 repo：agent-commander-os
5. 点击 Add file → Upload files
6. 把解压后的全部文件拖进去
7. Commit changes

注意：

GitHub 不能创建空文件夹。文件夹必须包含文件才会显示。

## 第三步：在 Codex App 里打开项目

根据 OpenAI 官方说明，Codex App 是用于并行运行 Codex threads、管理项目、使用 Git/worktree/automations 的桌面体验。你已经能在旧 Mac 上使用 Codex App，因此优先用 App 而不是网页端。

操作：

1. 打开 Codex App
2. 登录你的 ChatGPT / OpenAI 账号
3. 确认 GitHub 已连接
4. 选择或导入 repo：agent-commander-os
5. 新建一个 thread
6. 粘贴 README.md 里的第一条 Codex 任务

## 第四步：第一条 Codex 指令

复制：

```text
请阅读本 repo 的 README.md、05-workflows/7-day-demand-capture-loop.md 和 04-prompts/day1-demand-scan.md。
然后基于 02-scan-scope/first-scan-scope.md，生成第一轮需求扫描计划，并把结果写入 06-outputs/opportunity-list.csv。
不要修改目录结构。
```

## 第五步：你作为 Agent Commander 的工作方式

你不需要亲自改文件。

你的工作是给 Codex 下达类似这样的指令：

```text
今天只做 Day 2：需求扫描。
不要扩展系统，不要重构目录。
只输出 opportunity-list.csv，并在最后说明每条信号为什么值得关注。
```

## 第六步：每天复盘

每天让 Codex 更新：

```text
09-logs/daily-log.md
```

记录：

- 今天扫描了什么
- 发现了什么信号
- 哪些对象值得跟进
- 哪些假设需要修改
