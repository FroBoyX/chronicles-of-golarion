# Repository Agent Workflow

## Document Status

- Type: Project operations / repository workflow
- Maturity: Working control document
- Scope: Connector-backed discovery, safe reads and writes, impact analysis, cleanup, commits, and issue-backed handoffs
- Parent issue: GitHub issue #1
- Authority: `AGENTS.md` is the concise root instruction; this file provides the expanded procedure

## Purpose

Chronicles of Golarion is a prose-heavy, evidence-driven archive and an active campaign tool. It must preserve enough source truth to support narrative fidelity while keeping the working repository clear, responsive, and usable.

The goal is not maximal retention. The goal is a coherent active canon architecture backed by sufficient provenance.

## Active Architecture and Cleanup

### Active canon layer

The active layer contains the files agents should use for present decisions:

- controlling chronology;
- current-state tableaux;
- current PC/NPC dossiers and relationships;
- current source spines;
- approved narrative outputs;
- player-safe packets;
- current handoffs and indexes.

Only one document should control a given scope.

### Evidence layer

The evidence layer supports reconstruction and challenge:

- raw logs;
- player-authored records;
- GM corrections;
- player memory;
- sanitized extracts.

Evidence may retain legacy dates, misspellings, conflicting claims, or incomplete perspective because those features belong to the source. Active derived files should not repeat those errors as current truth.

### Cleanup rule

Do not preserve noise or failed architecture merely because Git history once contained it.

For derived files:

1. update the controlling document;
2. redirect incoming references;
3. merge unique useful content;
4. delete the obsolete file, or mark it superseded only when it retains unique provenance or reversal value;
5. remove superseded material from active routing and lookup indexes.

Temporary addenda, duplicate bridges, correction scaffolds, and stale task entries should not accumulate indefinitely.

### Fidelity rule

Cleanup must not flatten the campaign.

Preserve:

- causality and sequence;
- character knowledge and mistaken belief;
- meaningful uncertainty;
- recovered direct language;
- emotional and relationship development;
- the difference between table outcome, source perspective, and later interpretation.

Remove:

- repeated summaries that add no new value;
- stale process commentary;
- duplicate status records;
- known wrong derived dates or names;
- abandoned control structures;
- obsolete open checks;
- explanations that only describe how earlier agents made a mistake.

## Capability Matrix

| Need | Current connector support | Current project handling |
|---|---|---|
| Known-path file read | Supported | Use `fetch_file`; use ranges for long files. |
| Content search | Supported but index-dependent | Combine filename/title/phrase variants, indexes, issues, and commit search. |
| Recursive tree browsing | Not reliably exposed as one action | Use conventions, indexes, path searches, and recent commits; report confidence limits. |
| Long-file pagination | Ranged reads supported; automatic pagination not guaranteed | Continue explicit ranges until end of file. |
| Section patch / unified diff | Not exposed as a standard file-write action | Full replacement only after complete verified read and current SHA. |
| File creation/update/delete | Supported | Respect document classes, authority, and cleanup rules. |
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
- aligning one approved source spine's status metadata;
- deleting one obsolete scaffold after its content has been merged.

### Issue-backed agent task

Create or use an issue when:

- multiple agents/chats participate;
- the work has several phases;
- several related files may change;
- date/canon corrections have downstream impact;
- evidence gaps may need a GM ruling;
- completion must be handed to a different specialist.

Do not create issues for routine narrative production or one-file maintenance.

### Raw evidence intake

Raw intake remains specialized. Preserve useful source material before interpretation. Do not combine raw preservation, chronology correction, and final narrative writing in one uncontrolled pass.

Confirmed exact duplicates with no unique metadata, private lines, timestamps, or provenance value do not need permanent retention.

## Repository Discovery Procedure

### Phase 1: Resolve context

Record:

- repository;
- issue, if any;
- expected document class;
- known path or subject;
- likely controlling document;
- current access mode.

### Phase 2: Search by several strategies

Use applicable strategies:

1. Exact path fetch.
2. Filename and title fragments.
3. Character, NPC, ship, event, and date variants.
4. Distinctive quoted phrases.
5. Relevant index files.
6. Handoffs and task boards.
7. GitHub issues.
8. Recent commits, including deletions and corrections.
9. Related dossiers, chronology, current-state files, and source spines.
10. Uploaded-file search when the user refers to uploads.

Do not interpret no code-search result as conclusive absence.

### Phase 3: Resolve authority

Finding a file is not enough. Determine whether it is:

- controlling;
- supporting evidence;
- player-facing derivative;
- superseded;
- obsolete noise.

Do not build new work from a stale file merely because it was easier to find.

### Phase 4: Report confidence

When a source remains unfound, state which strategies were checked and whether repository-tree visibility or indexing may be incomplete.

## Complete Long-File Read Procedure

For files likely to exceed the connector response limit:

1. Fetch the opening range.
2. Note returned lines and SHA.
3. Fetch subsequent ranges with a small overlap.
4. Continue until the final line.
5. Confirm there are no skipped sections or duplicate joins.
6. Build the proposed change from complete content.
7. Re-fetch the changed section or current SHA immediately before writing when concurrent edits are plausible.
8. Abort and rebase if the SHA changed.

A partial read may support analysis, but not complete-file replacement.

## Provenance and Document Authority

Every derived control document should identify sources and status without becoming a metadata wall.

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

1. decide which is controlling;
2. merge unique useful material;
3. update incoming handoffs and indexes;
4. delete the obsolete duplicate when safe;
5. retain a superseded file only if it has unique audit or provenance value;
6. never leave both appearing equally authoritative.

Git history is sufficient preservation for ordinary replaced drafts and mistakes.

## Correction and Impact Inventory

A correction pass begins with an inventory, not immediate replacement.

| Occurrence type | Action |
|---|---|
| Raw evidence quote or legacy log label | Preserve unchanged when source retention is justified. Add current interpretation elsewhere. |
| Sanitized summary repeating an old label | Preserve the source label only where useful; clarify current handling. |
| Active chronology/control statement | Correct. |
| Current-state placement | Correct after chronology. |
| Character or NPC dossier | Correct if character fact or placement changes. |
| Source spine | Review date, sources, scene order, open checks, and output alignment. |
| Narrative output | Patch only when correction materially changes approved prose or metadata. |
| Player packet | Correct player-safe facts and knowledge boundaries. |
| Filename/reference | Inventory inbound references before rename or deletion. |
| Issue/chat prompt | Comment with correction when still active; stale chat text is not authority. |
| Obsolete derived scaffold | Merge unique value, then delete or explicitly supersede. |

The impact report must distinguish preserved source occurrences from corrected derived occurrences.

## Write and Commit Procedure

### Pre-write preview

Before substantial changes, report or issue-comment:

- controlling files planned for update;
- new files, if genuinely needed;
- files planned for deletion or supersession;
- authority and provenance;
- raw files intentionally untouched;
- expected commit grouping.

### Commit grouping

Prefer one coherent work unit.

When safe lower-level transaction operations are practical:

1. resolve the parent commit and base tree;
2. create all required blobs;
3. create a proposed tree;
4. review paths and content SHAs;
5. create one commit;
6. update the branch ref without force.

When the connector workflow cannot safely preview a transaction:

- make small ordered commits;
- use clear messages;
- group them under one issue progress comment;
- avoid mixing unrelated evidence, chronology, narrative, and architecture changes.

### Post-write verification

- fetch changed files or inspect commits;
- confirm content was not truncated;
- confirm raw evidence was not altered accidentally;
- confirm cross-references resolve;
- confirm obsolete controls no longer appear in active routing;
- update the issue with commits and blockers.

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

Use `## PROGRESS` after meaningful work units. Do not comment for every read or tiny commit.

### Blocked

Use `## BLOCKED` only after repository evidence and reasonable inference are exhausted. State a safe default or explicitly unresolved path.

### Handoff complete

The final comment identifies controlling outputs, created/updated/deleted paths, commits, decisions, preserved sources, unresolved items, and next owner.

### Close

Only Chronicle Master, GM, or designated final approver closes the issue. Close duplicates with the duplicate reason and point to the controlling issue.

Issues should be closed promptly after acceptance. Do not let completed coordination threads become a shadow task board.

## Current Pilot

GitHub issue #2 is the first Chronicle issue-backed agent handoff:

- Bonewrack Island Memory Reconstruction and Arodus 4 correction audit.

The pilot tests:

- whether issue context survives across chats;
- whether agents continue current repository state rather than restarting;
- whether blockers reach the GM only when necessary;
- whether commit groups and controlling documents are easier to identify;
- whether obsolete derived controls are cleaned rather than merely annotated;
- whether final handoff review avoids replaying the full chat history.

## Platform Improvement Backlog

GitHub issue #1 retains requests that require connector/platform changes rather than repository documentation.

The project can mitigate but cannot itself implement:

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
- any incident involving duplicate files, truncated replacement, raw-evidence modification, accidental chronology propagation, or retained obsolete controls.

Update `AGENTS.md` only when default rules change. Use this document for expanded procedures and refinements.
