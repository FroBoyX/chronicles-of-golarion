# PF1 to PF2e Conversion Handoff

## Document Status

- Type: Focused chat handoff
- Maturity: Working control document
- Scope: Pathfinder 1e to Pathfinder 2e conversion audits for relaunch mechanics

## Chat Purpose

Use this chat to evaluate, prototype, and document Pathfinder 2e conversion options for the Chronicles of Golarion campaign.

This chat does **not** rewrite campaign canon. It converts mechanics for possible future play while preserving PF1 evidence as the historical record.

## Primary Control Files

- `design/pf2e-conversion-method.md`
- `handoffs/chronicle-master-handoff.md`
- `tracking/pf2e-conversion-index.md`

## Primary Archive Inputs

Read these as needed:

- `characters/pcs/harvus-gron.md`
- `characters/pcs/mirei.md`
- `characters/pcs/rak-wraithraiser.md`
- `characters/pcs/sho-astor.md`
- `evidence/player-sheets/`
- `evidence/player-notes/`
- `tracking/open-questions.md`
- `state/current-npc-locations.md`
- `state/current-ship-state.md`
- `state/current-item-questions.md`
- `chronology/current-state.md`
- `chronology/arodus-5-split-scenes.md`

## Primary Output Folders

- `conversions/pf2e/pcs/`
- `conversions/pf2e/npcs/`
- `conversions/pf2e/encounters/`
- `conversions/pf2e/items/`
- `conversions/pf2e/ships/`

## Starter Prompt

```text
You are the PF1 to PF2e Conversion Auditor for FroBoyX/chronicles-of-golarion.

Read:
- `handoffs/pf2e-conversion-handoff.md`
- `design/pf2e-conversion-method.md`
- `handoffs/chronicle-master-handoff.md`
- `tracking/pf2e-conversion-index.md`
- the relevant PC/NPC dossier, item file, encounter file, or ship/state file for the task

Your job is to evaluate and document Pathfinder 1e to Pathfinder 2e conversion options for possible relaunch mechanics.

Do not rewrite campaign canon. Preserve PF1 sheets, rolls, encounters, and outcomes as historical evidence. Rebuild PF2e mechanics by concept, table identity, current story state, and future play needs rather than converting numbers one-for-one.

When making specific PF2e rules recommendations, check current primary rules sources and record the source basis. Offer candidates, tradeoffs, and open questions. Do not lock a PC build, encounter rebuild, item conversion, or ship subsystem without GM approval and, for PCs, player review.
```

## First Task Template

```text
First task: create a PF2e conversion audit for `<target>`.

Target type: PC / NPC / Encounter / Item / Ship / Campaign subsystem.

Before recommending mechanics, report:
- PF1 historical evidence used;
- identity or scene pillars that must be preserved;
- current story-state requirements;
- rules sources that need to be checked;
- likely conversion risks.

Then create or patch the relevant conversion brief under `conversions/pf2e/` and update `tracking/pf2e-conversion-index.md`.
```

## Recommended Pilot Tasks

### Pilot 1 — Sho Astor

Goal: test whether a PC can be rebuilt by concept without losing player-recognizable identity.

Focus:

- Suli / Jalmeray / monk identity;
- discipline, restraint, justice, unarmed combat;
- hot-box / Kahina current state;
- leadership wound after Man's Promise command failure;
- Agatha / cloak / self-control anchors.

### Pilot 2 — Rak Wraithraiser

Goal: test the hardest PC conversion pressure.

Focus:

- Nagaji alchemist / vivisectionist identity;
- cook's mate, booze, alchemy, violence, Besmara;
- Grok / Ambrose / galley loop;
- item dependence and mutagen/alchemy replacement questions;
- current Bonewrack player-knowledge boundaries.

### Pilot Encounter

Goal: test encounter conversion workload.

Suggested targets:

- Sho hot-box / shipboard mutiny-side confrontation.
- Man's Promise deck fight, if replay/reference map and battle mechanics are needed.
- Riptide Cove / Cauldron only after current rescue facts are stable.

## Routing Rules

- Use Chronicle Master for final adoption/rejection of PF2e conversion as relaunch mechanics.
- Use PC Dossiers / Player Packets for player-facing character truth, not mechanics conversion.
- Use Evidence Intake when raw PF1 source material has not yet been preserved.
- Use NPC & Crew State Audit when current positions, loyalties, or survival states block conversion.
- Use Battle Map Forge for visual/top-down map generation after encounter mechanics and tactical truth are clear.

## End-of-Task Report

End conversion tasks with:

```text
PF2e conversion task complete.

Created:
- path
  Commit: shortsha — message

Updated:
- path
  Commit: shortsha — message

Conversion target:
- ...

Recommended candidate:
- ...

Preserves:
- ...

Risks / losses:
- ...

Open conversion questions:
- ...

Next recommended conversion step:
- ...
```
