# Bonewrack Island Source Spine — Arodus 1-4

## Document Status

- Type: GM-side source spine / evidence-control layer
- Maturity: Reconciled supporting control
- Parent issue: GitHub issue #2
- Scope: Erastus 31 storm context through the Arodus 4 branch endpoint immediately before the fork encounter
- Player-facing status: Not player-facing by default
- Canon status: Supporting source-control document. Sequence and dates are controlled by `chronology/bonewrack-arodus-1-to-4-memory-spine.md` and `chronology/bonewrack-arodus-4-date-lock.md`
- Authority index: `chronology/bonewrack-control-and-impact-index.md`
- Narrative status: Not polished narrative
- Historical-label rule: `Aeodus 5th`, `Arodus 5`, and `Arodus 5th, 4701` remain preserved source metadata only

## Purpose

This file records the source basis, evidence classes, quote ledger, knowledge boundaries, unresolved encounter-state checks, and sibling-output constraints for Bonewrack.

It does **not** independently reconstruct the day-by-day chronology. Use the controlling memory spine for event order and the date-lock file for calendar truth.

## Evidence Classification

| Label | Meaning | Promotion rule |
|---|---|---|
| `TABLE-DIRECT` | Recovered direct chat, action, roll, or mechanical fragment | May establish visible actions and exact recovered wording within the fragment |
| `TABLE-SUMMARY` | Sanitized extraction from a recovered session cache | Strong table evidence; do not invent omitted dialogue or mechanics |
| `GM-LOCK` | Explicit current GM truth or canon ruling | Controls unless later GM correction supersedes it |
| `GM-MEMORY` | GM memory without complete direct log | Preserve as memory or locked outcome with mechanics open where needed |
| `PLAYER-NARRATIVE` | Retrospective player-authored character account | Strong for relative sequence, perception, and character experience; corroborate before globalizing |
| `PLAYER-NOTE` | Contemporaneous or near-contemporaneous notes | Strong for relative sequence and that character's experience |
| `PLAYER-MEMORY` | Later discovery answer or recollection | Strong for interiority and remembered interpretation |
| `RECONSTRUCTION` | Archive synthesis in a book, chronology, dossier, or chronicle | Useful derived layer; retain source limits |
| `AP-SCAFFOLD` | Published geography, hazard, encounter, or pacing structure | Context only; cannot prove played events |
| `UNRESOLVED` | Evidence supports multiple results or omits the required detail | Do not silently choose |

## Source Index

### Direct and Extracted Table Evidence

| Source ID | Path | Type | Use |
|---|---|---|---|
| `STORM-FRAGMENT` | `evidence/chat-logs/mans-promise-erastus-31-storm-grindylow-fight-fragment.md` | `TABLE-DIRECT` | Harvus in rigging; Sho and Rak fight; Rak badly wounded; Mirei falls; Sho cushions the fall |
| `LANDING-SWARM-EXTRACT` | `evidence/chat-logs/mans-promise-arodus-1-landing-camp-swarms-sequence.md` | `TABLE-DIRECT` / extract | Landing, early frog encounter, first camp, hidden flask, later ghoul combat, swarm sequence, Harvus macro correction |
| `SESSION-7` | `evidence/raw-session-logs/mirei-player-cache/session-07-storm-bonewrack-duplicate-summary.md` | `TABLE-SUMMARY` | Storm aftermath, ship damage, Plugg/Mirei pressure, island assignment, hidden placement |
| `FINAL-A5` | `evidence/raw-session-logs/mirei-player-cache/final-session-arodus-5-duplicate-summary.md` | `TABLE-SUMMARY` with historical label | Arodus 4 rescue aftermath, Rak/Syl route, Sho/Kahina branch, endpoint |
| `FINAL-DATE-EXTRACT` | `evidence/chat-logs/arodus-5-final-session-date-and-time-extract.md` | `TABLE-DIRECT` extract | Preserves historical date labels and within-branch times; objective date superseded |

### GM Truth and Rulings

| Source ID | Path | Type | Use |
|---|---|---|---|
| `GM-STORM-ISLAND` | `evidence/gm-notes/mans-promise-erastus-30-arodus-1-storm-island-shortform.md` | `GM-LOCK` | Initial abductees, Arodus 1 grounding, water loss, repair pressure, first camp, later Goyle capture |
| `GM-REST` | `evidence/gm-notes/bonewrack-coconut-beach-rest-and-riptide-day-clarification.md` | `GM-LOCK` | Three-rest structure, Coconut Beach recovery, stockade/first assault same day |
| `GM-RETURN` | `evidence/gm-notes/bonewrack-return-and-rak-escort-source-clarification.md` | `GM-LOCK` / evidence routing | Village return scope and uneventful village-to-ship continuation |
| `DATE-LOCK` | `chronology/bonewrack-arodus-4-date-lock.md` | Canon ruling | Final branch date is Arodus 4, 4712 AR |

### Player Narratives and Notes

| Source ID | Path | Type | Use |
|---|---|---|---|
| `HARVUS-NOTES` | `evidence/player-notes/harvus-light-timeline.md` | `PLAYER-NOTE` | Relative island sequence and rescue details |
| `HARVUS-NARRATIVE` | `evidence/player-narratives/harvus-bonewrack-day-30-31-and-day-31-part-2.md` | `PLAYER-NARRATIVE` | First assault, burned-tree camp, successful rescue, aftermath, movement to fork |
| `SHO-NARRATIVE` | `evidence/player-narratives/sho-bonewrack-day-28-to-31.md` | `PLAYER-NARRATIVE` | Day 28-31 sequence, swarms, Coconut Beach, cave retreat, village beating |
| `RAK-NARRATIVE` | `evidence/player-narratives/rak-bonewrack-cave-return-and-scourge-report.md` | `PLAYER-NARRATIVE` | First assault, rescues, retreat route, camp, village return, edited Scourge report |
| `HARVUS-RECALL` | `evidence/player-memory/harvus-player-memory-recall.md` | `PLAYER-MEMORY` | Harvus interpretation of Rak, Mirei, Sandara, and rescue |
| `MIREI-RECALL` | `evidence/player-memory/mirei-player-discovery-notes.md` | `PLAYER-MEMORY` | Mirei interiority; remaining cave-support and hidden-flask questions |
| `RAK-RECALL` | `evidence/player-memory/rak-wraithraiser-player-discovery-answers.md` | `PLAYER-MEMORY` | Rak character intent, route knowledge, and item memories |

### Campaign Reconstruction and State

| Source ID | Path | Type | Use |
|---|---|---|---|
| `BONEWRACK-CONTROL` | `chronology/bonewrack-arodus-1-to-4-memory-spine.md` | Controlling chronology | Day-by-day objective sequence |
| `BONEWRACK-BOOK` | `book-1/bonewrack-isle.md` | `RECONSTRUCTION` | Location inventory and campaign consequences |
| `RIPTIDE-FALL` | `chronicles/the-fall-of-riptide-cove.md` | `RECONSTRUCTION` / `GM-MEMORY` | Existing rescue chronicle; requires Whale-sequence review |
| `SANDARA-RESCUE` | `chronicles/the-rescue-of-sandara.md` | `RECONSTRUCTION` / `GM-MEMORY` | Character-centered rescue account; not independent evidence |
| `BOOK-ONE-BRIDGE` | `chronology/book-one-late-wormwood-to-arodus-5-bridge.md` | Active bridge with legacy filename | Late Wormwood through Arodus 4 endpoint |
| `A5-TABLEAU` | `state/arodus-5-current-state-tableau.md` | Current state with legacy filename | Arodus 4 branch state and knowledge boundaries |
| `A5-SPLIT` | `chronology/arodus-5-split-scenes.md` | Within-day chronology with legacy filename | Arodus 4 branch times and endpoint |

### Adventure Path Scaffold

| Source ID | Path | Type | Use |
|---|---|---|---|
| `AP-BONEWRACK` | `evidence/ap/mans-promise-whispers-storm-and-bonewrack-summary.md` | `AP-SCAFFOLD` | Storm, reef pressure, published island geography, encounter context |

## Calendar and Sequence Control

The objective sequence is locked:

- **Erastus 31:** storm; Sandara and Tilly taken.
- **Arodus 1:** grounding, assignment, landing, broken bridge/frogs, first camp, hidden flask, undead attack.
- **Arodus 2:** swamp/swarms, burning site, Coconut Beach, injury-driven recovery.
- **Arodus 3:** stockade/spring/spyglass, first Riptide assault, retreat, burned-tree camp.
- **Arodus 4:** morning split, village beating, successful rescue, rescue aftermath, Rak/Syl and Sho/Kahina branches, movement toward the fork.

Do not restore the historical Arodus 5 label to active chronology.

## Source-Control Beat Crosswalk

| Beat | Objective chronology source | Primary supporting evidence | Remaining source caution |
|---|---|---|---|
| Storm and initial abductions | Memory spine §0 | Storm fragment, GM storm note | Exact order of all storm actions remains incomplete |
| Grounding and assignment | Memory spine §§1-2 | Session 7, GM notes | Exact Plugg whispered wording remains unrecovered |
| Landing / bridge / frogs | Memory spine §2 | Direct landing extract, Sho narrative | Map geometry can refine route but not date |
| First camp / hidden flask / undead | Memory spine §3 | Direct extract, Sho and Harvus | Hidden-flask intent remains Mirei-private |
| Swamp / swarms | Memory spine §4 | Direct extract, Sho, Harvus | Harvus macro is an input correction, not exact dying proof |
| Burning site / Coconut Beach | Memory spine §§5-6 | Sho, Rak, GM rest lock | Mirei-flask causation remains unresolved |
| Stockade / spring / spyglass | Memory spine §7 | Rak, Sho, Harvus, location reconstruction | First tricorne sighting remains uncertain |
| First Riptide assault | Memory spine §§8-9 | Rak, Sho, Harvus | Cave-current terminology and exact casualties remain open |
| Burned-tree camp / split | Memory spine §§10-11 | All three narratives | Split location and morning are resolved |
| Village return / beating | Memory spine §12 | Rak and Sho narratives, chat | Sho's post-blackout transition remains open |
| Goyle capture | Memory spine §13 | GM lock, Goyle report | Exact raw-log placement remains open |
| Successful return / rescue | Memory spine §§14-17 | Harvus narrative, final source | Whale timing, Queen visibility, and item state remain open |

## Character Knowledge Boundaries at the Arodus 4 Endpoint

| Character / branch | Knows | Does not yet know | Handling rule |
|---|---|---|---|
| Harvus rescue branch | Rescue events; Goyle accusation; Mirei confession; route toward fork | Rak/Syl route details; Sho/Kahina bargain; exact shipboard state | Keep testimony within rescue branch until contact |
| Mirei rescue branch | Her hidden task and flask; rescue support; confession | Sho's confinement details; Rak's current route | Hidden intent remains Mirei/GM knowledge except confession content |
| Rak supply branch | Village confrontation; Scourge order; route and escort events | Rescue outcome; Mirei confession; Sho/Kahina bargain | Do not import rescue-side facts |
| Sho ship branch | Village beating; her confinement; Kahina bargain | Rescue outcome; Rak's route; Goyle testimony | Do not import island-branch facts |
| Sandara | Her abduction and rescue, limited by consciousness | Most island travel and branch developments | Do not treat her as omniscient after rescue |
| Tilly | Her abduction, captivity, and witnessed rescue fragments | Most prior island travel and shipboard events | Preserve trauma and underwater uncertainty |
| Goyle | Later ship attack, Tidal Cutlass strike, captivity, rescue, Plugg accusation | Earlier island route unless told | Character timing reports are not exact timestamps |

## Quote Ledger

Recovered direct dialogue remains sparse. Do not invent island dialogue without explicit embellishment approval.

| Speaker | Exact recovered quote | Source | Use status |
|---|---|---|---|
| Sho | `Doing alright?` | `STORM-FRAGMENT` | Exact but storm-limited |
| Rak | `Didn't even break a sweat` | `STORM-FRAGMENT` | Exact but storm-limited |
| Mirei | `Thanks Sho` | `STORM-FRAGMENT` | Exact but storm-limited |

Player-authored narrative dialogue may be quoted as character-journal text, but it is not recovered table chat unless independently preserved.

## Locked Facts for Sibling Outputs

- Sandara and Tilly are initial storm abductees; Goyle is captured later.
- The Man's Promise grounds on Arodus 1, 4712 AR.
- Rak, Sho, Mirei, and Harvus are sent ashore.
- The frog encounter occurs before the first camp.
- The first camp includes Mirei's hidden flask and a three-undead attack.
- Swarms badly injure Sho and Harvus.
- The party burns the foul site and recovers at Coconut Beach.
- Stockade/spring and first Riptide assault occur on Arodus 3 without a separate stockade rest.
- All four PCs participate in the first assault.
- Rak rescues Sho and carries Harvus out.
- The party camps at the burned-tree landmark and splits there the following morning.
- Rak and Sho return to the village and are beaten by Scourge's order.
- Harvus and Mirei return to Riptide Cove and rescue Sandara, Tilly, and Goyle.
- Harvus kills the Whale with Rak's spear.
- The rescue group leaves the cove, avoids the cornfield, and approaches the fork.
- Final split-session branches occur on Arodus 4, 4712 AR.

## Open Checks for Map / Item / Player-Memory Passes

### Cave and Encounter State

- Resolve inflow / outflow terminology and entry / retreat routes.
- Place Sho's ambush, Rak's guard position, Harvus's collapse, Whale movement, and Queen route.
- Reconcile exact grindylow casualties.
- Reconcile Harvus's Whale-ascent sequence against older opening-exchange reconstruction.
- Determine who directly saw the Queen flee.

### Items

- Final state of Rak's returning spear.
- Final state of Harvus's flail.
- Sandara's tricorne and holy symbol at the endpoint.

### Mirei

- Hidden-flask intent.
- Frog spell identification.
- Exact first-retreat and Cauldron support actions.
- Queen visibility and Sandara consciousness during confession.

### Other Character Memory

Use only the narrowed questions in `questions/bonewrack-island-memory-batches.md`. Do not re-ask resolved route, participation, rescue, camp, split, or date questions.

## Sibling Output Alignment

| Output | Path | Status | Alignment notes |
|---|---|---|---|
| Ship's Log | Not assigned | Not started | Decide whether to use daily Arodus 1-4 entries or a compressed island log |
| Narrative Write-Up | Not assigned | Not started | May use locked day sequence; retain encounter-state uncertainty where relevant |
| Narrative Chat Scene | Not assigned | Not started | Requires recovered chat or explicit embellishment approval |

## Use Restrictions

- Do not turn this spine into polished narrative without a separate output request.
- Do not use AP geography to overwrite played events.
- Do not turn one character's perspective into global knowledge.
- Do not alter raw Arodus 5 or legacy-year source labels.
- Do not restage the fork encounter here.
- Do not resolve cave-map, item-state, or Queen-visibility questions by convenience.
- Do not cross-contaminate Arodus 4 branch knowledge before in-game contact.