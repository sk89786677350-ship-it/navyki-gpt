---
name: project-continuity
description: Use when continuing an ongoing project across Codex or ChatGPT, after a meaningful milestone or decision, before a pause, or when the user asks to save or prepare continuation context.
---

# Project Continuity

Preserve accurate, portable project state so work can resume after a pause or move between Codex and ChatGPT. Use the full [continuity prompt](references/project-continuity-prompt.md) for detailed layouts, commands, and handoff wording.

## Scope and triggers

- Apply to ongoing multi-step work, significant project decisions, direction changes, resume requests, and pauses. A casual one-off task does not require project records.
- After each meaningful completed stage, important decision or direction change, and before pausing, briefly offer to save the current stage and prepare a ChatGPT handoff when the current state is not already saved and nothing material has changed.
- Do not repeat the offer after every message or when the saved checkpoint is still current.
- An offer is not a save. Update records only after the user says “сохрани”, “сохрани глобально”, or explicitly agrees to the exact proposed scope.

## Save and resume

- For “сохрани”, save the requested state to the real project files available in the authorized workspace. If the user names a file or target, use that target.
- For “сохрани глобально”, save project state in its project location and separately record only the explicitly authorized general rules through the available permitted global-memory mechanism. Never move private project facts into global guidance.
- Do not invent a project path, create placeholder project folders, or create MEMORY.md, GOALS.md, PROJECTS.md, journals, or README files unless the user requested a project context folder or those specific files.
- A checkpoint records facts only: project and goal, date, completed work and artifacts, accepted decisions and constraints, current stage, unfinished work, open questions/dependencies, next concrete step, and verified links/results. Keep history append-only where appropriate; update summaries without silently erasing important decisions.
- Read the latest accessible checkpoint before resuming. Briefly state the actual goal, stage, and next action. Follow the user's latest instruction if it supersedes an older record. If records are inaccessible or conflict, ask only for the missing fact needed to continue.
- Verify every requested file or record after saving. Say it is saved only after confirming the actual result. If writing is unavailable, provide a ready-to-copy checkpoint and state that no file was written.

## Codex and ChatGPT boundary

- In Codex, read and write only files actually accessible in the authorized project location. Never imply that a local Lenovo folder is automatically available in another chat or service.
- In ChatGPT, use only the tools and files that are actually available. If there is no authorized storage/transfer tool, prepare a portable summary for the user to copy or attach; do not claim that it was saved to ChatGPT memory.
- Do not create a new chat, send a message to another chat or person, publish, or incur costs as a side effect of saving. Each requires separate explicit authorization.
- Treat user-provided project documents as the source of project facts; do not invent user identity, history, goals, approvals, completed work, or test results. Do not put passwords, tokens, or other secrets in checkpoints.
