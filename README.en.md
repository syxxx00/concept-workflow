# Concept Workflow

[中文](README.md) | English

An AI skill that uses concepts to guide understanding, planning, creation, and revision.

It works from source materials to understand objects, relationships, uses, and conditions, giving concrete decisions a basis and revisiting them in light of actual results. A common path is “form concepts → make a plan → create content → revise from feedback.” Tasks that build on existing concepts can start at the relevant point.

## Usage

In a Codex environment that supports local skills, copy the entire [concept-workflow](concept-workflow/SKILL.md) folder into your user-level `.agents/skills/` directory, keeping the bundled references. If a skill with the same name already exists, compare versions and preserve the original files first.

> Use $concept-workflow to form a conceptual basis from these source materials, make a plan with clear deliverables, and create a concrete piece of content. Retain the understanding that still holds and review the work against actual results. Clearly identify any conditions you add.

You can also explicitly ask an agent to read `concept-workflow/SKILL.md` and the task materials. Image, audio, and code tasks still require the environment to provide the appropriate tools and materials.

The [worked example](concept-workflow/references/worked-example.md) (Chinese) shows how relationships inform reasoning and local corrections.

## Current evidence

Two AI subagents read the skill from an explicit path. Each completed an initial version and a follow-up revision for an original synthetic task. The task prompts, 12 actual artifacts, and limited findings are available in the [test overview](tests/README.md) and [test results](tests/RESULTS.md) (both in Chinese).

These tests did not establish automatic discovery or installation, reliability with less capable models, a net benefit over working without the skill, or real-world effectiveness.

## Origins and license

The [method lineage](provenance/method-lineage.md) (Chinese) explains what this package carries forward and organizes from the concept research. Feedback can include the task, materials, actual artifacts, and where a mismatch occurred.

Licensed under the [MIT License](LICENSE).
