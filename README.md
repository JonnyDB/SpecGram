# SpecGram

SDD Kit for Kilocode

SpecGram is a collection of Kilo Code workflows integrated with a memory bank system, focused on enabling Spec-Driven Development
(SDD) directly in Kilocode without the need for external tools or modes. This
doesn't prevent the use of external tools, but it does mean that you can work
entirely within Kilocode if you want to.

SpecGram is inspired by and pulls heavily from
[Spec Kit](https://github.com/github/spec-kit) and
[BMAD](https://github.com/bmad-code-org/BMAD-METHOD) (both under MIT License).

A Kilo is made up of thousands from Grams. It's just a Spec. 😊

## Workflows

| Workflow Name | Description                                 |
| ------------- | ------------------------------------------- |
| specify       | Create a new feature specification          |
| plan          | Plan how to implement the specified feature |
| tasks         | Break down the plan into executable tasks   |
| implement     | Implements the spec tasks for the feature   |

## User Guide

### specify: Create new feature specs

**Brief usage instructions:** This workflow generates a detailed specification document for a new feature based on your description.

**Example command syntax:** `/specify "Add user authentication to the application"`

### plan: Generate implementation plans

**Brief usage instructions:** This creates a comprehensive implementation plan from the existing feature specification.

**Example command syntax:** `/plan`

### tasks: Break down into executable tasks

**Brief usage instructions:** Breaks down the implementation plan into specific, actionable tasks.

**Example command syntax:** `/tasks`

## implement: Execute spec implementations

**Brief usage instructions:** Executes the tasks to implement the feature according to the specification and plan.

**Example command syntax:** `/implement`
**Memory Bank Reference:** After completing workflows, use `update memory bank` to preserve context and insights for future sessions.

## Memory Bank Integration

This project uses a memory bank system to maintain context between sessions. See .kilocode/rules/memory-bank for details.

## Credits

Pulls directly and heavily from:

- [Spec Kit](https://github.com/github/spec-kit)
- [BMAD](https://github.com/bmad-code-org/BMAD-METHOD)

## Give it a try

Copy the `.kilocode` directory into your project. `.kilocodemodes` is 100% optional. It installs modes that are available from the Kilocode marketplace. They are not used by any of the core `/specify`, `/plan`, or `/tasks` workflows but can be helpful during implementation.
