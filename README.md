# Concept Workflow

English | [简体中文](README.zh-CN.md)

An AI skill for developing an understanding of objects and their relationships, using it to guide plans and concrete work, and revising it through feedback.

Here, a **concept** is an understanding you can use and develop further. It helps an agent reason, explore possibilities, and form new questions. A common path is **understand → plan → create → revisit**. Existing understanding and small tasks can enter at the relevant point.

## Use it

In a Codex environment that supports local skills, copy the entire [concept-workflow](concept-workflow/SKILL.md) folder into your user-level `.agents/skills/` directory, including its references. Compare versions before replacing an existing skill with the same name.

> Use $concept-workflow to develop a conceptual basis from these materials, make a plan with clear deliverables, and create a concrete piece of work. Retain what still holds, review the results, and clearly identify any conditions you add.

You can also ask an agent to read `concept-workflow/SKILL.md` and your task materials directly. Image, audio, and code tasks need the corresponding tools and source materials. The installable instructions and references are in English; you can state your task in your preferred language.

## See the method at work

Two workbench arms can share a base. Both arms being installed does not establish that they can run at once. If completing one task releases the base, a plan can connect the two tasks in sequence. A later requirement to close the workbench after each task changes that plan and its operating instructions.

The [worked example](concept-workflow/references/worked-example.md) shows the full progression, including revised instructions. It is a synthetic teaching example. [Concepts and the working model](concept-workflow/references/concept-and-model.md) explain the method in more detail.

## Evidence

Two AI subagents each completed an initial task and a follow-up revision, producing 12 original documents. The recorded runs used the [Chinese source version](tests/source-skill/SKILL.md) and Chinese prompts. The [test guide](tests/README.md) provides English reading translations of all prompts, artifacts, and scoring criteria; [test results](tests/RESULTS.md) explain the findings.

The current English skill is a translation of that source version. Translation review does not constitute a new English execution test. The recorded tests did not establish automatic discovery or installation, reliability across models, a net benefit over working without the skill, or real-world effectiveness.

## Origins and license

[Method lineage](provenance/method-lineage.md) explains the research background and related work. Feedback can include your task, materials, actual output, and where the understanding or result failed to fit.

Licensed under the [MIT License](LICENSE).
