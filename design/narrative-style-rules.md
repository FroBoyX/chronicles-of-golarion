# Narrative Style Rules

## Document Status

- Type: Design note / narrative style control
- Maturity: Working control document
- Scope: Narrative write-ups, narrative chat scenes, ship's logs, Discord-ready narrative posts, and player-facing chronicle prose
- Owner: GM / canon authority

## Purpose

This file defines style rules that apply when preserved evidence becomes readable prose.

These rules supplement `design/narrative-output-method.md`.

## Core Style Rules

### No em dashes

Do not use em dashes in narrative output.

Use commas, periods, colons, semicolons, parentheses, or sentence breaks instead.

This applies to:

- narrative write-ups,
- narrative chat scenes,
- ship's logs,
- Discord-ready versions,
- player-facing summaries,
- and newly drafted prose in evidence-derived outputs.

### No explainer paragraphs in narrative prose

Do not add paragraphs that explain to the reader why a scene matters, why a beat is important, what a relationship means, or how the player should feel about an event.

Do not use phrases like:

- "The scene matters because..."
- "This establishes..."
- "This becomes important because..."
- "The important thing is..."
- "This is why..."

Those belong in source spines, open checks, GM notes, or post-narrative analysis, not inside player-facing narrative prose.

Narrative prose can imply, foreshadow, and make reasonable leaps through action, consequence, placement, tone, and character behavior. It should not step outside the scene to interpret itself for the player or character owner.

### Embellish carefully

Use embellishment to bridge, stage, and render supported events, not to replace them.

Allowed embellishment:

- physical staging consistent with known ship geography,
- sensory texture consistent with the scene,
- small connective action needed to move between known beats,
- recurring visual habits already approved in support files,
- likely work-task texture when clearly marked in the source spine.

Avoid embellishment that:

- changes a character's motive without support,
- creates a new exact quote,
- changes the outcome or order of recovered events,
- makes hidden information visible to a character who would not know it,
- turns a table joke into literal canon without approval,
- overstates emotional certainty where player ownership matters.

If a beat is uncertain, keep it light, phrase it as action rather than conclusion, or leave it in the source spine rather than the narrative.

### Descriptions must not contradict or repeat

Descriptions must fit established canon, support files, and the current scene.

Do not repeat the same descriptive function multiple times in nearby paragraphs. Once a trait is established, use brief callbacks instead of re-describing it.

Example:

- First mention: establish Syl's stillness and hand near her knife.
- Later mentions: use a brief callback, such as "Syl's hand drifted toward the knife again."

Do not stack multiple descriptions that all say the same thing with different words.

### Use stable character names

Use a stable name for each character once the narrative has established them.

Do not repeatedly use full names unless the scene needs formal identification or there are two characters with the same short name.

Preferred pattern:

- First appearance in a scene or section: full name if useful.
- Later references: set name, surname, first name, title, or role, whichever is the established narrative standard for that character.

Examples:

- Slippery Syl Lonegan first, then Syl.
- Jaundiced Jape first, then Jape.
- Fipps Chumlett first, then Fipps.
- Aretta Bansion first, then Aretta.
- Harvus G'ron first, then Harvus.
- Rak Wraithraiser first, then Rak.
- Sho Astor first, then Sho.
- Mirei stays Mirei.

### No scene-name titles in player-facing narrative drafts

Do not break player-facing narrative drafts into named scene sections such as "Sho and Grok," "Bloody Hour," or "Night Below" unless the GM specifically asks for a structured packet.

For narrative refinement, prefer continuous prose with clean paragraph transitions.

Document metadata headings may remain at the top of repository files, but the narrative body should not read like an outline.

### Keep a consistent style and tone

Use a steady chronicle style:

- grounded,
- readable,
- restrained,
- sensory where useful,
- emotionally suggestive rather than interpretive,
- character-facing rather than author-explaining.

Avoid sudden shifts into florid prose, comedy, mechanics language, recap language, or omniscient moral judgment unless the source material or GM explicitly calls for it.

### Avoid comma-list description blocks

Do not describe characters or areas as a list of traits separated by commas.

Avoid sentences like:

```md
He was tall, thin, pale, angry, scarred, nervous, cruel, and tired.
```

Instead, choose one or two relevant traits and render them through posture, movement, action, or the current scene.

## Chat Quote Rules

### Chat-log actions are not character voice

When a chat-log message contains an action, gesture, emote, or stage direction, do not quote that action as spoken character dialogue.

Examples of action text include:

- `*winks*`
- `*chuckles*`
- `laughs`
- `nods`
- `shrugs`
- action text embedded before, after, or inside a spoken line

Rendering rule:

- Convert the action into narration.
- Quote only the spoken portion as dialogue.
- Do not make an action tag part of the character's voice.

Example:

```md
Sandara winked.

> "I told her it was cursed by the sea."
```

Do not render it as:

```md
> "*Winks* I told her it was cursed by the sea."
```

### Spell-check chat-log messages

Spell-check recovered chat-log messages when using them in player-facing prose.

Allowed corrections:

- obvious spelling errors,
- capitalization where needed for readability,
- punctuation needed for basic readability,
- apostrophes in ordinary contractions or possessives,
- minor typo repair that does not change meaning, cadence, or character voice.

Do not use spell-check as permission to rewrite a character's line into smoother prose.

If a line needs more than typo-level correction, either:

- paraphrase it outside quotation marks, or
- ask the GM to approve a cleaned canon-facing rendering.

## Workflow Preference

For difficult narrative days, refine in this order:

1. Non-chat-integrated narrative draft.
2. GM edit / review.
3. Integrated quote pass.
4. Final player-facing edit.
5. Discord-ready formatting.

Do not jump directly to Discord-ready chat integration while the prose shape, tone, or scene order is still unsettled.

### Version alignment rule

The most recent GM-edited narrative prose is the prose authority.

When creating a chat-integrated version, carry over the approved prose verbatim except where recovered dialogue is being inserted or a minimal transition is required to make inserted dialogue read cleanly.

When creating a Discord-ready version, preserve the approved narrative or chat-integrated prose verbatim. Discord formatting may split text into postable blocks, add minimal channel labels, or adjust markdown wrappers, but it must not summarize, tighten, rephrase, reorder, or improve the writing.

If a section contains no inserted chat, such as a concluding harp, weather, aftermath, or scene-setting passage, it should be duplicated exactly between the narrative, chat-integrated, and Discord-ready versions unless the GM explicitly requests a new edit.

If a Discord Formatter or downstream handoff receives prose that differs from the approved source, stop and ask which text is authoritative before formatting.

## Existing Rules Still Apply

- Recovered quotes are preserved by default except for spell-check / typo-level cleanup.
- Do not invent exact dialogue for missing chat.
- Do not put source-gap disclaimers inside narrative prose.
- If support is insufficient, drop the beat or ask the GM for permission to embellish.
