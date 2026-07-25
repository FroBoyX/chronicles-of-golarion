# Repository Agent Operating Rules

## Purpose

These instructions govern ChatGPT, Codex, and other agent-style work in `FroBoyX/chronicles-of-golarion`.

The repository is the durable source of truth. Chats and GitHub issues coordinate work, but they do not replace evidence, chronology controls, state files, dossiers, source spines, or approved narrative outputs.

## Access Mode

Default to **GitHub connector operations**.

Before using command-line Git or GitHub CLI, explicitly establish all three of the following:

- a local checkout exists;
- the checkout path and current branch are known;
- direct GitHub networking and authentication work from that environment.

Do not run `git clone`, `git pull`, `git push`, or `gh` merely because connector access exists. Connector access and command-line Git access are separate capabilities.

When no local checkout is confirmed, state or record:

```text
Access mode: GitHub connector only.
Local checkout: not established.
Direct Git network access: not established.
```

## Authority and Evidence Order

Use the evidence hierarchy in `handoffs/chronicle-master-handoff.md` and `CANON.md`.

The general authority order is:

1. Current GM truth / direct product-owner correction.
2. Preserved primary campaign evidence.
3. Extracted evidence summaries.
4. Player memory, clearly labeled.
5. GM memory, clearly labeled.
6. Adventure Path scaffold.
7. Convenience or inference.

Do not let AP material overwrite table-specific evidence or GM truth.

## Document Classes and Mutation Rules

| Class | Typical paths | Mutation rule |
|---|---|---|
| Raw evidence | `evidence/raw-session-logs/`, raw chat exports, player uploads | Preserve exactly. Do not silently correct dates, spelling, or factual claims. Add separate summaries or correction notes. |
| Sanitized evidence extracts | evidence summaries and extraction files | May be clarified with source citations, but do not convert inference into recovered fact or dialogue. |
| GM correction / ruling | `evidence/gm-notes/`, explicit ruling sections | Preserve the ruling and its scope. Do not broaden it beyond what was decided. |
| Player memory | `evidence/player-memory/`, discovery notes | Preserve as player-confirmed internal truth or memory. Do not automatically promote to objective canon. |
| Chronology control | `chronology/`, timeline bridges and memory spines | Correct derived dates and sequence here. Identify controlling and superseded files. |
| Current state | `state/` | Keep actor placement, knowledge, ship status, and current pressures aligned with controlling chronology. |
| Dossiers / relationships | `characters/`, `relationships/` | Merge only evidence-supported facts and clearly marked internal/player truth. Preserve knowledge boundaries. |
| Source spines | `source-spines/` | Control sibling narrative alignment, source basis, locked facts, open checks, and output status. |
| Narrative outputs | `chronicles/`, `ship-logs/` | Patch-only after GM approval unless a rewrite is explicitly requested. |
| Player packets | `player-packets/` | Player-safe only. Do not cross-contaminate private branch knowledge. |
| Visual / conversion briefs | `visual-briefs/`, `conversions/` | Derived work. Link back to source files and do not rewrite historical canon. |

## File Discovery Protocol

Never declare a repository source absent after one failed code search.

Use this sequence:

1. Fetch the exact known path when one is supplied.
2. Search likely filenames, title fragments, character names, dates, and spelling variants.
3. Search distinctive content phrases.
4. Read relevant indexes, handoffs, task boards, source-spine indexes, and raw-log indexes.
5. Search recent commits for additions, renames, or corrections.
6. Inspect related dossiers, chronology controls, state files, and evidence summaries.
7. Search GitHub issues when the material may be in an active handoff.
8. Search uploaded-file sources only when the user refers to uploads or File Library material.
9. Request re-upload or declare absence only after the applicable strategies are exhausted.

Report search confidence:

- **High confidence absent:** known directories, filename/path variants, content variants, indexes, and recent commits were checked.
- **Medium confidence absent:** multiple repository searches were completed, but recursive tree visibility or indexing remained incomplete.
- **Low confidence absent:** only one search strategy was available. Do not request re-upload yet.

A no-match result from code search does not prove repository absence.

## Long-File Read Safety

A full-file update requires the complete current file and its current blob SHA.

When a file read is truncated:

1. Record the returned line range.
2. Continue with ranged reads until the final line is reached.
3. Use small overlap between ranges when continuity matters.
4. Confirm headings, repeated sections, and the end of file.
5. Only then construct a complete replacement.

Do not replace a long file from a truncated read.

When only full-file replacement is available, make the smallest possible content change while preserving all untouched text.

## Write Discipline

Separate evidence gathering from writing.

Before a substantial write:

- identify the authoritative target file;
- check for nearby duplicate or superseding files;
- state which document class is being edited;
- identify source files and provenance;
- inventory downstream references when changing a date, canonical term, filename, actor placement, or authoritative ruling.

Prefer section patches or unified diffs when the available tool supports them. When it does not, use a complete verified read and current SHA.

Do not create a new control document merely because updating the existing authority is harder. Create a new control document only when the old document has a distinct archival purpose or is explicitly marked superseded.

## Impact Analysis for Corrections

Before changing a canonical date, term, filename, item name, or current-state ruling:

1. Search exact and variant spellings.
2. Classify every occurrence:
   - raw quoted evidence: preserve;
   - legacy/source label: preserve with explanation;
   - derived chronology/state: update;
   - dossier/relationship: update if affected;
   - source spine/narrative/player packet: review for downstream correction;
   - filename/path/reference: inventory before rename.
3. Record the controlling correction.
4. Apply changes in dependency order:
   - chronology;
   - current state;
   - dossiers/relationships;
   - source spines;
   - player packets and narrative outputs, only where needed.
5. Report preserved raw occurrences separately from corrected derived occurrences.

## Commit Discipline

Batch related changes into coherent commits when the available tool path permits safe review.

Preferred behavior:

- one issue or work unit per coherent scope;
- preview intended changed paths before writing;
- use lower-level blob/tree/commit operations for transactional multi-file changes only when the base commit/tree is fully known and the proposed tree can be reviewed safely;
- otherwise use small sequential commits with clear messages and a final issue comment grouping them as one work unit;
- never hide corrective commits or accidental duplication;
- close duplicate issues/files explicitly and point to the controlling item.

Commit messages should describe the project effect, not the chat process.

## Issue-Backed Agent Handoffs

Use a GitHub issue when any of the following apply:

- work spans more than one chat or agent;
- work is expected to touch several related files;
- unresolved blockers may require GM/product-owner input;
- another chat must continue after the current chat ends;
- chronology, state, dossiers, and narrative outputs must be coordinated;
- a correction has broad downstream impact.

Issues coordinate work. They do not contain canonical facts unless those facts are also written to the appropriate repository document.

### Claim

The agent taking ownership posts:

```md
## CLAIMED

- Agent/chat role:
- Current task:
- Files expected to change:
- Immediate blockers:
```

### Progress

After a meaningful work unit:

```md
## PROGRESS

- Completed:
- Commits:
- New findings:
- Remaining blockers:
- Next action:
```

### Blocked

Use product-owner intervention only when needed:

```md
## BLOCKED

- Decision/evidence needed:
- Why repository evidence is insufficient:
- Files/sources already checked:
- Safe default if no ruling is made:
```

Routine uncertainty may remain labeled unresolved and does not require escalation.

### Completion

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

Chronicle Master or the designated final approver closes the issue.

## Player-Safety Rule

Before any player-facing output, explicitly evaluate character knowledge and spoiler scope.

Do not reveal:

- other PCs' hidden actions;
- split-branch knowledge not communicated in play;
- GM-only evidence;
- private player memory from another character;
- unresolved culpability presented as fact;
- coercive material beyond the approved player-safe framing.

## End-of-Task Report

Every repository task should report:

- access mode;
- issue number, when applicable;
- created paths;
- updated paths;
- commits;
- controlling documents used;
- raw evidence preserved;
- corrected derived references;
- unresolved questions;
- next owner or recommended task.
