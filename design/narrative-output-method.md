# Narrative Output Method

## Document Status

- Type: Design note / narrative output workflow
- Maturity: Working control document
- Scope: Ship's logs, narrative write-ups, narrative chat scenes, and their shared source spine
- Owner: GM / canon authority

## Purpose

This document defines how preserved evidence becomes three aligned narrative outputs without losing source boundaries or accidentally upgrading reconstruction into canon.

The three sibling outputs are:

1. **Ship's Log** — terse in-world ship record for a day or event.
2. **Narrative Write-Up** — clear paraphrased chronicle prose.
3. **Narrative Chat Scene** — longer immersive reconstruction using recovered direct quotes where available, with cautious setting and character-voice embellishment.

All three outputs must derive from the same source spine for the day or event.

## Shared Source Spine Rule

Before drafting any of the three sibling outputs, create or identify a shared source spine for the target day or event.

The source spine is not polished prose. It is the controlled factual layer that all sibling outputs use.

A source spine may be an existing chronology/day/event file if it already contains the required fields, or a dedicated spine file if the event needs one.

Recommended dedicated path pattern:

```text
source-spines/<date-or-event-slug>.md
```

Do not derive one sibling output from another sibling output. Derive each from the source spine.

## Source Spine Minimum Fields

```md
# <Date/Event> Source Spine

## Document Status

- Type: Source spine
- Maturity: Draft / Working / Locked
- Scope: <day/event>
- Source basis: <evidence files, dossiers, chronology files, state files>
- Spoiler scope: Player-safe / GM-only / Character-limited
- Canon status: <working / canon-candidate / signed off>

## Source Index

- Evidence:
- PC dossiers:
- NPC dossiers:
- Chronology/state:
- AP scaffold:
- Campaign encounter data:
- GM corrections:

## Timeline Beats

| Beat | Time/Order | Fact | Evidence | Confidence | Visibility |
|---|---|---|---|---|---|

## Quote Ledger

| Speaker | Exact recovered quote | Source | Use status | Notes |
|---|---|---|---|---|

Use status options:

- **Exact usable** — may be quoted directly.
- **Exact but limited** — quote only in the output whose spoiler scope permits it.
- **Paraphrase only** — preserve meaning, do not quote.
- **Missing side** — do not invent exact dialogue.
- **GM/player memory** — label as memory unless later confirmed.

## Character Knowledge Boundaries

| Character | Knows | Does not know | Output implications |
|---|---|---|---|

## Locked Facts

- 

## Open Checks

- 

## Sibling Output Alignment

| Output | Path | Status | Alignment notes |
|---|---|---|---|
| Ship's Log |  | Not started / Draft / Patched / Locked |  |
| Narrative Write-Up |  | Not started / Draft / Patched / Locked |  |
| Narrative Chat Scene |  | Not started / Draft / Patched / Locked |  |
```

## Quote Handling

Recovered direct quotes should remain exact unless the GM explicitly approves a canon-facing cleaned rendering.

Default quote policy:

- Preserve recovered wording, phrasing, syntax, and character diction.
- Only make spell-check / typo-level corrections when the correction does not alter character voice, word choice, meaning, or cadence.
- Do not rewrite a recovered quote into smoother prose.
- If a quote needs heavier cleanup for player-facing readability, either paraphrase it outside quotation marks or ask the GM to approve the cleaned version.
- Never present invented or completed dialogue as recovered chat.

## Source-Gap Handling In Narrative Outputs

Do not put archive-process disclaimers inside the narrative prose.

Avoid phrases such as:

- `the details did not survive`,
- `the logs are missing`,
- `we do not know`,
- `the current reconstruction is`,
- `not enough evidence survives`,
- or similar meta-statements inside the Ship's Log, Narrative Write-Up, or Narrative Chat Scene body.

Use this rule instead:

- If the source spine has enough support, write the supported beat cleanly.
- If the source spine does not have enough support, either drop the beat from the narrative body or ask the GM for permission to embellish.
- Put source gaps, uncertainty, and missing-evidence notes in the source spine, Document Status, What This Establishes, or Open Checks — not in the narrative prose itself.
- Do not use narrative prose to apologize for missing evidence.

## Source Use: AP / Campaign Encounter Data

Published Adventure Path material and GM campaign encounter data may be used as scaffold when building narrative output, especially for encounter structure, environmental context, travel pressure, hazards, enemy placement, and skipped connective tissue.

Rules:

- Treat AP material as scaffold, not proof that the table event happened exactly that way.
- Treat GM-provided campaign encounter data as stronger than AP baseline, but still keep it distinct from recovered chat unless the chat confirms the moment.
- Ask the GM for AP/campaign encounter details when the preserved evidence clearly depends on encounter context that is not yet in the repo.
- Use AP/campaign data to support plausible framing, not to overwrite player action, table-specific outcomes, or established character knowledge.
- Label the source basis clearly in the source spine.

## Narrative Compression and Scene Movement

Narrative output does not need to backfill every gap between preserved scenes.

Allowed techniques:

- **Time skips** — move over routine work, travel, watch rotations, sleep, or uneventful days when detailed reconstruction would add little.
- **Scene jumps** — cut between shipboard areas, PC groups, NPC pressure points, or parallel island/ship action for clarity or dramatic effect.
- **Context bridges** — summarize missing connective tissue in neutral prose when enough source support exists.
- **Unresolved gaps** — leave gaps explicit in source spines or open checks when evidence is absent or when backfilling would invent facts.

Rules:

- Do not use a time skip to hide an unresolved canon problem.
- Do not create exact dialogue inside a skipped or bridged period unless recovered evidence provides it.
- If a jump changes character perspective, keep hidden knowledge boundaries intact.
- If a skipped span includes known hazards, losses, discipline, relationship beats, or route changes, note them in the source spine even if the final prose compresses them.

## Output Definitions

### Ship's Log

Purpose: a terse, in-world record of ship movement, command decisions, weather, discipline, watches, encounters, casualties, and major crew state.

Voice / hand:

- Ship's Logs are **end-of-day official shipboard duty-log entries** compiled from watch/officer reports.
- They are **not** Captain Harrigan's personal diary and not a real-time deck-watch transcript.
- The default hand is an unnamed shipboard log-keeper / duty officer writing under the authority of the ship's command structure.
- On the Wormwood, this means the log reflects the administrative hand of the ship under Harrigan's command and, for daily crew discipline and assignments, under Mr. Plugg's practical authority.
- Use `ship-logs/README.md` as the style authority for ship-log voice.

Rules:

- Use the source spine's locked and high-confidence facts.
- Keep prose sparse and practical.
- Avoid interiority unless the log-writer would plausibly record it.
- Do not reveal hidden PC knowledge.
- Do not include uncertain reconstruction unless marked as rumor, report, or unresolved.
- Remember that the Ship's Log is an in-world official record, not omniscient truth; it may euphemize or flatten events from the command perspective.

### Narrative Write-Up

Purpose: a readable chronicle prose version of what happened.

Rules:

- Use clear paraphrase first.
- Use direct quotes only where they carry evidence weight or character voice.
- Preserve uncertainty and source boundaries outside the narrative body, using status/source/open-check sections.
- Keep character knowledge boundaries intact.
- Do not smooth away moral fractures, contradictory perspectives, or unresolved loyalties.
- Use time skips, scene jumps, and context bridges when they produce a cleaner reconstruction without inventing facts.
- Do not include source-gap disclaimers in the prose body; drop unsupported detail or ask the GM for embellishment approval.

### Narrative Chat Scene

Purpose: an immersive reconstruction suitable for table/player reading when the GM wants a scene-like version.

Rules:

- Use recovered direct quotes where available.
- Add setting, pacing, transitions, and body-language cautiously.
- Embellish character voice only around established facts and recovered tone.
- Do not invent exact dialogue for missing chat.
- If a line is not recovered, write it as narration or clearly marked paraphrase.
- Keep hidden PC knowledge out of player-facing versions unless the perspective character knew it.
- Scene cuts and time skips are allowed for effect, but should remain visibly anchored to the source spine.
- Do not include source-gap disclaimers in the scene body; drop unsupported detail or ask the GM for embellishment approval.

## Patch Policy

If an output already exists, patch the relevant section instead of regenerating the entire file unless the GM explicitly asks for a rewrite.

When patching sibling outputs:

1. Update the source spine first.
2. Patch each affected output from the updated spine.
3. Record the alignment status at the end of the task.

## Dialogue Expansion / Embellishment Discovery

Dialogue expansion and in-character embellishment are optional discovery work, not part of the default reconstruction pass.

Only open this mode when the GM explicitly asks for it.

When requested, keep it separate from locked narrative output until approved. Acceptable labels include:

- `Candidate dialogue`
- `Voice expansion draft`
- `Non-canon embellishment pending approval`

Rules for dialogue discovery:

- Never present invented dialogue as recovered chat.
- Preserve all recovered direct quotes exactly when quoting them, aside from GM-approved spell-check / typo-level corrections.
- Use candidate dialogue to explore voice, not to establish facts.
- Do not commit candidate dialogue into canon-facing outputs unless the GM signs it off or asks for that specific patch.

## End-of-Task Report

Every narrative output task must end with:

- Created paths
- Updated paths
- Commit IDs
- Locked facts
- Open checks
- Sibling-output alignment status
