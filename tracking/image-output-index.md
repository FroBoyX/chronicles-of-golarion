# Image Output Index

## Document Status

- Type: Visual asset tracking document
- Maturity: Working index
- Scope: Generated, commissioned, approved, rejected, and superseded visual assets

## Purpose

This file prevents visual output from drifting, being remade without need, or losing track of which prompt/brief produced which asset.

Every major visual asset should have a row here once it is drafted, approved, rejected, or superseded.

## Status Values

- **Planned** — desired but not briefed.
- **Briefed** — visual brief exists, no image yet.
- **Draft** — image or prompt draft exists, not approved.
- **Working anchor** — accepted enough to guide variants.
- **Approved visual canon** — GM-approved visual anchor.
- **Variant** — approved specific pose, outfit, state, lighting, crop, or map version.
- **Rejected** — do not use as anchor.
- **Superseded** — replaced by a newer asset, retained for history.

## Asset Index

| Asset ID | Stream | Subject | Asset Type | Brief Path | Asset Path / Link | Anchor Asset | Status | Spoiler Scope | Revision Policy | Notes |
|---|---|---|---|---|---|---|---|---|---|---|
| sho-hotbox-portrait-v1 | Character Art | Sho Astor | Portrait | visual-briefs/characters/sho-astor.md |  |  | Briefed | Player-safe if cropped/context-controlled | No remake without GM request | Suggested pilot; prompt drafted in visual brief. |
| harvus-post-riptide-portrait-v1 | Character Art | Harvus G'ron | Portrait | visual-briefs/characters/harvus-gron.md |  |  | Briefed | Player-safe after rescue reveal | No remake without GM request | Suggested pilot; prompt drafted in visual brief. |
| wormwood-exterior-v1 | Location Art | Wormwood | Establishing shot | visual-briefs/locations/wormwood.md |  |  | Briefed | Player-safe | No remake without GM request | Suggested pilot; prompt drafted in visual brief. |
| mans-promise-deck-map-v1 | Battle Map | Man's Promise deck | Battle map | visual-briefs/maps/mans-promise-deck.md |  |  | Briefed | GM-only until player-safe variant exists | No remake without GM request | Suggested pilot; truth-first prompt drafted; use recovered map notes and preferably original screenshot before final map generation. |

## Use Rules

- Add a row when a visual brief is created or a visual asset is requested.
- Do not delete superseded or rejected assets from the index; change status and note why.
- If a new image is a variant, link it to its anchor asset.
- If an image becomes the approved visual canon for a subject, mark it clearly.
- If an asset contains GM-only information, mark spoiler scope and create a separate player-safe variant if needed.

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
