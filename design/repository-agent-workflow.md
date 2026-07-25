# Repository Agent Workflow

## Document Status

- Type: Project operations / repository workflow
- Maturity: Working control document
- Scope: Connector-backed repository discovery, safe reads, writes, impact analysis, commits, and agent-to-agent issue handoffs
- Parent issue: GitHub issue #1
- Authority: `AGENTS.md` is the concise root operating instruction; this file provides the expanded procedure

## Purpose

Chronicles of Golarion is a prose-heavy, evidence-driven archive. Its repository includes raw sources, derived chronology, current state, character truth, narrative source spines, and approved outputs. Ordinary code-oriented repository habits are not sufficient because a convenient edit can silently damage provenance or create competing control documents.

This workflow reduces those risks while acknowledging current connector limitations.

## Capability Matrix

| Need | Current connector support | Current project handling |
|---|---|---|
| Known-path file read | Supported | Use `fetch_file`; use ranges for long files. |
| Content search | Supported but index-dependent | Combine filename/title/phrase variants, indexes, and commit search. |
| Recursive tree browsing | Not reliably exposed as one action | Use known indexes, path search, repository conventions, and recent commits; report confidence limits. |
| Long-file pagination | Ranged reads supported; automatic pagination not guaranteed | Continue explicit ranges until end of file. |
| Section patch / unified diff | Not exposed as a standard file-write action | Full replacement only after complete verified read and current SHA. |
| File creation/update/delete | Supported | Respect document classes and authority. |
| Multi-file transactional commit | Lower-level blob/tree/commit/ref operations exist, but no simple reviewed transaction helper | Use only when base tree and proposed changes are fully known; otherwise group sequential commits in one issue work unit. |
| Issue creation/comments | Supported | Use for durable ownership, blockers, progress, and handoff. |
| Local checkout / Git networking | Not implied by connector access | Treat as unavailable until explicitly established. |
| Reference/rename impact analysis | No single exhaustive action | Search exact term, variants, filenames, recent commits, indexes, and classify occurrences. |
| Duplicate-document detection | No automatic warning | Search adjacent titles/paths and identify controlling/superseded files before creation. |

## Work Classification

Before starting, classify the task.

### Direct repository task

Use normal connector work when the task is narrow, can be completed in one chat, and has no significant unresolved cross-file impact.

Examples:

- correcting one known dossier fact from a GM ruling;
- adding one evidence summary;
- aligning one approved source spine's status metadata.

### Issue-backed agent task

Create or use an issue when:

- multiple agents/chats participate;
- the work has several phases;
- more than a few related files may change;
- date/canon corrections have downstream impact;
- evidence gaps may need a GM ruling;
- completion must be handed to a different specialist.

### Raw evidence intake

Raw intake remains a specialized workflow. Preserve uploads or logs before interpretation. Do not combine raw preservation, chronology correction, and final narrative writing in one uncontrolled pass.

## Repository Discovery Procedure

### Phase 1: Resolve context

Record:

- repository;
- issue, if any;
- expected document class;
- known path or subject;
- current access mode.

### Phase 2: Search by several strategies

Use the applicable strategies:

1. Exact path fetch.
2. Filename and title fragments.
3. Character, NPC, ship, event, and date variants.
4. Distinctive quoted phrases.
5. Relevant index files.
6. Handoffs and task boards.
7. Recent commits.
8. Related dossiers, chronology, and current-state files.
9. GitHub issue history.
10. Uploaded-file search when the user refers to uploads.

Do not interpret no code-search result as a conclusive absence finding.

### Phase 3: Report confidence

When a source remains unfound, state which strategies were checked and whether repository-tree visibility or indexing may be incomplete.

## Complete Long-File Read Procedure

For files likely to exceed the connector response limit:

1. Fetch the opening range.
2. Note returned lines and SHA.
3. Fetch subsequent ranges with a small overlap.
4. Continue until the final line is reached.
5. Confirm there are no skipped sections or duplicate range joins.
6. Build the proposed change from the assembled complete content.
7. Re-fetch the relevant changed section or current SHA immediately before writing when concurrent edits are plausible.
8. Abort and rebase the edit if the SHA changed.

A partial read may support analysis, but not complete-file replacement.

## Provenance and Document Authority

Every derived control document should identify its sources and status.

Recommended metadata:

```md
## Document Status

- Type:
- Maturity:
- Scope:
- Source basis:
- Player-facing status:
- Canon status:
- Controlling / supporting / superseded relationship:
- Parent issue, when applicable:
```

When two chronology or state files cover the same scope:

1. identify the controlling document;
2. mark the older one supporting, archived, or superseded;
3. update incoming handoffs to reference the controlling file;
4. do not leave both appearing equally authoritative.

## Correction and Impact Inventory

A correction pass begins with an inventory, not immediate replacement.

For each occurrence, classify:

| Occurrence type | Action |
|---|---|
| Raw evidence quote or legacy log label | Preserve unchanged. Add interpretation elsewhere if needed. |
| Sanitized summary repeating an old label | Preserve source label, clarify current handling. |
| Active chronology/control statement | Correct. |
| Current-state placement | Correct after chronology. |
| Character or NPC dossier | Correct if the character fact or placement changes. |
| Source spine | Review date, sources, scene order, and output alignment. |
| Narrative output | Patch only when the correction materially changes approved prose or metadata. |
| Player packet | Correct player-safe facts and knowledge boundaries. |
| Filename/reference | Inventory all inbound references before rename. |
| Issue/chat prompt | Comment with correction; do not treat stale prompt text as repository authority. |

The impact report must distinguish preserved source occurrences from corrected derived occurrences.

## Write and Commit Procedure

### Pre-write preview

Before substantial changes, report or issue-comment:

- files planned for creation;
- files planned for update;
- authority and provenance;
- raw files intentionally untouched;
- expected commit grouping.

### Commit grouping

Prefer one coherent work unit.

When safe lower-level transaction operations are practical:

1. resolve the parent commit and base tree;
2. create all necessary blobs;
3. create a proposed tree;
4. review paths and content SHAs;
5. create one commit;
6. update the branch ref without force.

When the connector workflow cannot safely preview a transaction:

- make small, ordered commits;
- use clear conventional messages;
- group them under one issue progress comment;
- avoid mixing unrelated evidence, chronology, and narrative changes.

### Post-write verification

- fetch the changed file or inspect the commit;
- confirm no content was truncated;
- confirm raw evidence was not modified;
- confirm cross-references still resolve;
- update the issue with commits and remaining blockers.

## Issue-Backed Handoff Lifecycle

### Open

Issue body defines:

- objective;
- agent role;
- final approver;
- required sources;
- outputs;
- non-goals;
- safety boundaries;
- acceptance criteria.

### Claim

The working agent posts `## CLAIMED` before substantial writing.

### Progress

Use `## PROGRESS` after meaningful work units. Do not comment for every small read or commit.

### Blocked

Use `## BLOCKED` only after repository evidence and reasonable inference are exhausted. State a safe default or explicitly unresolved path.

### Handoff complete

The final comment must identify controlling outputs, commits, decisions, preserved sources, unresolved items, and next owner.

### Close

Only the Chronicle Master, GM, or designated final approver closes the issue. Close duplicates with the duplicate reason and link to the controlling issue.

## Current Pilot

GitHub issue #2 is the first Chronicle issue-backed agent handoff:

- Bonewrack Island Memory Reconstruction.

The pilot should test:

- whether issue context survives across chats;
- whether agents post useful progress rather than duplicating work;
- whether blockers reach the GM only when necessary;
- whether commit groupings and controlling documents are easier to identify;
- whether the final handoff can be reviewed without replaying the full chat history.

## Platform Improvement Backlog

GitHub issue #1 retains requests that require connector/platform changes rather than repository documentation.

The project can mitigate these gaps, but cannot itself implement:

- reliable recursive tree listing;
- automatic long-read pagination;
- first-class section patching;
- reviewed multi-file transactions;
- automatic reference/rename impact analysis;
- automatic duplicate-authority warnings;
- explicit local/network capability reporting from the connector.

## Review Cadence

Review this workflow after:

- the Bonewrack issue handoff completes;
- a second cross-agent issue completes;
- any incident involving duplicate files, truncated replacement, raw-evidence modification, or accidental chronology propagation.

Update `AGENTS.md` only when the default rules change. Use this document for expanded examples and procedural refinements.
