# Visual Output Method

## Document Status

- Type: Design note / visual output workflow
- Maturity: Working control document
- Scope: Character art, location art, battle maps, visual briefs, asset tracking, and reference handling
- Owner: GM / canon authority

## Purpose

This document defines how the archive turns established campaign facts, character dossiers, location notes, map notes, and visual references into consistent image-generation briefs and visual assets.

Visual output is parallel to narrative output. It should support play, player memory, and campaign relaunch without replacing evidence, canon, or tactical truth.

## Visual Output Streams

The visual workflow has three production streams:

1. **Character Art** — portraits, full-body references, crew portraits, expression/action variants, outfit/state variants.
2. **Location Art** — establishing shots, interiors, scene backdrops, ship spaces, island vistas, and environmental mood images.
3. **Battle Maps** — top-down tactical maps, player-safe maps, GM annotated variants, grid/no-grid variants.

A fourth control function, **Visual Canon / Art Direction**, maintains shared style, anchor assets, and the image-output index.

## Core Rule: Brief First

Before generating or requesting an image, create or identify a visual brief.

A visual brief is not the image prompt only. It is the controlled factual layer that records:

- subject identity;
- canon/source basis;
- visual anchors;
- required features;
- forbidden drift;
- style direction;
- intended output type;
- player-safe or GM-only scope;
- revision policy.

Recommended paths:

```text
visual-briefs/characters/<subject-slug>.md
visual-briefs/locations/<location-slug>.md
visual-briefs/maps/<map-slug>.md
```

Do not create major visual assets from vibes alone. Create the brief first, then the prompt.

## Reference Handling

Existing Pathfinder, Golarion, Skull & Shackles, or Paizo images may be used as setting and style references, but they should be handled carefully.

Rules:

- Use references for setting cues, costume language, material culture, tone, silhouette families, palette, and mood.
- Do not attempt to reproduce a specific official image one-to-one.
- Do not present a generated asset as official Paizo art.
- Do not store copyrighted reference image files in the repo unless the GM explicitly owns or has permission to archive them.
- Prefer recording reference notes, filenames, page/source hints, or descriptive cues in the visual brief.
- If the GM provides a reference image in chat, extract a visual brief from it and record how it was used.
- If an official image depicts a canon NPC or location, use it to preserve identity cues, not to directly copy the image.

Acceptable reference language:

- "Golarion / Skull & Shackles pirate fantasy tone."
- "Weathered Shackles crew clothing, salt-stained gear, practical shipboard grime."
- "Use official art as costume and mood reference, not as a direct copy."

Avoid reference language:

- "Copy this Paizo image exactly."
- "Same art, but extended."
- "Make a direct continuation of the official portrait."

## Visual Evidence Hierarchy

When visual sources conflict, use this order:

1. GM truth / current user confirmation.
2. Direct campaign evidence: chat logs, player sheets, Obsidian Portal, player notes.
3. Existing approved visual anchor for this archive.
4. Character/location/state dossiers.
5. Official setting/AP art as style or identity scaffold.
6. Published AP map or encounter geometry as map scaffold.
7. AI-generated drafts, only after GM approval.

Generated images are not canon by themselves. They become visual canon only after GM sign-off or explicit approval.

## Anchor Assets

Use anchor assets to maintain continuity.

### Character anchors

The first approved portrait or full-body image becomes the character's visual anchor.

Later variants should preserve:

- face and ancestry/species cues;
- body type and silhouette;
- key scars, markings, colors, or gear;
- outfit logic unless the variant is explicitly a costume/state change.

### Location anchors

The first approved establishing shot becomes the location's visual anchor.

Later location images should preserve:

- overall layout logic;
- major landmarks;
- material language;
- weather/lighting assumptions unless the variant changes them;
- relationship to known encounter/map geometry.

### Map anchors

The first approved tactical layout or map-truth brief becomes the map anchor.

Later beautified versions must not change:

- entrances/exits;
- encounter-relevant dimensions;
- line of sight;
- hazards;
- cover;
- terrain type;
- elevation/traversal rules.

## Minimum Visual Brief Fields

```md
# <Subject> Visual Brief

## Document Status

- Type: Character visual brief / Location visual brief / Battle-map brief
- Maturity: Draft / Working / Approved / Superseded
- Subject: <name or place>
- Asset type: Portrait / Full body / Establishing shot / Interior / Battle map / Variant
- Spoiler scope: Player-safe / GM-only / Character-limited
- Canon status: Working visual / Approved visual canon / Superseded

## Source Basis

- Canon/dossier files:
- Evidence files:
- Map notes/AP scaffold:
- GM corrections:
- Existing visual anchors:
- Reference notes:

## Required Visual Facts

- 

## Character / Location / Map Identity Cues

- 

## Style Direction

- 

## Output Requirements

- Orientation:
- Framing:
- Background:
- Grid/scale, if map:
- Variants needed:

## Avoid / Do Not Drift

- 

## Prompt Draft

```text
<prompt>
```

## Asset Index Links

- Tracking row:
- Generated asset paths or links:

## Open Checks

- 
```

## Character Art Workflow

1. Read the PC/NPC dossier and any player-safe discovery notes.
2. Create or update the character visual brief.
3. Identify required identity cues and unresolved visual conflicts.
4. Generate an anchor portrait first unless the GM explicitly requests full-body first.
5. Generate full-body only after the anchor portrait is accepted or the GM waives the anchor step.
6. Use approved anchors for crew portrait sets, outfit variants, injury-state variants, or action poses.
7. Update `tracking/image-output-index.md` after each approved or superseded asset.

Character art should prioritize recognizable identity over generic fantasy attractiveness.

## Location Art Workflow

1. Read the relevant location, ship, chronology, and encounter docs.
2. Create or update the location visual brief.
3. Identify shot type: establishing, approach, interior, object/feature, or scene backdrop.
4. Preserve spatial facts when known, but do not pretend scenic art is a tactical map.
5. Generate one anchor establishing shot before producing derivative views unless the GM requests a specific scene image first.
6. Update the asset index.

Location art should support memory and mood without overwriting map truth.

## Battle Map Workflow

Battle maps are truth-first.

1. Create or update the map-truth brief before any artistic prompt.
2. Record dimensions, entrances/exits, hazards, terrain, cover, elevation, lighting, and encounter-relevant objects.
3. Separate **player-safe** and **GM-only** variants.
4. Produce a readable tactical layout before producing a beautified version.
5. Do not let visual polish change tactical geometry.
6. Update the asset index and open checks.

Map outputs may include:

- player-safe grid;
- player-safe no-grid;
- GM annotated grid;
- GM annotated no-grid;
- printable or VTT export notes.

## Prompt Construction Rules

A final image prompt should include:

- subject and output type;
- source style direction;
- required visual facts;
- composition/framing;
- setting/material cues;
- exclusions only when they prevent known drift;
- spoiler scope where relevant.

Do not include unresolved facts as definite visual requirements.

## Patch / Remake Policy

If an approved or working visual asset already exists, do not remake it casually.

Use these change levels:

- **Patch prompt** — small correction or stronger required facts.
- **Variant** — new pose, outfit, expression, lighting, or crop using the same anchor.
- **Remake** — only when the GM asks, when the asset violates core canon, or when the style/identity is unusable.
- **Supersede** — mark the prior asset as superseded in the index instead of deleting its record.

## End-of-Task Report

Every visual-output task should end with:

- Created paths
- Updated paths
- Commit IDs, if repo files changed
- Brief used
- Asset IDs created or updated
- Locked visual facts
- Open visual checks
- Next recommended visual step
