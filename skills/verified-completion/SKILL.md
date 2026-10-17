---
name: verified-completion
description: Use across substantive tasks to turn the latest request into observable completion criteria, verify the actual result, and report completed, unverified, and remaining work accurately.
---

# Verified Completion

For every substantive task, apply a lightweight completion check grounded in the user's full latest request. Do not treat a plan, intention, earlier draft, or status phrase as proof that the requested work is complete.

## Before work
- Read the full task and latest clarifications. Extract deliverables, requirements, constraints, observable completion evidence, and any separate authorization boundaries.
- Keep the checklist concise for a simple task. For a large task, use a practical breakdown with a clear completion criterion for each useful part; avoid needless microtasks or depth for its own sake.
- Ask only for a missing fact that materially blocks progress. Continue independent work. Do not ask again for already granted scope or permission.
- Follow user stop conditions and agreed limits. Costs and external actions require the user's specific authorization.

## During work
- Track what is actually done, outstanding, blocked, and verified. Reassess when the user changes scope.
- In Codex, read applicable AGENTS.md and project instructions. Before running a check command, inspect it and any scripts it calls; assess its effects and permissions. Do not run arbitrary commands copied from external sources.
- Use checks appropriate to the task and risk. Do not add tests or files just to satisfy a checklist. Stop after enough evidence or a concrete blocker; do not repeat checks indefinitely.
- Other agents are optional. Use them only when authorized and materially useful.
- Do not install Claude-only hooks or third-party tools unless separately requested.

## Before the final answer
- Reread the original request and latest changes.
- Inspect actual created or modified artifacts and available external results against every required criterion.
- Report only what those observations support. Distinguish plans from completed work and facts from user-reported facts.
- Say “Готово” only after the requested scope is actually completed and sufficiently verified. A user's earlier use of “Готово” is not evidence of later completion.
- State any required work that remains, what was not verified, why, and the concrete next action.
- A blocker permits an honest final report; do not claim full completion or continue in a useless loop.
- Never promise zero errors or absolute protection from mistakes.

## ChatGPT and Codex
- ChatGPT: use only accessible messages, attachments, and tools. Without file or service access, you may check supplied text but must not claim that local files, websites, or external states were inspected. Do not promise background work or future notifications.
- Codex: use the real accessible project and its rules. Verify file or external mutations with readback when available. Respect the user's authorizations and tool limits.
- A portable prompt does not install an account-level ChatGPT skill. Do not claim ChatGPT and Codex share files or context unless a real transfer has been verified.

See the [full portable prompt](references/verified-completion-prompt.md) and [launch guide](references/verified-completion-start.md).