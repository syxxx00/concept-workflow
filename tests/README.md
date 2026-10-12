# Usage tests

English | [简体中文](README.zh-CN.md)

These two original synthetic tasks examine whether an agent uses relationships to shape a plan, produce usable content, and revise it when new materials arrive. They are separate from the skill's teaching example.

## Read the tasks and results

| Task | Initial prompt in English | Follow-up in English |
|---|---|---|
| Echo Workshop: card rules and a correction | [Task](translations/en/fixtures/resonance_card/task.md) | [Follow-up](translations/en/fixtures/resonance_card/followup.md) |
| Community Display: equipment, permission, and timing | [Task](translations/en/fixtures/shared_adapter/task.md) | [Follow-up](translations/en/fixtures/shared_adapter/followup.md) |

[Results](RESULTS.md) link to all 12 English artifact translations, including concepts, plans, and finished documents. Each translation links to its unchanged Chinese original. [Scoring criteria in English](translations/en/rubric.json) retain the original structure, task identifiers, and expectations; the [Chinese rubric](rubric.json) is preserved.

## What was actually run

The recorded runs used the Chinese prompts in [fixtures/](fixtures/) and the exact Chinese skill snapshot in [source-skill/](source-skill/SKILL.md). The original artifacts remain in [results/](results/). The current installable [English skill](../concept-workflow/SKILL.md) is translated from that snapshot. English files under `translations/en/` are reading translations prepared after the runs, not outputs from new English runs.

Each task was given to a separate AI subagent without the project's prior chat history. The agent was explicitly told where to read the skill. It received the initial prompt first, then the follow-up after its initial artifacts had been saved. It was not given the scoring rubric or expected answers. Both task prompts requested concept, plan, and finished documents, so that prompt structure also contributed to the work.

There was no comparison without the skill. The tests did not verify automatic discovery or installation, weaker models, performance across models, real-world use, or long-term maintenance. [Results and limitations](RESULTS.md) give the complete scope, including a gap found in the card prompt.

## Try your own run

Provide an agent with the installable skill and one initial prompt. Keep the follow-up, rubric, and saved answers out of its input until the initial work is complete. Save the initial artifacts, then provide the follow-up and save the revisions separately. Inspect the concrete decisions and corrections against the source materials and rubric.

A run using the English translations is a new run. Record its inputs and outputs separately from the original evidence here.
