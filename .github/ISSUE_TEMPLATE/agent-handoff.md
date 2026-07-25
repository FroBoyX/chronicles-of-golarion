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

Identify one controlling output per scope. Merge useful content from obsolete derived files, then delete or clearly supersede them rather than preserving duplicate active controls.

## Required sources

- `path`

## Controlling documents

- `path`

## Expected outputs

- Updated controlling path:
- New path only if genuinely required:
- Obsolete path expected to be deleted or superseded:

## Scope

- 

## Non-goals

- 

## Evidence / spoiler boundaries

- Preserve retained raw evidence exactly.
- Do not keep confirmed duplicate or valueless source noise when no unique text, metadata, or provenance would be lost.
- Do not expose player-private or split-branch knowledge outside its permitted scope.
- Do not promote player or GM memory to objective canon without the required review.

## Access and repository rules

- Use GitHub connector operations by default.
- Do not use command-line Git until local checkout, branch, network, and authentication are explicitly established.
- Search paths, filenames, content variants, indexes, handoffs, issues, and recent commits before declaring a source absent.
- Read long files completely before full-file replacement.
- Update authoritative controls instead of creating unnecessary duplicates.
- Inventory downstream references before canon/date/name/file corrections.
- Remove stale derived controls from active routing after their useful content is merged.
- Record commits and blockers in issue comments.
- Follow `AGENTS.md` and `design/repository-agent-workflow.md`.

## Acceptance criteria

- [ ] One controlling output is identified for each affected scope.
- [ ] Useful source evidence and narrative nuance are preserved.
- [ ] Known errors and stale derived references are corrected.
- [ ] Duplicate or obsolete controls are deleted or explicitly superseded.
- [ ] Active handoffs and indexes point only to current authorities.

## Claim protocol

The working agent should comment:

```md
## CLAIMED

- Agent/chat role:
- Current task:
- Controlling files:
- Files expected to change:
- Files expected to be deleted or superseded:
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
- Deleted or superseded paths:
- Commits:
- Canon/date decisions applied:
- Raw evidence preserved:
- Noise or obsolete scaffolding removed:
- Remaining unresolved questions:
- Recommended next owner/task:
```
