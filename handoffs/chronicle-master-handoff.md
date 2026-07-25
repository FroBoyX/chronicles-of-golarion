# Chronicle Master Handoff

## Document Status

- Type: Master routing / canon-control handoff
- Maturity: Active control document
- Scope: Project architecture, authority, priorities, specialist routing, and final approval
- Owner: GM / canon authority
- Assistant role: Chronicle Master, continuity lead, and repository architect

## Mission

Maintain a faithful and usable Chronicle of the campaign.

The goal is not to preserve every past reconstruction artifact. Preserve useful source evidence, maintain one active authority per scope, remove obsolete derived noise, and keep the repository fast to understand and use.

Read before substantial work:

- `AGENTS.md`
- `CANON.md`
- `design/repository-agent-workflow.md`
- `tracking/current-task-board.md`
- `tracking/chat-map.md`
- `tracking/open-questions.md`
- the active GitHub issue that owns the work, when applicable

## Campaign Anchors

- Campaign: Pathfinder, **Skull & Shackles**, archived as **Chronicles of Golarion**.
- Purpose: reconstruct, preserve, narrate, and relaunch the original campaign from surviving table evidence and memory.
- Press-ganging: **Erastus 4, 4712 AR**.
- Waking aboard the Wormwood: **Erastus 5, 4712 AR**.
- Current chronology correction: the final preserved Bonewrack session / cold-open endpoint is **Arodus 4, 4712 AR**. Older active derived references to Arodus 5 are cleanup targets under GitHub issue #2. Raw source labels remain unchanged where they document original evidence.

## Authority Order

When sources conflict:

1. Current GM truth / direct product-owner correction.
2. Preserved primary campaign evidence.
3. Sanitized evidence extracts.
4. Player memory, clearly labeled.
5. GM memory, clearly labeled.
6. Published Adventure Path scaffold.
7. Convenience or inference.

The Adventure Path supplies structure and setting context. It cannot overwrite table-specific evidence or GM rulings.

## Active Canon Architecture

- The repository is the source of truth.
- GitHub issues coordinate ownership, blockers, commits, and handoff; they are not canon storage.
- Each chronology period, current-state question, dossier, source spine, and workflow should have one controlling document.
- Merge useful content from temporary addenda and correction scaffolds, then delete or explicitly supersede them when they no longer help.
- Keep raw evidence when it carries unique text, perspective, timestamps, or provenance.
- Correct derived chronology and state instead of preserving known errors in active documents.
- Preserve narrative nuance: causality, character knowledge, uncertainty, exact recovered language, relationship development, and table outcome.
- Remove duplicate summaries, stale process notes, obsolete checks, and architecture that makes lookup harder.

## Standard Evidence Flow

```text
Source evidence
  -> conservative extraction
  -> controlling chronology / state / dossier integration
  -> source spine
  -> sibling narrative outputs or player-safe packet
  -> resolved checks removed; genuine uncertainty retained
```

For new source material:

1. Preserve useful raw evidence in the correct evidence path.
2. Extract facts conservatively.
3. Update the controlling derived document instead of creating a parallel control.
4. Record unresolved questions only when they affect future decisions.
5. Report paths, commits, preserved sources, corrected derived references, and remaining blockers.

## Issue-Backed Orchestration

Use issues for long-running, cross-agent, or cross-file work.

Active project issues:

- **#1 — Safer repository workflow:** repository safeguards are implemented; close after the handoff pilot is reviewed.
- **#2 — Bonewrack Island Memory Reconstruction:** controls the Arodus 1–4 memory pass, Arodus 4 correction audit, and island handoff completion.

Working agents claim their issue, post meaningful progress, and finish with a handoff comment. Chronicle Master reviews and closes.

Routine one-file changes and ordinary narrative-day production do not need issues.

## Specialist Pass-Offs

### Narrative Output / Reconstruction

Control document: `design/narrative-output-method.md`.

For an evidence-stable day or event, produce sibling outputs from one source spine:

1. **Ship's Log** — terse officer-side record.
2. **Narrative Write-Up** — readable paraphrased chronicle prose.
3. **Narrative Chat Scene** — immersive reconstruction with recovered direct quotes.

Rules:

- siblings derive from the source spine, not from one another;
- recovered quotes receive typo-level cleanup only;
- dialogue embellishment is opt-in and remains candidate text until approved;
- approved prose is patch-only unless the GM requests a rewrite;
- after approval, perform an administrative source-spine close pass: lock date/title/status, record sibling paths, resolve stale checks, and identify the Discord formatter source without rewriting prose.

Narrative Output remains active for evidence-stable days even while current cold-open staging remains unresolved.

### PC Discovery / Player Packets

Control document: `handoffs/pc-dossiers-player-packets-handoff.md` plus PC-specific discovery handoffs.

- Preserve player answers as player memory/internal truth before canon integration.
- Keep player-facing discovery chats free of GM-only branch knowledge.
- Use dedicated character chats for targeted memory questions.
- Generate cold-open packets only from the character's actual knowledge.

Mirei's direct player workflow is controlled by `handoffs/mirei-character-discovery-handoff.md` and `questions/mirei-active-narrative-beats.md`.

### Man's Promise / Bonewrack

Control handoff: `handoffs/mans-promise-bonewrack-handoff.md`.

Current island memory reconstruction is issue-backed under #2. Do not restart it from an older prompt or use stale Arodus 5 controls as authority.

Current cold-open staging remains a separate practical task: exact positions, guard state, survivor alignment, ship movement, and seaworthiness.

### NPC & Crew State Audit

Control handoff: `handoffs/npc-crew-state-handoff.md`.

Use for exact actor placement, survival and capability, survivor loyalties, command authority, and crew viability. Do not invent convenient loyalties or positions when evidence ends. Return genuine staging decisions to Chronicle Master.

### Visual Output / Art Direction

Control documents:

- `design/visual-output-method.md`
- `design/visual-style-guide.md`
- `handoffs/visual-output-handoff.md`
- `tracking/image-output-index.md`

Create a visual brief before major generation. Generated images become visual canon only after GM approval. Battle maps are truth-first.

### PF1 to PF2e Conversion

Control documents:

- `design/pf2e-conversion-method.md`
- `handoffs/pf2e-conversion-handoff.md`
- `tracking/pf2e-conversion-index.md`

PF2e is a possible relaunch-mechanics layer, not a rewrite of PF1 history. Rebuild by concept and table identity. PC conversions require player and GM review.

## Current Priority Order

1. Complete issue #2: finish the Bonewrack memory spine, Arodus 4 impact cleanup, targeted memory routing, and controlling/superseded chronology decision.
2. Finish cold-open staging: exact confinement and guard state, command placement, survivor positions and stances, Coconut Beach timing, and Man's Promise seaworthiness.
3. Prepare player-safe cold-open packets once each branch's current facts are stable.
4. Continue Narrative Output for evidence-stable earlier days; close source spines administratively after approval.
5. Continue targeted character discovery without reopening settled chronology.
6. Pilot PF2e conversion only as a separate mechanics audit, not as a blocker for reconstruction.

## Knowledge and Player-Safety Rules

- Do not cross-contaminate split-branch knowledge before communication or reunion.
- Keep private actions and testimony scoped to what each character knows.
- Player knowledge is not automatically character knowledge.
- Sensitive relationship material must remain careful, evidence-bound, and player-led in player-facing work.

## Language and Narrative Rules

- Do not describe early Wormwood as a normal adventuring party. Use **new hands**, **press-ganged crew**, **crew**, or names.
- Preserve uncertainty where it matters; remove uncertainty that has been resolved.
- Preserve raw source spelling only in evidence files. Active prose and controls should be clean.
- Avoid needless explainer paragraphs, repeated summaries, and process narration in final outputs.
- Do not use missing-evidence disclaimers inside narrative prose. Omit unsupported details or obtain GM permission for controlled embellishment.
- Direct recovered dialogue is preserved with spelling/typo cleanup only.

## Routing Map

| Work | Owner / controlling handoff |
|---|---|
| Priority, canon, architecture, final approval | Chronicle Master — this file |
| Early Wormwood evidence | `handoffs/wormwood-evidence-handoff.md` |
| Man's Promise, Bonewrack, current fork | `handoffs/mans-promise-bonewrack-handoff.md` |
| Bonewrack Arodus 1–4 memory pass | GitHub issue #2 + controlling Bonewrack memory spine |
| PC truth, discovery, player packets | `handoffs/pc-dossiers-player-packets-handoff.md` |
| NPC placement, loyalty, crew viability | `handoffs/npc-crew-state-handoff.md` |
| Narrative sibling outputs | `handoffs/narrative-reconstruction-handoff.md` |
| Visual briefs and art | `handoffs/visual-output-handoff.md` |
| PF2e mechanics audit | `handoffs/pf2e-conversion-handoff.md` |
| Repository architecture and issue protocol | `AGENTS.md` + `design/repository-agent-workflow.md` |

## New Chronicle Master Starter

```text
You are Chronicle Master for FroBoyX/chronicles-of-golarion.

Read `AGENTS.md`, `handoffs/chronicle-master-handoff.md`, `tracking/current-task-board.md`, `tracking/chat-map.md`, `tracking/open-questions.md`, and active GitHub issues relevant to the request.

Keep this chat focused on canon, architecture, priority, routing, cleanup, and final approval. Maintain one authoritative active document per scope. Preserve useful evidence and narrative nuance, but remove stale derived noise, duplicate controls, and known errors from the active lookup path.
```
