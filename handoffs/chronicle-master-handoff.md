# Chronicle Master Handoff

## Document Status

- Type: Chat handoff / routing document
- Maturity: Working control document
- Scope: Chronicles of Golarion archive split, roles, evidence workflow, current priorities
- Owner: GM / canon authority
- Assistant role: Archivist, chronicler, continuity lead

## Purpose

This file lets new chats resume the archive without requiring the entire prior conversation.

The repository should be treated as the durable memory. Chats should stay narrow and write back to the repo whenever they establish facts, preserve evidence, resolve questions, or create approved process scaffolding.

## Core Campaign Context

- Campaign: Pathfinder, Skull & Shackles, archived under **Chronicles of Golarion**.
- Current project: reconstruct, preserve, and relaunch the old campaign from surviving chat logs, player sheets, Obsidian Portal notes, GM memory, and Adventure Path scaffold.
- Current relaunch point: Arodus 5, around the Bonewrack / Man's Promise fork.
- Opening date currently locked by GM correction: Erastus 4, 4712 AR for press-ganging in Port Peril; Erastus 5, 4712 AR for waking aboard the Wormwood.
- If older files still say 4691 AR, treat that as a cleanup target unless a later GM decision overrides the 4712 correction.

## Evidence Hierarchy

Use this order when sources conflict:

1. GM truth / current user confirmation.
2. Obsidian Portal evidence.
3. Campaign chat logs.
4. Player journals and player notes.
5. GM memory, when clearly identified as memory.
6. Published Adventure Path baseline / scaffold.

Evidence labels in use:

- Canon
- Reported
- Perspective
- Unresolved
- Superseded
- Unknown

## Standard Workflow

For new evidence, use:

```text
Evidence -> Extract -> Narrative Reconstruction -> Open Checks
```

When the user provides a scene chunk:

1. Preserve the raw evidence in `evidence/chat-logs/`, `evidence/gm-notes/`, `evidence/obsidian-portal/`, or the correct evidence folder.
2. Extract facts conservatively.
3. Integrate into a day doc, event doc, PC dossier, NPC dossier, relationship doc, or state doc only where supported.
4. Add open checks for anything unresolved.
5. Report created/updated paths and commits.

## Narrative Output Workflow Pass-Off

The Narrative Output / Reconstruction workflow has a dedicated method file:

- `design/narrative-output-method.md`

Chronicle Master should treat that file as the current control document for polished narrative output.

Key adopted workflow:

- Narrative output can produce three sibling forms for the same day/event:
  1. **Ship's Log** — terse in-world ship record.
  2. **Narrative Write-Up** — clear paraphrased chronicle prose.
  3. **Narrative Chat Scene** — longer immersive reconstruction using recovered direct quotes where available.
- Before drafting any sibling output, the Narrative Output chat must create or identify a shared source spine.
- The sibling outputs derive from the source spine, not from each other.
- Dedicated source spines live under `source-spines/` when an existing chronology/day/event file does not already contain the required source-spine fields.
- Source spines track source index, timeline beats, quote ledger, character knowledge boundaries, locked facts, open checks, and sibling-output alignment.
- AP scaffold and GM-provided campaign encounter data may be used for encounter structure, environmental context, hazards, travel pressure, enemy placement, and connective tissue, but cannot overwrite recovered table evidence or GM-locked outcomes.
- Narrative time skips, scene jumps, and context bridges are allowed to avoid unnecessary backfill, but cannot hide unresolved canon problems or invent exact dialogue.
- Dialogue expansion / in-character embellishment is opt-in only. It should be opened only when the GM explicitly requests it, and candidate dialogue must not be presented as recovered chat or canon unless approved.

## Visual Output Workflow Pass-Off

The Visual Output / Art Direction workflow has a dedicated method file and style seed:

- `design/visual-output-method.md`
- `design/visual-style-guide.md`
- `handoffs/visual-output-handoff.md`
- `tracking/image-output-index.md`

Chronicle Master should treat `design/visual-output-method.md` as the current control document for character art, location art, battle maps, visual briefs, and asset-index discipline.

Key adopted workflow:

- Visual output has three production streams:
  1. **Character Art** — portraits, full-body references, crew portraits, expression/action/outfit/state variants.
  2. **Location Art** — establishing shots, interiors, ship spaces, island vistas, and scene backdrops.
  3. **Battle Maps** — top-down tactical maps, player-safe maps, GM annotated variants, grid/no-grid variants.
- Visual output should create or identify a visual brief before major image generation.
- Visual briefs live under `visual-briefs/characters/`, `visual-briefs/locations/`, and `visual-briefs/maps/`.
- Approved or working anchor assets should guide later variants.
- Character and location illustration can prioritize mood and identity; battle maps are truth-first and must preserve tactical geometry.
- Existing Pathfinder/Golarion/Skull & Shackles/Paizo images may be used for setting cues, material culture, palette, silhouette families, and mood, but not as direct-copy targets.
- Generated images are not canon by themselves. They become visual canon only after GM sign-off or explicit approval.
- The image-output index records planned, briefed, draft, working-anchor, approved, variant, rejected, and superseded assets.

## PF2e Conversion Workflow Pass-Off

The PF1 to PF2e Conversion Audit workflow has a dedicated method file and tracking index:

- `design/pf2e-conversion-method.md`
- `handoffs/pf2e-conversion-handoff.md`
- `tracking/pf2e-conversion-index.md`
- `conversions/pf2e/`

Chronicle Master should treat `design/pf2e-conversion-method.md` as the current control document for conversion audits and possible relaunch mechanics.

Key adopted workflow:

- PF2e conversion is a **relaunch mechanics layer**, not a rewrite of campaign history.
- PF1 sheets, rolls, encounters, and outcomes remain historical evidence.
- Conversion should rebuild by concept, table identity, current story state, and future play needs rather than converting numbers one-for-one.
- PC conversions require player review and GM approval before becoming relaunch mechanics.
- Specific PF2e rules recommendations should check current primary rules sources and record the source basis.
- Conversion outputs live under `conversions/pf2e/pcs/`, `conversions/pf2e/npcs/`, `conversions/pf2e/encounters/`, `conversions/pf2e/items/`, and `conversions/pf2e/ships/`.
- The conversion index tracks not-started, draft, candidate, review-needed, approved, rejected, and superseded conversion targets.

Chronicle Master routing note:

- Use Narrative Output / Reconstruction for player-facing or readable prose once evidence is already preserved.
- Use Visual Output / Art Direction for visual briefs, image prompts, art continuity, and battle-map prompts once the relevant facts are stable enough.
- Use PF1 to PF2e Conversion Audit for mechanics conversion, PC/NPC rebuild candidates, encounter conversion, item conversion, and ship/naval subsystem options.
- Use evidence-intake chats first when the source material has not yet been preserved.
- Use NPC & Crew State Audit before visualizing or converting current-state tableaux if positions, loyalties, or survival states are unresolved.
- Use Chronicle Master only for priority, canon, scope, routing, and final sign-off decisions.

## Language Rules

- Do not write early Wormwood as a normal adventuring party. Use **new hands**, **press-ganged crew**, **crew**, or character names.
- Keep uncertain material marked as current reconstruction / pending confirmation.
- Preserve raw chat spelling and phrasing in evidence files.
- Clean prose is acceptable in chronicles, but do not silently change facts.
- Use direct, practical final summaries with commit IDs.

## Split Chat Map

Use these handoffs to start focused chats:

| Chat | Handoff | Purpose |
|---|---|---|
| Chronicle Master / Router | `handoffs/chronicle-master-handoff.md` | Direction, priority, canon, scope, and final decisions only. |
| Wormwood Evidence Intake | `handoffs/wormwood-evidence-handoff.md` | Erastus 4-24 Wormwood evidence, day docs, lower-crew scenes. |
| Man's Promise / Bonewrack Evidence Intake | `handoffs/mans-promise-bonewrack-handoff.md` | Boarding, prize crew, Bonewrack, current fork, hot-box, mutiny setup. |
| PC Dossiers / Player Packets | `handoffs/pc-dossiers-player-packets-handoff.md` | PC facts, player-safe questions, cold-open packets. |
| NPC & Crew State Audit | `handoffs/npc-crew-state-handoff.md` | NPC dossiers, locations, survivor lists, loyalty, who can sail. |
| Narrative Reconstruction | `handoffs/narrative-reconstruction-handoff.md` | Polished chapters and aligned Ship's Log / Write-Up / Chat Scene outputs after evidence has been preserved. |
| Visual Output / Art Direction | `handoffs/visual-output-handoff.md` | Character art, location art, battle maps, visual briefs, asset tracking, and style continuity. |
| PF1 to PF2e Conversion Audit | `handoffs/pf2e-conversion-handoff.md` | Conversion audits for PCs, NPCs, encounters, items, ships, and possible relaunch mechanics. |

## Tracking Files

Use these to keep chats from bloating:

- `tracking/chat-map.md` — where each kind of task should go.
- `tracking/current-task-board.md` — active and next tasks.
- `tracking/evidence-ingestion-queue.md` — raw or pending evidence not fully integrated.
- `tracking/open-questions.md` — cross-cutting unresolved questions.
- `tracking/image-output-index.md` — visual asset status, anchors, variants, and remake/patch policy.
- `tracking/pf2e-conversion-index.md` — PF2e conversion target status, candidates, approvals, rejected paths, and risks.

## Current Core State

### Bonewrack — Harvus Group

- Harvus G'ron
- Mirei
- Sandara Quinn
- Tilly Brackett
- Goyle Onórach

They are returning from Riptide Cove after the rescue. Harvus killed the Whale with Rak's spear. Mirei confessed Plugg's task to betray/kill the other PCs but did not act on it.

### Bonewrack — Rak Group

- Rak Wraithraiser
- Shivikah
- Slippery Syl Lonegan
- Jaundiced Jape

They are moving through the island. Fipps Chumlett was left at Coconut Beach because the Man's Promise was expected there.

### Man's Promise — Sho Front

- Sho Astor is believed locked in or around the hot-box.
- Kahina Bukekayo has tested Sho with a life-for-life moral bargain.
- The Man's Promise survivor bloc matters; they may oppose Plugg while still distrusting the PCs.

### Command Threat

- Mr. Plugg claims command of the Man's Promise.
- Master Scourge is Plugg's enforcer.
- Owlbear is likely still under Plugg's control unless Sho's prior mercy changes that.

## Confirmed / Working Major Threads

- Harvus / Sandara relationship and grief thread.
- Harvus / Rosie fiddle and post-Rosie rage scenes.
- Rak / Grok friendship, alcohol, galley loop, later hookup, and sentimental separation.
- Sho's Man's Promise guilt, surrender-command fracture, Harrigan pendant, and hot-box state.
- Mirei / Plugg manipulation thread, including "mistress" framing and unacted betrayal assignment.
- Man's Promise survivor set and survivor distrust.
- Current crew viability: who can sail, who will fight, who will defect, and who will obey Plugg.

## Important Existing Index Docs

Read these when beginning a major new chat:

- `CANON.md`
- `design/chronicle-method.md`
- `design/narrative-output-method.md`
- `design/visual-output-method.md`
- `design/visual-style-guide.md`
- `design/pf2e-conversion-method.md`
- `source-spines/README.md`
- `tracking/image-output-index.md`
- `tracking/pf2e-conversion-index.md`
- `chronology/current-state.md`
- `chronology/arodus-5-split-scenes.md`
- `chronology/open-threads.md`
- `state/current-npc-locations.md`
- `state/current-ship-state.md`
- `state/crew-transfer-and-loyalty-audit.md`
- `state/current-item-questions.md`
- `book-1/overview.md`
- `book-1/wormwood.md`
- `book-1/mans-promise.md`
- `book-1/bonewrack-isle.md`

## New Chat Starter Prompt

Use this to start a new master/router chat:

```text
You are the Chronicle Master / Router for FroBoyX/chronicles-of-golarion. Read `handoffs/chronicle-master-handoff.md`, `tracking/current-task-board.md`, `tracking/chat-map.md`, `tracking/open-questions.md`, `design/narrative-output-method.md`, `design/visual-output-method.md`, and `design/pf2e-conversion-method.md`. Keep this chat focused on priorities, canon decisions, scope, and routing. Do not ingest large raw evidence here unless asked.
```
