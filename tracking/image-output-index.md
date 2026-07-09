# Image Output Index

## Document Status

- Type: Visual asset tracking document
- Maturity: Working index, updated with Sho no-AI-generation restriction
- Scope: Generated, commissioned, approved, rejected, and superseded visual assets

## Purpose

This file prevents visual output from drifting, being remade without need, or losing track of which prompt/brief produced which asset.

Every major visual asset should have a row here once it is drafted, approved, rejected, restricted, or superseded.

## Status Values

- **Planned** — desired but not briefed.
- **Briefed** — visual brief exists, no image yet.
- **Draft** — image or prompt draft exists, not approved.
- **Working anchor** — accepted enough to guide variants.
- **Approved visual canon** — GM-approved visual anchor.
- **Variant** — approved specific pose, outfit, state, lighting, crop, or map version.
- **No AI generation** — character/asset has a visual brief but AI image generation is not permitted.
- **Rejected** — do not use as anchor.
- **Superseded** — replaced by a newer asset, retained for history.

## Asset Index

| Asset ID | Stream | Subject | Asset Type | Brief Path | Asset Path / Link | Anchor Asset | Status | Spoiler Scope | Revision Policy | Notes |
|---|---|---|---|---|---|---|---|---|---|---|
| slippery-syl-portrait-v1 | Character Art | Slippery Syl Lonegan | Full-body portrait / NPC plate | visual-briefs/characters/slippery-syl-lonegan.md | art/characters/slippery-syl-portrait-v1.png |  | Working anchor | Player-safe as isolated portrait; GM-only when tied to current Bonewrack fork state | No remake without GM request; variants should preserve identity lock | GM-approved current style/identity lock; asset file imported by GM. |
| fipps-chumlett-portrait-v1 | Character Art | Fipps Chumlett | Full-body portrait / NPC plate | visual-briefs/characters/fipps-chumlett.md | art/characters/fipps-chumlett-portrait-v1.png |  | Approved visual canon | Player-safe as isolated portrait; GM-only if tied to Coconut Beach current-state scene | No remake without GM request; variants should preserve identity lock | GM approved with no notes; locked as Fipps visual anchor; use Syl only as house style baseline; asset file imported by GM. |
| rak-wraithraiser-portrait-v1 | Character Art | Rak Wraithraiser | Full-body PC character plate | visual-briefs/characters/rak-wraithraiser.md | art/characters/rak-wraithraiser-portrait-v1.png |  | Approved visual canon | Player-safe as isolated portrait | No remake without GM request; variants should preserve nagaji pirate-alchemist identity lock | GM approved final brown-scaled nagaji pirate-alchemist plate with smaller tail, visible alchemist gear, and spear in lowered pose; asset file imported by GM. |
| sho-hotbox-portrait-v1 | Character Art | Sho Astor | Portrait / commission reference | visual-briefs/characters/sho-astor.md |  |  | No AI generation | Player-safe if cropped/context-controlled | Do not route to AI generation; use only for human commission, manual art direction, or player-approved non-AI process | Sho player does not permit AI image generation; brief retained as visual direction only. |
| harvus-post-riptide-portrait-v1 | Character Art | Harvus G'ron | Portrait | visual-briefs/characters/harvus-gron.md |  |  | Briefed | Player-safe after rescue reveal | No remake without GM request | Suggested pilot; prompt drafted in visual brief. |
| wormwood-exterior-v1 | Location Art | Wormwood | Establishing shot | visual-briefs/locations/wormwood.md |  |  | Briefed | Player-safe | No remake without GM request | Suggested pilot; prompt drafted in visual brief. |
| mans-promise-deck-map-v1 | Battle Map | Man's Promise deck | Battle map | visual-briefs/maps/mans-promise-deck.md |  |  | Briefed | GM-only until player-safe variant exists | No remake without GM request | Suggested pilot; truth-first prompt drafted; use recovered map notes and preferably original screenshot before final map generation. |

## Use Rules

- Add a row when a visual brief is created or a visual asset is requested.
- Do not delete superseded, restricted, or rejected assets from the index; change status and note why.
- If a new image is a variant, link it to its anchor asset.
- If an image becomes the approved visual canon for a subject, mark it clearly.
- If an asset contains GM-only information, mark spoiler scope and create a separate player-safe variant if needed.
- If a player or GM blocks AI generation for a character, mark the asset **No AI generation** and keep the brief for commission/manual art direction only.

## Common Asset ID Pattern

```text
<subject-slug>-<asset-type>-v<number>
```

Examples:

```text
sho-hotbox-portrait-v1
sandara-crew-portrait-v1
wormwood-exterior-v1
riptide-cove-player-map-v1
riptide-cove-gm-map-v1
```

## Patch / Remake Notes

Use these revision labels in Notes when needed:

- Patch prompt only.
- Variant requested.
- Remake approved by GM.
- Superseded by asset ID.
- Rejected due to canon drift.
- Rejected due to style drift.
- No AI generation by player request.
