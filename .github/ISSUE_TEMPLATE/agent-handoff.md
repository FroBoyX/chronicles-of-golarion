---
name: Agent handoff
description: Durable coordination for work spanning agents, chats, files, or unresolved GM decisions
title: "[Agent Handoff] "
labels: []
assignees: []
---

## Status

Active / Blocked / Review / Complete

## Agent role

<!-- Name the specialist role or chat that should own the work. -->

## Product owner

FroBoyX. Escalate only genuine canon, staging, permission, or missing-private-evidence decisions.

## Final approver

Chronicle Master / GM canon authority, unless another approver is named here.

## Objective

<!-- Describe the durable outcome, not just the next chat message. -->

## Repository authority

The repository remains the source of truth. This issue coordinates ownership, scope, blockers, progress, commit references, and handoff status. Canonical facts must be written to the correct repository documents.

## Required sources

- `path`

## Expected outputs

- `path`

## Scope

- 

## Non-goals

- 

## Evidence / spoiler boundaries

- Preserve raw evidence exactly.
- Do not expose player-private or split-branch knowledge outside its permitted scope.
- Do not promote player or GM memory to objective canon without the required review.

## Access and repository rules

- Use GitHub connector operations by default.
- Do not use command-line Git until local checkout, branch, network, and authentication are explicitly established.
- Search paths, filenames, content variants, indexes, handoffs, issues, and recent commits before declaring a source absent.
- Read long files completely before full-file replacement.
- Update authoritative controls instead of creating unnecessary duplicates.
- Inventory downstream references before canon/date/name/file corrections.
- Record commits and blockers in issue comments.
- Follow `AGENTS.md` and `design/repository-agent-workflow.md`.

## Acceptance criteria

- [ ] 

## Claim protocol

The working agent should comment:

```md
## CLAIMED

- Agent/chat role:
- Current task:
- Files expected to change:
- Immediate blockers:
```

## Progress protocol

```md
## PROGRESS

- Completed:
- Commits:
- New findings:
- Remaining blockers:
- Next action:
```

## Blocker protocol

```md
## BLOCKED

- Decision/evidence needed:
- Why repository evidence is insufficient:
- Files/sources already checked:
- Safe default if no ruling is made:
```

## Completion protocol

```md
## HANDOFF COMPLETE

- Controlling output:
- Created paths:
- Updated paths:
- Commits:
- Canon/date decisions applied:
- Raw evidence preserved:
- Remaining unresolved questions:
- Recommended next owner/task:
```
