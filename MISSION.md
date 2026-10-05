# Mission: Pi Agent

## Why
通过 Pi 当前真实源码建立对现代 Agent harness 的可迁移理解，而不是只会使用 Pi CLI。最终能够独立读懂、解释、修改 Pi 的核心执行链，并把其中值得保留的设计原则用于自己的轻量 Agent 设计与实现。

## Success looks like
- 不看资料也能画出 Pi 从 model provider 到 agent loop、tool execution、coding harness、session/compaction 的主要执行链。
- 能沿真实源码解释一次 user prompt 如何变成 LLM request、tool call、tool result 和下一轮 request。
- 能区分哪些能力属于通用 Agent core，哪些属于 coding harness、skill、extension、MCP 或 session 层。
- 能解释 Pi 关键设计选择的 trade-off，而不是只复述文件名或概念。
- 能独立设计并实现一个 mini-Pi，保留必要机制而不过度复制 Pi。

## Constraints
- 每课固定采用：Technical Foundation → Primary Source → Source Walkthrough → Execution Trace / Mental Model → Practice → Learning Gate。
- Technical Foundation 只讲阅读当前源码所需的最小知识，不做脱离源码的泛化 Agent 课程。
- Pi 当前源码和官方文档是事实来源；视频字幕只作辅助解释。
- 未通过 retrieval/application gate，不把“看过”记录成“学会”。
- 课程保持小步、可验证，避免一次塞入过多源码文件。

## Out of scope
- 现阶段不追求熟练 Pi TUI 快捷键、主题美化或所有 CLI 选项。
- 不把 Claude Code、Codex、OpenCode 等做成平行产品课程；只有在比较 Pi 设计取舍时才引入。
- 不为了“完整”而提前学习与当前源码链无关的 Agent 框架概念。
