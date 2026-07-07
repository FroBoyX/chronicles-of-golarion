# Evidence Ingestion Queue

## Document Status

- Type: Evidence tracking document
- Maturity: Working queue
- Scope: Raw or partially integrated evidence waiting for focused handling

## Use

Use this file when evidence has been mentioned, pasted, or identified but not fully preserved and integrated.

When a scene is completed, mark it as completed and list the evidence file plus any integration targets.

## Queue Format

```md
### Scene / Evidence Name

- Source type:
- Date candidate:
- Placement confidence:
- Destination evidence file:
- Integration targets:
- Status:
- Open checks:
```

## Active / Watch Items

### Harvus-side recent update and questions

- Source type: already preserved chat evidence / recent repo updates
- Date candidate: Wormwood storm and surrounding days; exact scene dates vary by file
- Placement confidence: varies by scene
- Destination evidence files:
  - `evidence/chat-logs/floating-before-erastus-13-harvus-rosie-fiddle-drink.md`
  - `evidence/chat-logs/wormwood-rosie-storm-rescue-messages.md`
  - `evidence/chat-logs/floating-erastus-14-15-harvus-sandara-rage-after-rosie.md`
- Integration targets:
  - `characters/pcs/harvus-gron.md`
  - `characters/npcs/rosie-cusswell.md`
  - `characters/npcs/sandara-quinn.md`
  - `relationships/harvus-rosie.md`
  - `relationships/harvus-sandara.md`
- Status: Preserved and integrated, but question follow-up may still need cleanup.
- Open checks:
  - Exact date placement for floating Harvus / Rosie / Sandara scenes.
  - Whether Harvus player packet needs a cleaned question set from these scenes.
  - How much of Harvus' rage / grief is player-safe for current cold open.

### Sho "monk man" / Ebony Saable

- Source type: GM identification plus Obsidian Portal source extract
- Date candidate: Man's Promise survivor / current hot-box context
- Placement confidence: identification high; relationship details unresolved
- Destination evidence file: `evidence/obsidian-portal/ebony-saable.md`
- Integration targets:
  - `characters/npcs/ebony-saable.md`
  - `state/current-npc-locations.md`
  - `state/crew-transfer-and-loyalty-audit.md`
- Status: Preserved and integrated.
- Open checks:
  - What exact Sho note or log called him the "monk man"?
  - What is Ebony's stance toward Sho and Kahina's test?
  - Is Ebony physically near Sho at cold open?

### Man's Promise named survivor physical positions

- Source type: GM truth / state reconstruction
- Date candidate: Current cold open, Arodus 5
- Placement confidence: survivor set fixed; physical positions unresolved
- Destination evidence file: existing survivor-set docs
- Integration targets:
  - `state/current-npc-locations.md`
  - `state/crew-transfer-and-loyalty-audit.md`
  - six survivor NPC dossiers
- Status: Pending.
- Open checks:
  - Dahrehn, Ebony, Merchiel, Nor'gal physical positions.
  - Who is guarding Sho?
  - Who supports Kahina's life-for-life test?

### Year consistency cleanup

- Source type: cross-repo cleanup
- Date candidate: global
- Placement confidence: current GM truth says 4712 opening year
- Destination evidence file: none
- Integration targets:
  - `chronology/current-state.md`
  - `state/current-npc-locations.md`
  - `state/current-ship-state.md`
  - `chronicles/the-fork.md`
  - any files still preserving 4691 incorrectly
- Status: Pending audit.
- Open checks:
  - Identify whether 4691 is still present as active chronology or only legacy text.
  - Correct only if it conflicts with the GM-locked 4712 timeline.

## Completed Recently

### Mirei Day 2 first recovered performance

- Evidence file: `evidence/chat-logs/wormwood-day-2-mirei-first-performance-badger.md`
- Integrated into:
  - `chronicles/wormwood-day-two.md`
  - `characters/pcs/mirei.md`
  - `characters/npcs/badger-medlar.md`
- Status: Completed.

### Rak and Grok Day 2 brew / bonding loop

- Evidence file: `evidence/chat-logs/wormwood-day-2-rak-grok-brew.md`
- Integrated into:
  - `relationships/rak-grok.md`
  - `characters/npcs/cut-throat-grok.md`
  - `chronicles/wormwood-day-two.md`
- Status: Completed.

## Intake Rule

Do not leave raw pasted logs only in chat. If a scene matters, create an evidence file first.
