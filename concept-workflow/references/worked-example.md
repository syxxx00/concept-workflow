# Worked example: two tasks on one workbench

This is a self-contained teaching example. Its author constructed the rules, task, content, and follow-up feedback. The written traces demonstrate relationships under those rules; they are not evidence from a real workbench, real participants, or a test of the skill's additional benefit. The example shows a complete bounded path. Its rules do not become requirements for other tasks.

## Input material and task

Task: Write a short instruction sheet from the rules below, allowing the same workbench to complete both the left and right tasks within one sequence of events. Keep the existing hardware.

Material M1: The workbench has an installed left arm and right arm that share one base. Their installed state does not change during this example's operations.

Material M2 (initial rules):

- Initially, permission to start is granted, the base is free, and neither task is complete.
- A task can start only while permission is granted, the base is free, and that task is not already complete. Starting it occupies the base.
- Completing the task in progress marks that side complete and releases the base.
- Closing the workbench revokes permission to start. It does not remove the arms or erase completion records. This version has no operation for reopening.
- There are no operations for repeating tasks or adding bases.

These rules are the entire basis for the example. There is no material about hardware dimensions, real durations, or user experience.

## Concept: connect objects and relationships

Both arms being installed means that both installation relationships hold in the same state. It does not prove that both tasks can start simultaneously. Starting a task competes for the base, but completing it releases the base. One side can therefore complete before the other within the same event history. Permission is a condition for starting; closing is an event that changes permission. A free base does not automatically restore permission.

The current anchor is: "Completion releases shared support, allowing the other side to start next." Left before right is a choice made by this instruction sheet's author. The rules also allow right before left; there is no permanent task priority.

## Plan: let relationships determine the arrangement

Use the shared-base relationship to choose a left → right sequence. Keep permission granted until both tasks complete, then close. The instruction sheet states the conditions for each start and supplies a trace to check that both completions occur in the same event history. No new hardware or entry point for repetition is needed. Do not infer simultaneous operation from installation alone.

## Content: the complete first instruction sheet

> **Workbench instruction sheet**
>
> Initial check: Permission to start is granted, the base is free, and neither task is complete.
>
> 1. Start the left task. It occupies the base while running, so the right task cannot start yet.
> 2. Complete the left task. Keep its completion record and confirm that the base has been released.
> 3. Start and then complete the right task.
> 4. Confirm that both tasks have completion records and that the base is free. Then close the workbench.
>
> Closing preserves the hardware and completion records. This version provides no entry point for starting again.

Complete trace under the rules:

| Event/state | Permission to start | Base | Left task | Right task |
|---|---|---|---|---|
| Initial state | Granted | Free | Incomplete | Incomplete |
| Start left | Granted | Occupied by left | In progress | Incomplete |
| Complete left | Granted | Free | Complete | Incomplete |
| Start right | Granted | Occupied by right | Complete | In progress |
| Complete right | Granted | Free | Complete | Complete |
| Close | Revoked | Free | Complete | Complete |

This trace supports completing both tasks and closing at the end in this example. It does not support repeated use, simultaneous operation, or claims about real experience. The first version is valid under the initial material.

## Feedback: new material changes the connections

The example's author then supplies M3 as a revised operating constraint: Immediately close after each side completes. After closing, only an inspector may reopen the workbench, after recording an inspection event. The material adds an explicit reopening entry point. It does not authorize the operator to skip the inspection.

This makes the first version's "complete left → immediately start right" sequence inapplicable. It does not erase the understanding of the shared base, installed hardware, or completion records. This is a rule revision; it does not retroactively make the first version violate rules that were unknown at the time.

Add the supporting relationships "close after completion" and "inspection event → inspector reopens" to the concept. Change the plan to insert closing, inspection, and reopening between the tasks, and update the content accordingly. Changing only the final note is insufficient. Do not assume that a free base grants permission. Without the inspector reopening it, this route stops with only the left task complete; it cannot be reported as completing both.

## Complete content after revision

> **Workbench instruction sheet: inspection and reopening**
>
> Initial check: Permission to start is granted, the base is free, and neither task is complete.
>
> 1. Start and complete the left task. Immediately close the workbench after completion. Keep the left completion record and hardware.
> 2. Have the inspector record the inspection event and reopen the workbench. Confirm that permission to start is granted and the base is free. Stop here if the workbench has not been reopened.
> 3. Start and complete the right task. Immediately close the workbench after completion.
> 4. Check both completion records and the final closed state.
>
> This sheet schedules each task once. Reopening between tasks depends on an actual action by the inspector. Closing at the end does not grant permission to repeat tasks.

Complete revised trace:

`Initial state → start left → complete left → close → record inspection → inspector reopens → start right → complete right → close`

Both arms remain installed throughout this trace. Each completion releases the base; each closure revokes permission. Reopening after inspection connects the left and right tasks. Both completion records remain at the end, and permission is revoked.

A plan that allows the inspector to reopen is still distinct from an event history in which reopening actually occurred. The trace above is the author's demonstration under the rules. In a real task, permission to reopen without an event record supports a feasible plan, not a claim of actual completion.

## Adjacent uses and unaffected scope

If the next task requires repeatedly running the left side, the existing completion marker prevents another start. Check the repetition rules separately; do not invent a reset operation. This new need does not automatically become part of the current delivery.

If the instruction sheet merely misstates "the right task cannot start yet" as "the right arm has been removed," correct the content directly; the concept and plan need no change. If both sides are required to run simultaneously, the shared base contradicts the current plan. Wording cannot turn sequential completion into simultaneous completion.
