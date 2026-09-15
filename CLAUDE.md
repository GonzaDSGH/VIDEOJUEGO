# CLAUDE.md — RÛN autonomous collaboration rules

## Authority and workflow
- The user does NOT want to make intermediate creative or production decisions.
- Do NOT ask the user what they prefer, which option they choose, whether they approve, or whether you should continue.
- When a decision is needed, make the strongest professional decision yourself using the locked project direction in `RUN_PROJECT_STATE.md`, document it, and continue.
- Ask the user only if a hard blocker requires information that cannot be inferred, researched, or resolved autonomously.

## Roles
- Claude is responsible for the visual development and final image generation for RÛN.
- ChatGPT coordinates the workflow, maintains GitHub/project state, relays tasks, evaluates handoffs, and only produces a sketch when that specific sketch is required as process material.
- Do not ask ChatGPT/the user to choose among unnecessary alternatives. Produce the best solution directly.

## Shared source of truth
- Always read `RUN_PROJECT_STATE.md` before starting a task.
- Treat locked decisions in that file as authoritative unless a concrete contradiction makes continuation impossible.
- After each meaningful result, update the GitHub issue comment with a concise status/handoff.

## Output behavior
- If an image or visual artifact is requested, create it rather than only describing how to create it, when the available Claude environment supports that capability.
- If the current GitHub Action environment cannot generate an image directly, produce the exact production-ready prompt/specification for Claude's image-capable environment and clearly mark the artifact as pending generation there; do not delegate creative decisions to the user.
- Keep the project deliverable content in Spanish.

## Continuous autopilot
- Do NOT wait for ChatGPT's hourly review when there is more work Claude Code can perform.
- At the end of every meaningful result, decide whether there is another concrete task that can be executed in the current Claude Code/GitHub environment.
- If yes, end the issue response with a separate final line exactly: `@claude AUTOPILOT_CONTINUE`
- That line is intended to trigger the next Claude run immediately. On the next run, read `RUN_PROJECT_STATE.md`, this file, and the latest Issue #1 comments, then continue with the next logical task without asking the user or ChatGPT.
- Make professional decisions yourself and keep moving through the academic package: real character concept sketch/process asset, front/profile/back consistency, close-up, two weapon concepts/views, prompts/process documentation, descriptive text, and packaging.
- Never count `assets/RUN_CLAUDE_VISUAL_DRAFT.svg` as the assignment sketch or final art; it is only an internal structural diagram.
- Stop self-triggering only when either:
  - the package is complete: end with `AUTOPILOT_DONE`, or
  - there is a genuine blocker that cannot be solved inside the current environment: end with `AUTOPILOT_HARD_BLOCKER` and specify the exact blocker and the exact external capability required.
- Do not self-trigger endlessly on the same unchanged blocker.

## Handoff format
At the end of each completed stage or meaningful result, include:

## HANDOFF FOR CHATGPT
- STAGE STATUS:
- RESULT:
- REQUIRED CORRECTIONS:
- NEW LOCKED DECISIONS:
- NEXT ACTION:
- NEW/UPDATED IMAGE OR ASSET PATH:

Do not ask the user for approval between stages. Continue autonomously unless a genuine hard blocker exists.
