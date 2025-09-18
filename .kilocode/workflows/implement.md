---
name: implement
mode: orchestrator
description: Implements the spec tasks for the feature.
allowed-tools: read_file, search_files, list_files, apply_diff, write_to_file, execute_command, switch_mode, new_task, ask_followup_question, attempt_completion, update_todo_list
argument-hint: <implementation_instructions>
---

<switch_mode>
<mode_slug>orchestrator</mode_slug>
<reason>Always start in Orchestrator mode for high-level planning.</reason>
</switch_mode>

## Steps

Your TODO list is as follows. Use the sections below for detailed instructions.

1. Setup
2. Implement Tasks

### 01. Setup

Using `read_file`, read the `{FEATURE_DIR}/tasks.md` file to understand the
tasks to be implemented.

Each task must be tracked as a todo AND updated in `tasks.md`.

### 02. Implement Tasks

`switch_mode` to `orchestrator` mode to plan the implementation of each task.

use `code` mode to implement each task.

Each todo must be executed using `new_task` and must
maintain its own todo list. Always validate each task completion with tests.
Use TDD principles. Automatically switch to the `code-reviewer` mode to review
complex code changes. Use the `test-engineer` mode to create and run tests.
Simplify complex code with the `code-simplifier` mode. Do multiple passes if
needed to complete each task fully before moving to the next.

Each task must
be tracked as a todo. Each todo must be executed using `new_task` and must
maintain it's own todo list. Always validate each task completion with tests.
Use TDD principles. Automatically switch to the `code-reviewer` mode to review
complex code changes. Use the `test-engineer` mode to create and run tests.
Simplify complex code with the `code-simplifier` mode. Do multiple passes if
needed to complete each task fully before moving to the next.

ALWAYS: After each task is completed, update the tasks list in
`{FEATURE_DIR}/tasks.md` as you complete each task so that it reflects the
current state.

NEVER attempt to run a completed task again. Mark it complete and move on to the
next.

## OPTIONAL: Git Checkpoint

If and only if `--git-checkpoint` is provided in the arguments, create a git
checkpoint after each task is completed. Use the task ID and a brief summary of
the task as the commit message. For example, for task T001, the commit message
might be "T001: Implement user authentication".
