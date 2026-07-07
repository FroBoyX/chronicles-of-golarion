# PF2e Wound Thresholds Conversion Policy

## Document Status

- Type: PF2e campaign subsystem conversion note
- Maturity: Draft / deferred conversion policy
- PF2e status: Do not port directly; preserve as table-history and revisit only if baseline PF2e injury feels too binary
- Spoiler scope: Player-safe rules draft
- Created: 2026-07-07

## Purpose

This document preserves the table's Pathfinder 1e Wound Thresholds rule as conversion evidence and records the current PF2e conversion decision.

The rule should not be treated as approved PF2e relaunch mechanics. It should not be ported directly into early PF2e pilots.

This file does not rewrite PF1 historical evidence, prior rolls, prior outcomes, or campaign canon.

## PF1 Historical / Table Basis

The table had Wound Thresholds active from Pathfinder Unchained.

The PF1-era rule divided a character's maximum hit points into quarters and applied worsening penalties as the character dropped below thresholds:

- **Healthy:** above 3/4 maximum HP; no special modifier.
- **Grazed:** at or below 3/4 maximum HP but above 1/2; -1 penalty on attack rolls, saving throws, skill checks, ability checks, AC, and caster level.
- **Wounded / Injured:** at or below 1/2 maximum HP but above 1/4; -2 penalty on the same categories.
- **Critical:** at or below 1/4 maximum HP; -3 penalty on the same categories.
- **Disabled:** extended below 0 HP based on Constitution modifier for characters with Constitution 12+.
- **Staggered:** nonlethal-damage staggered range was extended based on Constitution bonus.

The design intent was to make injuries matter before knockout, increase the strategic value of healing, and avoid the feel that a badly injured creature fights at full capacity until it suddenly drops.

## PF2e Source Basis Checked

Rules basis checked against Archives of Nethys PF2e pages on 2026-07-07:

- Dying — Player Core pg. 411; a creature with dying is unconscious, dying has a value, and dying 4 means death.
- Unconscious — Player Core pg. 411; unconscious creatures cannot act, take a -4 status penalty to AC, Perception, and Reflex saves, are blinded and off-guard, and usually fall prone/drop held items.
- Wounded — Player Core pg. 411 / condition entry pg. 447; losing the dying condition gives or increases wounded, and wounded increases dying when the creature gains dying again.
- Doomed — Player Core pg. 411; doomed lowers the dying value at which the creature dies.
- Heroic Recovery — Player Core pg. 411; Hero Points can stabilize a dying character without adding or increasing wounded from that recovery.
- Recovery Checks — Player Core pg. 411; dying recovery uses flat checks modified by dying value.
- PF2e tight math / degrees of success — because bonuses and penalties can shift both hit/miss and critical thresholds, global HP-threshold penalties are much harsher in PF2e than they appear from a PF1 mindset.

## Design Position

Do not port PF1 Wound Thresholds directly.

PF2e already has a serious-injury loop:

- dropping to 0 HP causes dying and unconsciousness;
- recovery from dying creates or worsens wounded;
- wounded makes future knockdowns more dangerous;
- doomed can lower the death threshold;
- Hero Points interact with stabilization and wounded.

PF2e does not normally apply global penalties merely because a creature is below a fraction of maximum HP. Adding quarter-HP penalties would create a strong death spiral on top of PF2e's existing wounded/dying system.

## Why Direct Port Is Not Recommended

Risks:

- PF2e math is tighter than PF1; a -1, -2, or -3 penalty can strongly alter hit, miss, critical hit, save, and DC outcomes.
- The penalty applies to too many categories at once: attacks, AC, saves, skills, and spellcasting equivalents.
- Injured sides become increasingly less able to recover, creating a snowball that punishes the side already losing.
- Healing becomes mathematically mandatory to remove penalties rather than tactically useful.
- Bosses and large monsters become swingier or easier to collapse once damaged.
- Shipboard attrition, disease, poison, fatigue, Facing, and Active Defense already add pressure.
- Foundry automation would require custom threshold tracking or effects for every creature.
- NPC generator work becomes more complicated if every creature needs threshold breakpoints.

## Current Conversion Decision

Current recommendation:

- Preserve PF1 Wound Thresholds as table-history and design evidence.
- Do not port the quarter-HP penalty track into the first PF2e pilot.
- Use PF2e's native wounded, dying, unconscious, doomed, and healing rules first.
- Revisit only if PF2e combat still feels too binary after testing baseline PF2e, Facing Variant, Active Defense, and affliction templates.

## Preserved Design Intent

The old rule's core intent remains valuable:

- injury should be visible before knockout;
- healing should matter before someone drops;
- battered combatants should sometimes change tactics;
- PCs and NPCs should feel the difference between fresh, hurt, and near-collapse;
- attrition should matter in shipboard, island, and survival contexts.

Preserve that intent through narration and selective mechanics rather than universal penalties.

## PF2e-Native Alternatives

Prefer these before adding global wound thresholds:

### 1. Visible Injury States Without Mechanics

Use HP bands as narration only:

- above 3/4 HP: steady / fresh;
- 1/2 to 3/4 HP: bloodied, bruised, winded, grazed;
- 1/4 to 1/2 HP: visibly hurt, limping, breathing hard;
- 1/4 HP or less: reeling, desperate, bleeding, barely standing.

This gives the table the desired fiction without changing PF2e math.

### 2. Encounter-Specific Injury Effects

For certain monsters, hazards, duels, or major NPCs, define bespoke bloodied-state effects.

Examples:

- a wounded monster becomes more desperate or reckless;
- a ship officer loses command presence after being bloodied;
- a creature retreats, surrenders, or calls for aid at half HP;
- a supernatural enemy changes phase at half HP;
- a duel target gains or loses access to a tactical option when near collapse.

### 3. Serious Wounds Only After Dying

Use PF2e wounded/dying as written, then add narrative or downtime consequences only after a character drops, is treated, or survives a severe scene.

This keeps injury consequence tied to real near-death events rather than every HP loss.

### 4. Optional Wound Marks for Gritty Scenes

If needed later, create a smaller custom rule:

- no quarter-HP global penalties;
- no automatic attack/AC/save penalties;
- apply a wound mark only when a creature is critically hit, drops to 0 HP, takes massive environmental harm, or fails a specific hazard/save;
- wound marks affect recovery, shipboard labor, travel, or specific actions rather than every roll;
- remove through Treat Wounds, rest, magic, or scene resolution.

This is only a future fallback, not current relaunch mechanics.

## Relationship to Other Draft Subsystems

### Facing Variant

Facing already makes tactical injury and exposure more consequential through rear-arc off-guard and active-arc threat limits.

### Active Defense

Active Defense already lets hurt or outmatched characters survive by choosing a guarded posture.

### Affliction Templates

Diseases, poisons, fatigue, infection, and toxins already provide progressive condition pressure outside HP loss.

### Stamina / Combat Tricks

Stamina is deferred. Do not add wound thresholds plus stamina plus active defense without testing them separately.

## Recommended Pilot Position

Pilot order:

1. Baseline PF2e HP, dying, wounded, unconscious, healing, and Treat Wounds.
2. Facing Variant.
3. Active Defense.
4. Affliction templates for disease/poison/injury pressure.
5. Only then reassess whether Wound Thresholds are needed.

Success criteria for leaving Wound Thresholds aside:

- players can tell when foes are battered through narration and token state;
- healing matters tactically without mandatory quarter-HP penalties;
- dropping to 0 HP and becoming wounded feels dangerous enough;
- NPCs and monsters do not feel like perfect fighting machines at low HP because morale, tactics, and scene state change;
- Foundry tracking remains manageable.

## Open Questions

- Did the old table enjoy the wound penalties in practice, or did they mostly exist as a realism preference?
- Did Wound Thresholds affect major recovered scenes or outcomes?
- Were thresholds applied to monsters and NPCs consistently, or mostly to PCs?
- Would visible bloodied states satisfy the same need without mechanical penalties?
- Should major named NPCs have morale / bloodied behavior instead of penalties?
- Should critical hits or near-death events cause lingering wounds in downtime?
- Would a custom injury packet be better than universal HP-band penalties?
- Can Foundry track visible bloodied states without applying mechanical modifiers?

## Status

Draft conversion policy preserved.

Current recommendation: do not port PF1 Wound Thresholds into the first PF2e pilot. Use PF2e's native wounded/dying rules, visible injury narration, and encounter-specific bloodied behavior first.