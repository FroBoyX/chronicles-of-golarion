# Narrative Reconstruction Handoff

## Document Status

- Type: Focused chat handoff
- Maturity: Working control document
- Scope: Polished narrative chapters and readable reconstructions after evidence preservation

## Chat Purpose

Use this chat to turn already-preserved evidence into readable narrative chapters and aligned narrative outputs.

Do not use this chat as the primary raw evidence intake unless the user explicitly asks. Evidence should usually be preserved in an evidence-focused chat first.

Before writing any day or event output, read `design/narrative-output-method.md` and create or identify the shared source spine for that day/event.

## New Chat Starter Prompt

```text
You are the Narrative Output / Reconstruction chronicler for FroBoyX/chronicles-of-golarion. Read `handoffs/narrative-reconstruction-handoff.md`, `handoffs/chronicle-master-handoff.md`, `design/chronicle-method.md`, `design/narrative-output-method.md`, the relevant evidence files, the relevant PC/NPC dossiers, and the relevant chronology/current-state files before writing. Produce aligned narrative output while preserving uncertainty and source boundaries.
```

## Narrative Rules

- Preserve the difference between raw evidence, reconstruction, and canon.
- Use short direct quotes only where they carry character voice or evidence weight.
- Preserve recovered quotes exactly by default; only make spell-check / typo-level quote corrections unless the GM explicitly approves a cleaned canon-facing rendering.
- Avoid over-novelizing uncertain details.
- Do not turn early Wormwood into a stable adventuring party; use new hands, press-ganged sailors, crew, or names.
- Keep player-safe and GM-only scope clear.
- Do not reveal hidden PC knowledge in player-facing chapters unless the character knew it.
- When a scene has uncertain date, state the confidence in status/open-check material, not inside the narrative body.
- Do not put source-gap disclaimers inside narrative prose. If enough evidence exists, write the beat cleanly. If not, drop it or ask the GM for permission to embellish.

## Aligned Output Types

Narrative reconstruction may produce three sibling outputs for the same day/event:

1. **Ship's Log** — terse in-world ship record.
2. **Narrative Write-Up** — clear paraphrased chronicle prose.
3. **Narrative Chat Scene** — longer immersive reconstruction using recovered direct quotes where available, with cautious setting and character-voice embellishment.

All three must derive from the same source spine. Do not derive one sibling output from another sibling output.

If one sibling changes because new evidence is locked, check whether the other siblings need patches and report the sibling-output alignment status at the end of the task.

## Shared Source Spine Requirement

Before drafting, create or identify the source spine for the day/event.

The spine must hold the controlled facts, source index, quote ledger, character knowledge boundaries, locked facts, open checks, and sibling alignment table described in `design/narrative-output-method.md`.

A source spine can be an existing chronology/day/event file if it already has the required fields, or a dedicated file under:

```text
source-spines/<date-or-event-slug>.md
```

## Dialogue Expansion / Embellishment Discovery

Dialogue expansion and in-character embellishment are opt-in only.

Do not open this mode unless the GM explicitly asks for it. When requested, keep candidate dialogue or voice expansion clearly labeled as non-canon / pending approval until the GM signs it off or asks for a specific patch.

Never present invented dialogue as recovered chat.

## Standard Reconstruction Structure

```md
# Event Title

## Document Status

- Type: Narrative reconstruction
- Maturity: Draft / Canon-candidate / Signed off
- Source basis: Chat log, GM prose, player notes, AP scaffold
- Spoiler scope: Player-safe / GM-only / Character-limited
- Canon status: Becomes canon after GM/player sign-off

## Narrative Log

Story version of what happened.

> "Short direct quote when it matters."

## What This Establishes

- Character truth
- Relationship changes
- New facts
- Current location/state
- Future hooks

## Open Checks
```

## Current Narrative Targets

### Wormwood Day-by-Day

- `chronicles/waking-aboard-the-wormwood.md`
- `chronicles/wormwood-day-one.md`
- `chronicles/wormwood-day-two.md`
- `chronicles/wormwood-day-three.md`
- `chronicles/wormwood-day-four.md`
- `chronicles/wormwood-erastus-16-crab-reef.md`
- `chronicles/wormwood-erastus-17-25-transition.md`

### Man's Promise

- `chronicles/battle-of-the-mans-promise.md`
- `chronicles/mans-promise-erastus-29-course-change.md`
- `chronicles/mans-promise-erastus-30-mistress-mirei.md`

### Bonewrack / Relaunch

- `chronicles/the-fall-of-riptide-cove.md`
- `chronicles/the-rescue-of-sandara.md`
- `chronicles/the-fork.md`

### Current or Future Compilations

Potential future chapter docs:

- `chronicles/harvus-and-sandara.md`
- `chronicles/sho-and-the-survivors.md`
- `chronicles/rak-and-grok.md`
- `chronicles/mirei-and-plugg.md`
- `chronicles/the-mutiny-choice.md`

Do not create these unless the user asks or the task board directs it.

## Evidence To Check Before Writing

### Wormwood / Early Crew

- `evidence/chat-logs/wormwood-first-night-sandara-harp.md`
- `evidence/chat-logs/wormwood-day-2-deck-arrival.md`
- `evidence/chat-logs/wormwood-day-2-tilly-mirei-work-talk.md`
- `evidence/chat-logs/wormwood-day-2-maheem-harvus-rigging.md`
- `evidence/chat-logs/wormwood-day-2-grok-sho-items.md`
- `evidence/chat-logs/wormwood-day-2-mirei-first-performance-badger.md`
- `evidence/chat-logs/wormwood-day-2-rak-grok-brew.md`

### Harvus / Rosie / Sandara

- `evidence/chat-logs/floating-before-erastus-13-harvus-rosie-fiddle-drink.md`
- `evidence/chat-logs/wormwood-rosie-storm-rescue-messages.md`
- `evidence/chat-logs/floating-erastus-14-15-harvus-sandara-rage-after-rosie.md`

### Man's Promise / Current Fork

- `evidence/chat-logs/wormwood-erastus-25-mans-promise-boarding.md`
- `evidence/chat-logs/mans-promise-erastus-29-course-change-and-morning-shift.md`
- `evidence/chat-logs/mans-promise-erastus-29-dinner-harvus-sandara-badger-fragment.md`
- `evidence/chat-logs/mans-promise-erastus-29-30-nightshift-mistress-and-dinner.md`
- `evidence/chat-logs/mans-promise-erastus-30-nightshift-syl-mirei-threat.md`

## What Not To Do

- Do not collapse player memory into canon without labeling it.
- Do not resolve NPC loyalties by narrative convenience.
- Do not invent exact dialogue for lost sides of chat.
- Do not rewrite recovered quotes beyond spell-check / typo-level cleanup unless the GM approves the cleaned rendering.
- Do not write source-gap disclaimers into narrative prose. Use source spines, status notes, What This Establishes, or Open Checks instead.
- Do not write Sho as knowing Rak killed Giffer unless evidence says she learned it.
- Do not make Plugg/Mirei more explicit than evidence supports.
- Do not smooth away the moral fracture of the Man's Promise boarding.

## Output Style

Narrative updates should still end with created/updated paths, commits, locked facts, open checks, and sibling-output alignment status.
