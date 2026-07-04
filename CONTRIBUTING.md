# Contributing to the Chronicle

This repository is maintained as a campaign archive. Contributions should improve continuity, evidence quality, or usability during play.

## Product Owner

John Thomas Cleveland / FroBoyX is the final decision maker for canon, scope, tone, and archive priorities.

## Archivist Responsibilities

The archivist maintains:

- timeline integrity,
- character and NPC continuity,
- relationship tracking,
- source provenance,
- repository structure,
- open thread tracking,
- contradiction tracking,
- and documentation quality.

## Commit Style

Use conventional commits with gitmoji where practical.

Examples:

```text
docs(repo): 📝 establish Chronicle archive home
docs(canon): 📝 establish canon hierarchy
docs(chronology): 📝 seed timeline through Arodus 5
docs(wormwood): 📝 recover ship layout and crew state
docs(harvus): 📝 add recovered Book 1 campaign history
```

## File Style

Prefer Markdown.

Use clear headings, short paragraphs, and stable sections.

Do not bury important state in prose when a short labeled field is better.

## Entity Principle

One entity gets one canonical file.

Examples:

- one file for Harvus G'ron,
- one file for Sandara Quinn,
- one file for the Wormwood,
- one file for Bonewrack Isle.

Other documents link to entity files rather than duplicating full profiles.

## Evidence Handling

Raw material belongs in `evidence/`.

Canonical synthesis belongs in the relevant chronology, character, ship, location, faction, or world file.

Do not treat raw evidence and canon synthesis as the same thing.

## Intake Workflow

When new material is recovered:

1. Identify source type.
2. Place or summarize it in evidence tracking.
3. Extract objective events.
4. Extract relationship changes.
5. Extract open threads.
6. Update affected entity files.
7. Update chronology if the material changes the timeline.
8. Record contradictions if unresolved.

## Current Operating Mode

The repository is in **Archive Phase**.

Recovered material may arrive out of order. The archivist is responsible for placing it in the correct campaign context.

## Do Not

- Do not convert the campaign to 5e in this repository phase unless explicitly directed.
- Do not overwrite campaign truth with published adventure path defaults.
- Do not erase contradictions silently.
- Do not fictionalize missing material.
- Do not expand player-facing profiles with GM-only secrets unless the target document is explicitly GM-facing.
