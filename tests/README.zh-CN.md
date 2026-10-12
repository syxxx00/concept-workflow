# 有限使用测试

简体中文 | [English](README.md)

检查模型是否把概念关系用于计划、具体产物和后继修正。两个情境均为原创合成材料，与 skill 教学案例分开。

| 任务 | 初始材料 | 后继材料 |
|---|---|---|
| 回声工坊：卡牌规则与局部纠正 | [task.md](fixtures/resonance_card/task.md) | [followup.md](fixtures/resonance_card/followup.md) |
| 社区展台：器材用途、许可与时间 | [task.md](fixtures/shared_adapter/task.md) | [followup.md](fixtures/shared_adapter/followup.md) |

每项任务由一个不继承项目旧会话的 AI 子代理执行，通过明确路径读取[当时的中文 skill](source-skill/SKILL.md)。先完成初作，再取得后继材料；接收者没有获得预期答案或[评分依据](rubric.json)。初作和后继均保留，便于比较改变与仍成立的部分。

实际产物、结果及原题的一处空缺说明见 [RESULTS.zh-CN.md](RESULTS.zh-CN.md)。初始任务本身要求概念、计划和产物三份文稿，因此这项提示也参与了工作。

当前可安装 skill 已整理为英文。[英文测试入口](README.md)提供四份任务材料、12份产物及评分依据的完整阅读译本，每篇译本可返回中文原件。中文原题、原产物和被测 skill 快照保留原样；翻译校对不构成新执行结果。

本测试未设置无 skill 对照，未验证自动发现与安装、弱模型、真实现场或长期维护。通过结果只支持对应材料和接收条件中的有限结论。
