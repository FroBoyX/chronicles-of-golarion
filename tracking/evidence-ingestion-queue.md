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

### Eight Wormwood-side Man's Promise survivors

- Source type: GM truth / survivor transfer correction
- Date candidate: Erastus 27 ship split and later Wormwood-side continuity
- Placement confidence: broad placement high; individual identities unresolved
- Destination evidence file: `evidence/gm-notes/mans-promise-survivor-set.md`
- Integration targets:
  - `state/current-npc-locations.md`
  - `state/crew-transfer-and-loyalty-audit.md`
  - `tracking/open-questions.md`
  - future Wormwood-side survivor notes if identities are recovered
- Status: Broad placement integrated; identities and later Wormwood-side duties pending.
- Open checks:
  - Who were the eight non-skeleton Man's Promise survivors?
  - What duties or status did they hold aboard the Wormwood after the Erastus 27 ship split?
  - Did any later re-enter the record or remain narratively untracked?

## Completed Recently

### Man's Promise Erastus 29-30 Mistress / Dinner / Syl Threat

- Evidence files:
  - `evidence/chat-logs/mans-promise-erastus-29-30-nightshift-mistress-and-dinner.md`
  - `evidence/chat-logs/mans-promise-erastus-30-nightshift-syl-mirei-threat.md`
  - `evidence/gm-notes/mistress-and-dinner-clarifications.md`
- Integrated into:
  - `chronicles/mans-promise-erastus-30-mistress-mirei.md`
  - `relationships/mirei-plugg.md`
  - `characters/npcs/slippery-syl-lonegan.md`
  - `characters/npcs/tam-narwhal-tate.md`
  - `characters/npcs/ebony-saable.md`
  - `characters/npcs/fipps-chumlett.md`
  - `characters/npcs/jaundiced-jape.md`
  - `characters/npcs/goyle-onorach.md`
- Status: Raw evidence already preserved; this pass verified integration and corrected Fipps' Ebony reference from likely to GM-confirmed.
- Open checks:
  - Whether Harvus attempted the Sandara-requested quarters investigation before the storm interrupted the night.
  - Whether Sho was ever involved in Sandara's backup "rough way" idea.
  - What Plugg and Scourge did with Syl's report about Mirei's handling of Tam and Sho.
  - Whether Syl's knife wound on Mirei left visible evidence or required treatment.
  - Whether Mirei ever ate the third plate Plugg said would wait.
  - Who was the second sailor with Tam when Mirei approached "you two."

### Active relaunch year cleanup

- Evidence source: GM correction preserved in `handoffs/chronicle-master-handoff.md`
- Integrated into:
  - `README.md`
  - `chronology/current-state.md`
  - `state/current-ship-state.md`
  - `chronicles/the-fork.md`
  - `tracking/open-questions.md`
- Status: Completed for active relaunch-facing files.
- Open checks:
  - Future searches may still find 4691 in handoffs or queue-history text; treat those as cleanup-history references unless they assert an active current date.

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