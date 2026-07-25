# Repository Agent Operating Rules

## Purpose

These instructions govern ChatGPT, Codex, and other agent-style work in `FroBoyX/chronicles-of-golarion`.

The repository is the durable source of truth. Chats and GitHub issues coordinate work, but they do not replace evidence, chronology controls, state files, dossiers, source spines, or approved narrative outputs.

## Architectural Objective

The Chronicle exists to preserve and render the campaign with high narrative fidelity while remaining fast to understand, search, and use at the table.

Agents have authority to improve the repository architecture when doing so makes the Chronicle clearer, more faithful, and more responsive.

Apply these principles:

- **Active canon over archival clutter.** Preserve useful source evidence, but do not keep stale derived documents, duplicate controls, obsolete scaffolds, or known errors in the active lookup path merely because they once existed.
- **One authority per scope.** A chronology period, current-state question, character truth, narrative day, or workflow should have one clearly controlling document.
- **Remove anti-patterns.** Fix or delete misleading structures instead of documenting them forever. Keep a superseded artifact only when it preserves unique provenance, supports reversal, or contains evidence not available elsewhere.
- **Fidelity is not maximal volume.** Preserve causality, point of view, character knowledge, uncertainty, meaningful dialogue, and emotional sequence. Remove repetition, chat-process debris, duplicate summaries, and explanations that no longer help.
- **Do not flatten.** A concise control document may link outward, but it must retain enough context to support correct decisions without forcing a full archaeological search.
- **Fast lookup matters.** Handoffs, indexes, task boards, and issues should direct an agent to the controlling file quickly. Superseded material should not appear equally authoritative.
- **Corrections propagate forward.** Raw source evidence may retain historical wording, but active chronology, state, dossiers, source spines, packets, and outputs should reflect current canon.

## Access Mode

Default to **GitHub connector operations**.

Before using command-line Git or GitHub CLI, explicitly establish all three of the following:

- a local checkout exists;
- the checkout path and current branch are known;
- direct GitHub networking and authentication work from that environment.

Do not run `git clone`, `git pull`, `git push`, or `gh` merely because connector access exists. Connector access and command-line Git access are separate capabilities.

When no local checkout is confirmed, record:

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
| Raw evidence | `evidence/raw-session-logs/`, raw chat exports, player uploads | Preserve exact source content when retained. Do not silently correct dates, spelling, or claims. Remove only confirmed duplicates or valueless noise when no unique evidence would be lost. |
| Sanitized evidence extracts | Evidence summaries and extraction files | Clarify with source references. Do not convert inference into recovered fact or dialogue. Consolidate redundant extracts once their unique evidence is safely represented. |
| GM correction / ruling | `evidence/gm-notes/`, explicit ruling sections | Preserve the ruling and scope. Propagate it into active derived documents. |
| Player memory | `evidence/player-memory/`, discovery notes | Preserve as player-confirmed internal truth or memory. Do not automatically promote to objective canon. |
| Chronology control | `chronology/`, timeline bridges and memory spines | Maintain one controlling chronology per scope. Correct dates and sequence here first. Delete or clearly supersede competing controls. |
| Current state | `state/` | Keep actor placement, knowledge, ship status, and current pressures aligned with controlling chronology. Remove obsolete tableaux from active routing. |
| Dossiers / relationships | `characters/`, `relationships/` | Merge evidence-supported facts and clearly marked internal truth. Retire temporary addenda after successful merge unless they retain unique audit value. |
| Source spines | `source-spines/` | Control sibling narrative alignment, source basis, locked facts, open checks, and output status. Close stale drafting checks once resolved. |
| Narrative outputs | `chronicles/`, `ship-logs/` | Patch-only after GM approval unless a rewrite is explicitly requested. Preserve prose fidelity while correcting material canon errors. |
| Player packets | `player-packets/` | Player-safe only. Keep branch knowledge and private actions separated. |
| Visual / conversion briefs | `visual-briefs/`, `conversions/` | Derived work. Link to controlling sources and do not rewrite historical canon. |
| Coordination | GitHub issues, task board, handoffs | Route work and record blockers. Do not duplicate canon or become a second truth store. Clean stale status promptly. |

## Retention and Cleanup

Use these rules when deciding whether to retain a file:

- Keep raw evidence that contains unique table text, timestamps, player perspective, or provenance.
- Do not keep byte-for-byte duplicates solely for sentiment or process history.
- Do not keep temporary addenda after merger unless they provide meaningful audit evidence that the main dossier cannot carry.
- Do not keep two current chronology or state controls for the same scope.
- A superseded file must state what supersedes it and must be removed from active handoffs and indexes.
- Delete obsolete process scaffolding when its function has been absorbed by a better control document.
- Git history already preserves prior versions; the working tree does not need to preserve every mistake as a live document.

## File Discovery Protocol

Never declare a repository source absent after one failed code search.

Use this sequence:

1. Fetch the exact known path when supplied.
2. Search likely filenames, title fragments, character names, dates, and spelling variants.
3. Search distinctive content phrases.
4. Read relevant indexes, handoffs, task boards, source-spine indexes, and raw-log indexes.
5. Search recent commits for additions, renames, deletions, or corrections.
6. Inspect related dossiers, chronology controls, state files, and evidence summaries.
7. Search GitHub issues when material may be in an active handoff.
8. Search uploaded-file sources only when the user refers to uploads or File Library material.
9. Request re-upload or declare absence only after the applicable strategies are exhausted.

Report search confidence:

- **High confidence absent:** known directories, filename/path variants, content variants, indexes, and recent commits were checked.
- **Medium confidence absent:** several strategies were checked, but recursive tree visibility or indexing remained incomplete.
- **Low confidence absent:** only one search strategy was available. Do not request re-upload yet.

A no-match result from code search does not prove repository absence.

## Long-File Read Safety

A full-file update requires the complete current file and current blob SHA.

When a file read is truncated:

1. Record the returned line range.
2. Continue with ranged reads until the final line.
3. Use small overlap when continuity matters.
4. Confirm headings, repeated sections, and the end of file.
5. Re-fetch the current SHA when concurrent edits are plausible.
6. Only then construct a complete replacement.

Do not replace a long file from a truncated read.

When only full-file replacement is available, make the smallest responsible content change while preserving all useful untouched text.

## Write Discipline

Separate evidence gathering from writing.

Before a substantial write:

- identify the authoritative target file;
- check for nearby duplicate or superseding files;
- state which document class is being edited;
- identify source files and provenance;
- decide whether obsolete files should be updated, superseded, consolidated, or deleted;
- inventory downstream references when changing a date, canonical term, filename, actor placement, or ruling.

Prefer section patches or unified diffs when available. Otherwise use a complete verified read and current SHA.

Do not create a new control document merely because updating the existing authority is harder. Create a new control only when the old document has a distinct archival purpose or the new scope is genuinely different.

## Impact Analysis for Corrections

Before changing a canonical date, term, filename, item name, or current-state ruling:

1. Search exact and variant spellings.
2. Classify occurrences:
   - raw quoted evidence: preserve;
   - legacy/source label: preserve only where it documents source context;
   - derived chronology/state: update;
   - dossier/relationship: update if affected;
   - source spine/narrative/player packet: review for downstream correction;
   - filename/path/reference: inventory before rename;
   - stale coordination text: update or remove.
3. Record the controlling correction in the appropriate active document.
4. Apply changes in dependency order:
   - chronology;
   - current state;
   - dossiers/relationships;
   - source spines;
   - player packets and narrative outputs, where needed;
   - routing and task controls.
5. Report preserved source occurrences separately from corrected derived occurrences.

## Commit Discipline

Batch related changes into coherent commits when the available tool path permits safe review.

Preferred behavior:

- one issue or work unit per coherent scope;
- preview intended changed paths before writing;
- use lower-level blob/tree/commit operations for transactional multi-file changes only when the base tree and proposed tree are fully known;
- otherwise use small ordered commits and group them under one issue progress comment;
- never hide corrective commits or accidental duplication;
- remove or explicitly close duplicate active artifacts;
- use commit messages that describe the project effect, not the chat process.

## Issue-Backed Agent Handoffs

Use a GitHub issue when:

- work spans more than one chat or agent;
- work is expected to touch several related files;
- unresolved blockers may require GM/product-owner input;
- another chat must continue after the current chat ends;
- chronology, state, dossiers, and narrative outputs must be coordinated;
- a correction has broad downstream impact.

Do not create issues for routine one-file edits, ordinary narrative-day production, or status chatter.

Issues coordinate work. They do not contain canonical facts unless those facts are also written to the appropriate repository document.

### Claim

```md
## CLAIMED

- Agent/chat role:
- Current task:
- Files expected to change:
- Immediate blockers:
```

### Progress

```md
## PROGRESS

- Completed:
- Commits:
- New findings:
- Remaining blockers:
- Next action:
```

### Blocked

```md
## BLOCKED

- Decision/evidence needed:
- Why repository evidence is insufficient:
- Files/sources already checked:
- Safe default if no ruling is made:
```

Routine uncertainty may remain explicitly unresolved and does not require escalation.

### Completion

```md
## HANDOFF COMPLETE

- Controlling output:
- Created paths:
- Updated paths:
- Deleted or superseded paths:
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
- deleted or superseded paths;
- commits;
- controlling documents used;
- raw evidence preserved;
- corrected derived references;
- unresolved questions;
- next owner or recommended task.
