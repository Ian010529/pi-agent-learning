# Pi Agent Resources

## Knowledge

- [Pi current source: earendil-works/pi](https://github.com/earendil-works/pi)
  本课程的最高优先级事实来源。Use for: 所有实现细节、当前行为、文件结构与 design trade-off。

- [Pi Agent Core](https://github.com/earendil-works/pi/tree/main/packages/agent)
  通用 stateful agent、tool execution、event streaming。Use for: agent loop、message flow、tool calling、steering/follow-up、termination。

- [Pi Coding Agent](https://github.com/earendil-works/pi/tree/main/packages/coding-agent)
  把通用 Agent 组装成 coding harness。Use for: system prompt、coding tools、skills、extensions、sessions、compaction、MCP。

- [How Pi Works](https://github.com/earendil-works/pi/blob/main/packages/coding-agent/docs/how-pi-works.md)
  官方高层运行模型。Use for: 在进入源码前建立 session、branch、agent loop、context 的官方术语地图。

- [Matt Pocock: teach skill](https://github.com/mattpocock/skills/blob/main/skills/productivity/teach/SKILL.md)
  本仓库的教学方法来源。Use for: mission、short lessons、retrieval practice、learning records、zone of proximal development。

- **Uploaded subtitle: “Pi 大道至简，超越Codex和Claude Code的极简Agent，保姆级全攻略，一期视频精通”**
  Secondary explanatory reference only. Use for: 直觉、例子、视频中的学习线索。它不是当前 Pi 行为的权威来源；与当前源码冲突时必须标注差异并以源码为准。

## Wisdom (Communities)

- [Pi GitHub repository](https://github.com/earendil-works/pi)
  Use for: issues/PRs 中的真实设计讨论、边界条件和维护者决策。

- [Pi Discord](https://discord.com/invite/3cU7Bz4UPx)
  官方 README 提供的社区入口。Use for: 当源码不能回答“为什么这样设计”时寻找实践者/维护者语境。

## Gaps

- 视频字幕对应的 Pi 版本与当前主干并不完全一致；课程中遇到历史行为时，需要明确标成“historical/video claim”而不是自动套用到当前源码。
- 对某个设计动机若源码和官方文档都没有说明，不把推断写成事实；必要时再查 issue/PR/community。
