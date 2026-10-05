# Pi Agent Learning Roadmap

课程不是按 Pi UI 功能排列，而是按“从最小 agent core 到完整 harness”的依赖顺序排列。

| Lesson | Technical Foundation | Primary Source | Gate target |
|---|---|---|---|
| 01 Minimal Agent Loop | LLM message、tool calling、turn/loop、termination | `packages/agent/src/{types,agent,agent-loop}.ts` | 能闭卷恢复一次 tool-call execution trace |
| 02 Model Boundary | provider abstraction、streaming、normalized context | `packages/ai` + `streamAssistantResponse()` | 能解释为什么 model API 与 agent loop 分层 |
| 03 Tool Execution | schema validation、result protocol、sequential/parallel | `executeToolCalls*` + `core/tools/*` | 能从 tool declaration 推导执行与回灌过程 |
| 04 Agent State & Events | state、transcript、event lifecycle | `agent.ts`, `types.ts` | 能解释 state 与 event 各自解决什么 |
| 05 Steering & Follow-up | queue、interrupt、scheduling | inner/outer loop + queues | 能判断新消息在不同时间点何时进入 context |
| 06 Coding Harness | harness vs core、system prompt、tool loadout | `coding-agent/src/core/system-prompt.ts` + tools | 能说明 generic agent 如何成为 coding agent |
| 07 Skills | progressive disclosure、discovery、prompt injection | `core/skills.ts`, resource loader | 能解释 skill 与 tool/extension 的边界 |
| 08 Context & Compaction | context window、summary replacement | `core/compaction/*` | 能解释 compaction 改变 model context 但不抹掉 session history |
| 09 Extensions | hooks、custom tools、runtime extension | extensions docs/source | 能选对 extension point 而不是修改 core |
| 10 MCP & Tool Exposure | external tools、dynamic exposure、registry | MCP docs/source | 能解释 MCP 工具如何进入模型可见工具集合 |
| 11 Sessions & Branches | persistence、tree/branch、resume | `session-manager.ts`, `agent-session.ts` | 能从 session tree 重建 active model context |
| 12 Own Design: mini-Pi | boundary selection、trade-offs、eval | prior lessons | 设计并实现一个最小但可测试的 agent harness |

## Dependency rule

不因为“后面会用到”就提前塞内容。只有当前 lesson 的 gate 暴露出 gap，或下一段源码确实依赖某个概念时，才补 technical foundation。

## Current

- Lesson 01: **prepared**
- Learning gate: **not attempted**
- Learning records: **none yet**
