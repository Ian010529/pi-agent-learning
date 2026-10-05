# Teaching Notes

## User learning preferences

- 核心形式：**Technical Foundation + 真实源码**，不能只做口头概念讲解。
- 每课先建立“读这段源码所需”的基础，再沿 Pi 当前实现走真实调用链。
- 喜欢“原理 + 例子 + 练习”，但练习必须服务于源码理解。
- 需要能串起来，而不是碎片化知识点列表。
- 学习目标是形成可迁移的 Agent 架构能力，不是记 Pi API。
- 对复杂概念优先用 execution trace、状态变化和小代码片段解释。
- Gate 需要 retrieval/application evidence；只看懂不算掌握。
- 源码/官方 docs 与字幕冲突时，必须显式指出，不静默修正。

## Course operating rule

每次开始新 lesson 前：
1. 读取 MISSION.md。
2. 读取已有 learning-records（如果已经出现）。
3. 确定当前 zone of proximal development。
4. 只引入当前 lesson 所需的 technical foundation。
5. 读取并引用当前 Pi primary source。
6. 结束时给 retrieval/application gate。
7. 只有用户通过后才写 learning record，并决定下一课。
