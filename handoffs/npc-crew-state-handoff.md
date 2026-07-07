# NPC & Crew State Handoff

## Document Status

- Type: Focused chat handoff
- Maturity: Working control document
- Scope: NPC dossiers, current locations, survivor lists, loyalty buckets, crew viability

## Chat Purpose

Use this chat for NPC and crew state work.

This includes:

- creating and updating NPC dossiers,
- resolving current locations,
- tracking Man's Promise survivors,
- tracking Wormwood vs Man's Promise transfer,
- mapping loyalties,
- deciding who can sail,
- and preventing relaunch-state drift.

## New Chat Starter Prompt

```text
You are the NPC & Crew State auditor for FroBoyX/chronicles-of-golarion. Read `handoffs/npc-crew-state-handoff.md`, `handoffs/chronicle-master-handoff.md`, `state/current-npc-locations.md`, `state/crew-transfer-and-loyalty-audit.md`, `state/current-ship-state.md`, and `tracking/open-questions.md`. Keep NPC placement, loyalty, and survival state grounded in evidence; do not invent loyalties.
```

## Core State Files

- `state/current-npc-locations.md`
- `state/current-ship-state.md`
- `state/crew-transfer-and-loyalty-audit.md`
- `state/current-item-questions.md`
- `state/post-island-decision-space.md`
- `chronology/arodus-5-split-scenes.md`
- `chronology/open-threads.md`

## Man's Promise Named Survivor Set

The six named Man's Promise skeleton-crew survivors are currently fixed as:

| Character | Role | Current Notes |
|---|---|---|
| Dahrehn Numus | Swab | Previously wealthy trader; exact cold-open position unresolved. |
| Ebony Saable | Rigger | Sho's referenced "monk man"; short, dark, bald, leanly muscled, mostly silent. |
| Goyle Onórach | Swab | Rescued from Riptide Cove; with Harvus group; former quartermaster context. |
| Kahina Bukekayo | Rigger | Aboard Man's Promise; testing Sho with life-for-life bargain. |
| Merchiel V'giatore | Rigger | Restrained Nor'gal in first-night Rak confrontation; exact cold-open position unresolved. |
| Nor'gal Daraa | Swab | Revenge thread for brother Kor'al / Cor'Wal; exact cold-open position unresolved. |

Do not conflate the named six with the full survivor count. The count says fourteen surviving captured Man's Promise crew after Harrigan kills one weakened sailor; only six are currently tracked as named skeleton-crew actors.

## Current Location Buckets

### Bonewrack — Harvus Group

- Harvus G'ron
- Mirei
- Sandara Quinn
- Tilly Brackett
- Goyle Onórach

### Bonewrack — Rak Group

- Rak Wraithraiser
- Shivikah
- Slippery Syl Lonegan
- Jaundiced Jape

### Coconut Beach

- Fipps Chumlett, presumed alive.

### Man's Promise — Sho / Survivor Front

- Sho Astor, believed in hot-box.
- Kahina Bukekayo, nearby or recently guarding / interrogating.
- Other named survivors: likely aboard unless specifically placed elsewhere, but exact physical positions unresolved.

### Man's Promise — Command Threat

- Mr. Plugg
- Master Scourge
- Owlbear Hartshorn, likely aboard under Plugg unless Sho's mercy changes him.

### Wormwood-Side / Not Present

- Barnabas Harrigan
- Cut-Throat Grok
- Peppery Longfarthing
- Riaris Krine
- Habbly Quarne
- Caulky Tarroon

### Dead / Removed

- Jakes Magpie
- Rosie Cusswell
- Aretta Bansion
- Giffer Tibbs
- Harmak Gruft
- Kor'al / Cor'Wal Daraa
- The Whale

## Loyalty Buckets

These are working buckets, not final canon.

### Plugg / Scourge Hostile Bloc

Likely or probable:

- Slippery Syl Lonegan
- Jaundiced Jape
- Fipps Chumlett
- possibly Maheem
- possibly Tam Tate
- possibly Kipper
- any Wormwood sailors whose survival depends on Plugg

### PC / Ally-Leaning

Likely or player-evidenced:

- Sandara Quinn
- Tilly Brackett
- Ambrose Kroop
- Goyle Onórach, conditionally
- Badger Medlar, per Rak sheet and social evidence, placement unresolved
- Barefoot Samms Toppin, per Harvus influence evidence
- Jack Scrimshaw, per Rak friendly? note
- Owlbear, if Sho's mercy is actionable

### Man's Promise Survivor Bloc

Likely includes:

- Kahina Bukekayo
- Goyle Onórach
- Ebony Saable
- Dahrehn Numus
- Merchiel V'giatore
- Nor'gal Daraa
- unnamed surviving Man's Promise crew

This bloc may oppose Plugg while still distrusting the PCs.

### Uncommitted / Survival Bloc

Sailors who will support whoever can keep the ship alive, fed, and crewed.

## NPC Dossier Targets

High-priority dossier maintenance:

- `characters/npcs/kahina-bukekayo.md`
- `characters/npcs/goyle-onorach.md`
- `characters/npcs/ebony-saable.md`
- `characters/npcs/dahrehn-numus.md`
- `characters/npcs/merchiel-vgiatore.md`
- `characters/npcs/norgal-daraa.md`
- `characters/npcs/badger-medlar.md`
- `characters/npcs/maheem.md`
- `characters/npcs/shivikah.md`
- `characters/npcs/slippery-syl-lonegan.md`
- `characters/npcs/fipps-chumlett.md`
- `characters/npcs/jaundiced-jape.md`
- `characters/npcs/owlbear-hartshorn.md`
- `characters/npcs/ambrose-fishguts-kroop.md`
- `characters/npcs/cut-throat-grok.md`

## State Questions To Resolve

- Which named survivors are physically aboard the Man's Promise at the cold open?
- Where are Dahrehn, Ebony, Merchiel, and Nor'gal at the exact hot-box moment?
- Who is guarding Sho?
- Who among the survivors supports Kahina's test?
- Which Wormwood NPCs transferred to the Man's Promise and which stayed behind?
- Badger placement: Man's Promise or Wormwood?
- Maheem placement: Man's Promise or Wormwood?
- Patch, Kipper, Tam, Samms, Jack, Ratline, Conchobhar placement.
- Who can sail / rig / cook / lead after a mutiny?
- Whether the crew would accept Sho, Harvus, Rak, Mirei, Goyle, Sandara, or someone else as a command solution.

## Output Style

State updates should be matrix-friendly. Prefer tables for location, status, role, loyalty, and unresolved notes.
