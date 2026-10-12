# Concept Workflow

用概念组织理解、计划、制作与修正的 AI skill。

它从材料中认识对象、关系、用途和条件，让具体取舍有依据，再根据实际结果返回修正。常见路径是“形成概念 → 制定计划 → 制作内容 → 根据反馈修正”；已有概念的局部任务可以从有关位置进入。

## 使用

支持本地 skill 的 Codex 环境可将整个 [concept-workflow](concept-workflow/SKILL.md) 文件夹复制到用户的 `.agents/skills/` 下，保留随附参考。已有同名 skill 时，先比较版本并保留原文件。

> 使用 $concept-workflow，根据这些原材料形成概念依据，制定有明确交付点的计划，并完成一段具体内容。沿用仍成立的理解，根据实际结果复查；补入的条件请保持可辨认。

也可明确让智能体读取 `concept-workflow/SKILL.md` 和任务材料。图像、音频或代码任务仍需要环境提供相应工具与资料。

[教学案例](concept-workflow/references/worked-example.md)展示关系怎样参与推导和局部纠正。

## 当前证据

两个 AI 子代理通过明确路径读取 skill，分别完成一项原创合成任务的初作与后继修正。原题、12 份实际产物及有限结论见 [测试说明](tests/README.md)和[测试结果](tests/RESULTS.md)。

这些测试未验证自动发现与安装、弱模型可靠性、相较不使用 skill 的净增益，或真实现场效果。

## 来路与许可

[方法来路](provenance/method-lineage.md)说明本包从 concept 研究中继承和整理的范围。反馈可以附上任务、材料、实际产物及发生失配的位置。

采用 [MIT License](LICENSE)。
