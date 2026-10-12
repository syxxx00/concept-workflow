# Test results

English | [简体中文](RESULTS.zh-CN.md)

2026-10-13. Two original synthetic tasks each produced an initial version and a follow-up revision, with 12 original documents saved. The AI subagents read the [Chinese source skill](source-skill/SKILL.md) from an explicit path and received Chinese task materials. A separate AI subagent that did not create the tasks or produce the answers checked the artifacts item by item and found no substantive errors.

The links below provide complete English reading translations, each linked to its unchanged Chinese original. They are not outputs from new English runs. The current installable English skill is also a translation; the recorded results apply to the Chinese source version.

## Results

Card values below are **Luo / Lan** (洛 / 岚).

| Task | Initial result | Follow-up revision |
|---|---|---|
| Echo Workshop | Case A: 13 / 0; B: 7 / 0; C: 2 / 6. Payment occurs before an entry is added to the pending list. Removing the source does not cancel existing entries. The reward goes to the operator recorded when the entry was created. | Case A starts with 5. The first payment leaves 2, so the second operation cannot be paid for. Remove the incorrectly recorded second operation and its echo; keep the first operation's two entries. Case A ends at 8 / 0. Cases B and C and the device descriptions remain unchanged. |
| Community Display | The Blue Box holds a fixed entrance sign; visitors can flip the White Box to read the routes. Four clamps, borrowing periods, and the staffing window support the arrangement. | The White Box's new permission ends before the display does. The team uses its own folding display board to show both routes on one face. The quiet route marker changes to a green square. The White Box is not used for display and is returned at 11:18. The entrance sign and short route remain unchanged. |

## Read the artifacts in English

- Echo Workshop, initial: [concept](translations/en/results/resonance_card/initial/CONCEPT.md), [plan](translations/en/results/resonance_card/initial/PLAN.md), [rules](translations/en/results/resonance_card/initial/RULES.md); follow-up: [concept](translations/en/results/resonance_card/followup/CONCEPT.md), [plan](translations/en/results/resonance_card/followup/PLAN.md), [rules](translations/en/results/resonance_card/followup/RULES.md).
- Community Display, initial: [concept](translations/en/results/shared_adapter/initial/CONCEPT.md), [plan](translations/en/results/shared_adapter/initial/PLAN.md), [display document](translations/en/results/shared_adapter/initial/DISPLAY.md); follow-up: [concept](translations/en/results/shared_adapter/followup/CONCEPT.md), [plan](translations/en/results/shared_adapter/followup/PLAN.md), [display document](translations/en/results/shared_adapter/followup/DISPLAY.md).

The [original artifacts](results/) are preserved without edits. The [test guide](README.md) links the prompts and scoring criteria and explains the recorded setup.

## A gap in the card prompt

The prompt specified that echo entries go on top, but did not specify where manually generated entries are inserted. The recipient identified this gap and completed what could be determined. The rubric initially assumed a unique total order for all four entries. Checking the prompt led to withdrawing that unsupported requirement while retaining checks for echo placement, payment timing, attribution, trigger counts, and final values. The task, follow-up, and skill were not changed for this correction, and the recipient received no extra answer. This was a correction to the test design.

## Scope of the findings

For these two sets of materials and this explicit reading setup, the executors produced inspectable concepts, plans, and content, then applied the follow-up conditions to revised artifacts. The initial prompts also requested these three documents, so the entire workflow cannot be attributed to the skill.

These tests did not verify automatic discovery, installation, or implicit invocation; reliability with weaker models or across models; or the translated English skill. The exact engine version was not independently confirmed. There was no comparison without the skill, so its independent net benefit cannot be determined. Card playtesting, equipment installation, sensory experience, reading photographs, returning equipment on site, long-term maintenance, and general human-like conceptual ability are outside the evidence from these tests.
