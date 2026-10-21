---
name: project-repository-sync
description: Use when saving, sending, publishing, syncing, or closing project work across a local project folder and a GitHub or other Git repository, including cloud tasks that need to continue on the local computer.
---

# Project and Repository Sync

## Purpose

Keep the project folder on the local computer and its explicitly matched remote repository consistent, preserve a portable handoff, and report exactly what was synchronized. A user command authorizes only the action its wording and the standing cloud-task rule cover.

## Workflow

### 1. Identify the project and destination

- Identify the current project folder, project purpose, active branch, and configured remotes using the current environment's available tools.
- Match a remote to the project using explicit user selection or corroborating project metadata. A familiar-looking name, stale README, or stale mapping alone is not enough. If evidence leaves any doubt, preserve work locally and ask the user to confirm the exact repository link or owner/name before publishing.
- Only after the user confirms there is no remote or the candidate is not the project repository, offer creation with a proposed name and visibility; wait for selection or approval before creating it. For a verified existing project, provide the repository link when useful.
- Support GitHub and other configured Git remote services through available tools or Git. If the service cannot be reached or written to, report the exact unsatisfied step; do not claim the project is synced.

### 2. Interpret the save request

- On the local computer, “save” alone means persist the current local work and update the portable handoff; do not push unless the user also says send, publish, sync, or names a repository.
- On the local computer, “save and send to GitHub/repository” or an equivalent explicit instruction authorizes a routine commit and push to the verified matching remote, within this workflow's safeguards.
- For a cloud project task, the user's standing rule requires saving completed changes to the verified matching repository before claiming the task is closed. If a candidate repository exists but is still unverified, ask only for its exact link or owner/name; do not offer a new repository as a substitute. Offer creation only after the user confirms there is no remote or the candidate is not this project's repository, then wait for the user's selection or approval.

### 3. Inspect both sides before changing either

- Record the current branch and working-tree status. Fetch remote metadata where supported; inspect the relevant target branch and pending changes.
- Compare project file inventories and content in both directions. Identify files present locally but absent remotely, files present remotely but absent locally, changed files on each side, and conflicts.
- Preserve every uncommitted local change. Never use destructive reset, clean, force-push, blind checkout, or overwrite to make the trees look equal.
- If independent additions can be reconciled without replacing different content, carry each missing file to the other side and verify it.
- If the same path differs on both sides, do not replace either copy. Preserve each version in its existing environment, capture a diff or safe side-by-side snapshot if possible, and stop for the user's choice. Do not claim full sync.

### 4. Remove only proven duplicates

- A candidate duplicate must be byte-for-byte identical and redundant in the project's structure. Same name, similar appearance, or similar text is not proof.
- Before removing a copy, check references, build/configuration usage, and whether the path is part of an intentional distribution. Keep one canonical copy and update references if needed.
- If redundancy or references cannot be established, preserve the files and report the candidates. Never delete distinct versions or user data as a cleanup shortcut.

### 5. Protect the repository

- Review all additions and changes before staging. Exclude credentials, tokens, private keys, `.env` secrets, personal data, machine-specific absolute paths, and unrelated files.
- Do not publish or copy secrets into a handoff or logs, even when the user says to send everything or the repository is private. If a secret is already tracked, do not silently rewrite history; report the exposure and recommend credential rotation and a separately planned history cleanup. State clearly that the sync excluded the secret-bearing file.
- Keep `PROJECT_HANDOFF.md` portable: summarize project purpose, completed work, important decisions, current branch or change reference, validation performed, and next steps. Do not put private local paths, credentials, or unrelated conversation content in it.

### 6. Save and verify

- For a clear matching repository and an authorized send/sync request or cloud-task close, stage only reviewed project files, create a descriptive commit or the closest supported saved change, and push to the intended branch when the available environment permits. Do not merge into a protected/default branch unless the user specifically requests that.
- If the environment supports only a patch, review, or pull request, use that supported route and identify its state accurately. A draft, local commit, or open pull request is not a completed push/merge.
- Verify the remote contains the intended change using the remote service or a fresh fetch/inspection, and verify the local project contains the reconciled files. Report the verified branch/change and any remaining divergence in plain language.

### 7. Cloud-to-local continuation

- A cloud task must save its changes to the matching repository and update the handoff before it can claim remote save is complete.
- If the task has an approved connection to the local computer or local project, apply/fetch the saved change into the mapped local folder, preserving local work, then verify both sides.
- If the cloud environment cannot access the local project folder, do not claim local synchronization. Leave the change safely saved remotely when authorized, record a clear handoff, and state that the local project folder still needs a fetch/pull or other explicit transfer. Do not invent a working local path.
- Standalone skills installed on local computer do not automatically load into cloud tasks. For a cloud task to use this workflow, the project repository must contain this skill under `.agents/skills/project-repository-sync/SKILL.md`, or the task must have another supported distribution of the skill.

## Completion report

State: (1) which local folder and remote repository/branch were matched, (2) what was synchronized in each direction, (3) whether any exact duplicates were removed, (4) what verification ran, (5) whether both local and remote copies are current, and (6) any blocked conflicts or next step. Separate completed actions from recommendations.
