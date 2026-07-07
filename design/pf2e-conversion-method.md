# PF1 to PF2e Conversion Method

## Document Status

- Type: Design note / conversion workflow
- Maturity: Working control document
- Scope: Pathfinder 1e to Pathfinder 2e conversion audits for PCs, NPCs, encounters, items, ships, and relaunch mechanics
- Owner: GM / canon authority

## Purpose

This document defines how the archive evaluates and performs a possible conversion from Pathfinder 1e to Pathfinder 2e without damaging the preserved PF1 campaign record.

PF2e conversion is a **relaunch mechanics layer**, not a rewrite of campaign history.

The original Pathfinder 1e sheets, rolls, encounters, and table outcomes remain historical evidence. PF2e builds are reconstructed tools for future play.

## Core Principles

### Preserve PF1 Evidence

Do not overwrite or discard PF1 sheets, PCGen exports, Foundry exports, chat logs, item notes, or encounter evidence.

PF1 material remains the archive's evidence for what happened at the table.

### Convert Concept, Not Numbers

Do not attempt direct one-for-one conversion of:

- BAB;
- saving throws;
- skill ranks;
- feat chains;
- class feature math;
- wealth-by-level totals;
- monster stat blocks;
- encounter CR.

Instead, rebuild the playable PF2e version from:

- character concept;
- ancestry/species identity;
- role in the party;
- table behavior;
- relationship arc;
- signature actions;
- signature gear;
- current story state.

### Separate Historical Canon From Relaunch Mechanics

Use these labels:

- **PF1 Historical Evidence** — what the original campaign used.
- **Conversion Candidate** — proposed PF2e rebuild, not approved.
- **Relaunch Mechanics** — approved mechanics for resumed play.
- **Rejected Conversion** — tested but not adopted.
- **Open Conversion Question** — unresolved mechanical or concept issue.

### Player Identity Matters

PC conversion must preserve what the player recognizes as the character.

A technically legal PF2e build that loses the character's table identity should be treated as a failed conversion candidate.

### Current Rules Must Be Checked

When making specific PF2e rules recommendations, check current primary rules sources rather than relying on memory.

Acceptable source categories:

- official Paizo rulebooks or PDFs available to the GM;
- Archives of Nethys PF2e pages;
- Foundry PF2e system documentation for implementation details;
- GM-provided rule excerpts or purchased source references.

Record the source basis in the conversion brief.

## Conversion Evidence Hierarchy

Use this order when conversion sources conflict:

1. GM conversion decision / current user confirmation.
2. Player-approved character identity and current discovery answers.
3. PF1 historical sheets and campaign evidence.
4. PC/NPC dossiers and relationship files.
5. Current PF2e primary rules sources.
6. Foundry PF2e implementation constraints.
7. Conversion convenience.

## Conversion Streams

### PC Conversion

For player characters:

1. Read the PC dossier and player discovery material.
2. Read PF1 sheet/export evidence.
3. Identify the character's non-negotiable identity pillars.
4. Identify PF1 mechanics that were table-important.
5. Propose 2-3 PF2e build paths if the mapping is uncertain.
6. Explain what each path preserves and what it loses.
7. Do not lock a build without GM and player sign-off.

### NPC Conversion

For NPCs:

1. Identify campaign function first: ally, threat, crew actor, officer, survivor, witness, ship specialist.
2. Decide whether the NPC needs a full PF2e stat block, a simple DC/role, or narrative-only treatment.
3. Use existing PF2e creatures or NPC stat blocks when possible.
4. Custom-build only when the NPC is mechanically important.

### Encounter Conversion

For encounters:

1. Preserve the table outcome and scene purpose.
2. Rebuild encounter challenge using PF2e encounter math.
3. Use PF2e creatures, hazards, terrain, and conditions rather than direct PF1 stat conversion.
4. Record whether the converted encounter is for replay, flashback reference, or future resumed play.
5. Do not let the converted version imply the old PF1 table outcome should have been different.

### Item and Treasure Conversion

For items:

1. Identify story-significant items separately from disposable gear.
2. Convert item function and story role before value.
3. Rebuild treasure using PF2e expectations if resumed play uses PF2e.
4. Mark PF1 item values as historical, not relaunch balance.

### Ship / Naval Conversion

For ships and sea travel:

1. Preserve ship identity and current state from the archive.
2. Identify whether ship rules need full mechanics or scene-level procedures.
3. Use current PF2e nautical rules or GM-approved subsystems where available.
4. Do not convert shipboard social pressure into pure mechanics; the campaign depends on crew relationships and command legitimacy.

## Minimum PC Conversion Brief

```md
# <PC Name> PF2e Conversion Brief

## Document Status

- Type: PF2e PC conversion brief
- Maturity: Draft / Candidate / Player-reviewed / GM-approved / Rejected / Superseded
- PF1 source status: <sheet/export/evidence used>
- PF2e status: Conversion candidate / Relaunch mechanics
- Spoiler scope: Player-safe / GM-only / Character-limited

## Source Basis

- PF1 sheet/export evidence:
- PC dossier:
- Player discovery:
- Current-state files:
- PF2e rules sources checked:
- Foundry/PF2e implementation notes:

## Character Identity Pillars

- 

## PF1 Historical Mechanical Identity

- 

## Current Story State Requirements

- 

## PF2e Build Path Candidates

| Path | Ancestry/Heritage | Background | Class | Archetype(s) | Preserves | Loses / Risks | Status |
|---|---|---|---|---|---|---|---|

## Recommended Candidate

- 

## Open Conversion Questions

- 

## Player / GM Sign-Off

- Player reviewed:
- GM approved:
- Notes:
```

## Minimum Encounter Conversion Brief

```md
# <Encounter> PF2e Conversion Brief

## Document Status

- Type: PF2e encounter conversion brief
- Maturity: Draft / Candidate / GM-approved / Rejected / Superseded
- Purpose: Replay / Relaunch future encounter / Reference only
- Spoiler scope: Player-safe / GM-only

## Source Basis

- PF1 evidence:
- AP/campaign scaffold:
- Chronology/state files:
- PF2e rules sources checked:

## Historical PF1 Scene Function

- 

## Table Outcome To Preserve

- 

## PF2e Encounter Goal

- 

## Conversion Proposal

- Party level assumption:
- Encounter difficulty target:
- Creature/NPC choices:
- Hazards/terrain:
- Rewards/items:

## Open Conversion Questions

- 
```

## Tracking

Use `tracking/pf2e-conversion-index.md` to track conversion targets and statuses.

Recommended conversion output paths:

```text
conversions/pf2e/pcs/<pc-slug>.md
conversions/pf2e/npcs/<npc-slug>.md
conversions/pf2e/encounters/<encounter-slug>.md
conversions/pf2e/items/<item-or-treasure-slug>.md
conversions/pf2e/ships/<ship-slug>.md
```

## Recommended Pilot

Run a narrow pilot before committing to a full campaign conversion.

Suggested pilot sequence:

1. Convert one PC by concept.
2. Convert one immediate scene or encounter.
3. Test whether the PC still feels like themselves.
4. Estimate workload for the remaining PCs and current relaunch state.
5. Decide whether PF2e conversion is adopted, deferred, or rejected.

Recommended first PC pilot:

- Sho Astor, because her current hot-box / mutiny-side role tests moral authority, monk identity, and combat readiness without immediately depending on complex alchemy conversion.

Recommended second PC pilot:

- Rak Wraithraiser, because he is likely the hardest concept to preserve mechanically and should be tested before committing.

## End-of-Task Report

Every PF2e conversion task should end with:

- Created paths
- Updated paths
- Commit IDs, if repo files changed
- Conversion target
- Source basis
- Recommended candidate, if any
- What the candidate preserves
- What the candidate loses or risks
- Open conversion questions
- Next recommended conversion step
