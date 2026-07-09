# NPC & Crew State Handoff

## Document Status

- Type: Focused chat handoff
- Maturity: Working control document, corrected with Erastus 27 ship-split model, Rahadoumi-officer example sequence, and current Man's Promise / Wormwood placement handling
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
You are the NPC & Crew State auditor for FroBoyX/chronicles-of-golarion. Read `handoffs/npc-crew-state-handoff.md`, `handoffs/chronicle-master-handoff.md`, `state/current-npc-locations.md`, `state/mans-promise-crew-viability-reference.md`, `state/crew-transfer-and-loyalty-audit.md`, `state/current-ship-state.md`, and `tracking/open-questions.md`. Keep NPC placement, loyalty, and survival state grounded in evidence; do not invent loyalties.
```

## Core State Files

- `state/current-npc-locations.md`
- `state/mans-promise-crew-viability-reference.md`
- `state/current-ship-state.md`
- `state/crew-transfer-and-loyalty-audit.md`
- `state/current-item-questions.md`
- `state/post-island-decision-space.md`
- `chronology/arodus-5-split-scenes.md`
- `chronology/current-state.md`
- `tracking/open-questions.md`

## Corrected Erastus 27 Ship-Split Model

The Man's Promise and the Wormwood separated on **Erastus 27, 4712 AR**.

Correct sequence:

1. The Wormwood captured the Man's Promise on Erastus 25.
2. The post-battle captured Man's Promise survivor lineup contained 15 captured survivors.
3. Harrigan threw the **only surviving Rahadoumi officer** overboard as an example.
4. Fourteen captured Man's Promise survivors remained alive.
5. Harrigan assigned Mr. Plugg a skeleton crew and Plugg claimed captaincy of the Man's Promise.
6. The Wormwood and the Man's Promise separated.
7. Six named Man's Promise survivors were assigned to Plugg's skeleton crew.
8. The other eight surviving captured Man's Promise crew went with the Wormwood.

Do not place the other eight captured Man's Promise survivors at Bonewrack or aboard the Arodus 5 Man's Promise unless later evidence brings them back.

Do not preserve older active-state language that leaves a Rahadoumi officer alive after Harrigan's example unless later evidence identifies a separate non-officer witness or distinct survivor.

## Ship Crew Viability Reference

The Man's Promise should be treated as a Pathfinder First Edition sailing ship with a **Crew 20** effective-operations reference.

Use this as a pressure tool, not a railroad:

- 20 effective crew means the ship can be sailed properly and sustainably.
- Fewer than 20 may allow emergency movement or short repositioning, but the ship is under-crewed, unsafe, and vulnerable to failed repairs, fatigue, weather, and morale collapse.
- Count only people alive, aboard, capable, and willing or controllable.

## Man's Promise Named Survivor Set

The six named Man's Promise skeleton-crew survivors are currently fixed as:

| Character | Role | Current Notes |
|---|---|---|
| Dahrehn Numus | Swab | Previously wealthy trader; likely Man's Promise, exact cold-open position unresolved. |
| Ebony Saable | Rigger | Sho's referenced `monk man` and Fipps' `dark one` assignment target; short, dark, bald, leanly muscled, mostly silent. |
| Goyle Onórach | Swab / former quartermaster | Rescued from Riptide Cove; with Harvus group; witness against Plugg. |
| Kahina Bukekayo | Rigger | Aboard Man's Promise; testing Sho with life-for-life bargain. |
| Merchiel V'giatore | Rigger | Restrained Nor'gal in first-night Rak confrontation; exact cold-open position unresolved. |
| Nor'gal Daraa | Swab | Revenge thread for brother Kor'al / Cor'Wal; exact cold-open position unresolved. |

Do not conflate the named six with the full survivor count. The count says fourteen surviving captured Man's Promise crew after Harrigan throws the officer overboard. Six of those fourteen are named survivors assigned to Plugg's skeleton crew; the other eight went with the Wormwood.

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

- Sho Astor, believed in or around the hot-box.
- Kahina Bukekayo, nearby or recently guarding / interrogating.
- Other named survivors likely aboard unless specifically placed elsewhere: Dahrehn, Ebony, Merchiel, Nor'gal. Exact physical positions unresolved.

### Man's Promise — Command Threat

- Mr. Plugg
- Master Scourge
- Owlbear Hartshorn, likely aboard under Plugg unless Sho's mercy changes him.

### Man's Promise — Practical / Transfer Network

Evidence-backed or likely Man's Promise-side actors include:

- Ambrose Kroop
- Crimson Cogward
- Ratline Rattsberger
- Tam `Narwhal` Tate
- Barefoot Samms Toppin, strong evidence / likely
- Badger Medlar, GM-corrected aboard; exact position unresolved
- Jack Scrimshaw, GM-corrected aboard; exact position unresolved
- Conchobhar Turlach Shortstone, unresolved placement

### Wormwood-Side / Not Present

- Barnabas Harrigan
- Cut-Throat Grok
- Peppery Longfarthing
- Riaris Krine
- Habbly Quarne
- Caulky Tarroon
- Maheem, believed Wormwood-side
- Kipper, believed Wormwood-side
- Patch Patchsalt, believed Wormwood-side
- the other eight surviving captured Man's Promise crew who went with the Wormwood after the Erastus 27 split

### Dead / Removed

- Jakes Magpie
- Rosie Cusswell
- Aretta Bansion
- Giffer Tibbs
- Harmak Gruft
- Kor'al / Cor'Wal Daraa
- The Whale
- Man's Promise captain
- only surviving Rahadoumi officer thrown overboard by Harrigan

## Loyalty Buckets

These are working buckets, not final canon.

### Plugg / Scourge Hostile Bloc

Likely or probable:

- Mr. Plugg
- Master Scourge
- Slippery Syl Lonegan
- Jaundiced Jape
- Fipps Chumlett
- potentially Owlbear, if Sho's mercy is not actionable
- any hostile Wormwood sailors whose survival depends on Plugg

### PC / Ally-Leaning

Likely or player-evidenced:

- Sandara Quinn
- Tilly Brackett
- Ambrose Kroop
- Goyle Onórach, conditionally
- Badger Medlar, per Rak sheet and social evidence; exact position unresolved
- Barefoot Samms Toppin, per Harvus influence and course-change evidence
- Ratline Rattsberger, per Harvus influence evidence
- Conchobhar, per Harvus influence evidence, placement unresolved
- Jack Scrimshaw, per Rak friendly? note; exact position unresolved
- Owlbear, if Sho's mercy is actionable

### Man's Promise Survivor Bloc

Includes:

- Kahina Bukekayo
- Goyle Onórach
- Ebony Saable
- Dahrehn Numus
- Merchiel V'giatore
- Nor'gal Daraa

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
- `characters/npcs/barefoot-samms-toppin.md`
- `characters/npcs/ratline-rattsberger.md`
- `characters/npcs/crimson-cogward.md`
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
- Can Maheem, Kipper, and Patch be locked Wormwood-side, or should they remain strong GM belief?
- Conchobhar placement.
- Exact positions for Badger, Jack, Tam, Samms, Ratline, and Crimson.
- Who can sail / rig / cook / repair / pump / stand watch / lead after a mutiny?
- Whether the Man's Promise can meet or approximate the Crew 20 effective-operations reference after casualties and refusals.
- Whether the crew would accept Sho, Harvus, Rak, Mirei, Goyle, Sandara, or someone else as a command solution.
- What are the names and later Wormwood-side fates of the other eight captured Man's Promise survivors?

## Output Style

State updates should be matrix-friendly. Prefer tables for location, status, role, loyalty, and unresolved notes.
