# PF2e Facing Variant

## Document Status

- Type: PF2e campaign subsystem conversion note
- Maturity: Draft / GM-originated homebrew candidate
- PF2e status: Conversion candidate, not approved relaunch mechanics
- Spoiler scope: Player-safe rules draft
- Created: 2026-07-07

## Purpose

This document preserves the GM's preferred tactical-facing rule for possible use in a PF2e relaunch of *Chronicles of Golarion*.

This is a homebrew tactical overlay. It does not rewrite PF1 historical evidence, prior rolls, prior outcomes, or campaign canon.

## GM Design Rationale

The GM added facing because omnidirectional threat and defense feel too abstract for weapon combat.

The design premise is:

- a combatant does not threaten or guard every direction equally;
- a combatant has an active guard / weapon line / attention arc;
- the space behind that guard is vulnerable unless the combatant turns or repositions;
- terrain matters, because putting one's back to a wall or obstruction can protect that rear vulnerability.

This is especially relevant for *Skull & Shackles* play because shipboard combat often involves decks, rails, masts, hatches, ladders, doorways, cramped interiors, caves, ambushes, boarding lines, and knife-range pressure.

## PF2e Source Basis Checked

Rules basis checked against Archives of Nethys PF2e pages on 2026-07-07:

- Off-Guard condition — Player Core pg. 445; off-guard imposes a -2 circumstance penalty to AC and can apply only against certain creatures or attacks.
- Flanking — Player Core pg. 425; flanking makes a creature off-guard to melee attacks from creatures flanking it, and depends on opposite positioning, ability to attack, and reach.
- Reactive Strike — Player Core pg. 138; trigger depends on a creature within reach taking specified actions or leaving a square during movement.
- Size, Space, and Reach — Player Core movement / encounter rules; establishes normal reach and space assumptions.

## Design Position

This variant should not redefine PF2e flanking.

Instead, it adds a new way to become **off-guard**:

> A creature is off-guard against melee attacks made from its rear arc.

This keeps PF2e's existing off-guard condition as the mechanical hook while avoiding a new flanking subsystem.

## Core Rule Draft

Each creature has a facing on the grid.

For a Small or Medium creature occupying one square:

- the **active arc** includes the three squares in front of the creature and the squares directly to its left and right;
- the **rear arc** includes the three squares behind the creature.

A creature can make melee Strikes, contribute to flanking, and use reach-based reactions only against creatures in its active arc.

A creature is **off-guard** against melee attacks made from its rear arc.

A creature may change its facing as part of:

- a move action;
- a Strike;
- a reaction, when the reaction involves movement or a melee Strike;
- choosing its facing at the end of its turn.

Turning in place without taking another action costs 1 action.

## Obstructions and Protected Rear Arc

A creature whose rear arc is blocked by a solid obstruction is not off-guard from that blocked direction.

Examples of solid obstructions include:

- wall;
- mast;
- bulkhead;
- cliff face;
- large crate;
- stacked cargo;
- closed door;
- ship rail or similar barrier, if the GM rules it substantially blocks approach or attack.

A creature can still be attacked from behind if the attacker has a legal line of effect and a way to attack past the obstruction, such as:

- reach;
- elevation;
- incorporeal movement;
- flight;
- a special ability that bypasses the obstruction;
- another GM-approved circumstance.

If only part of the rear arc is blocked, only the blocked squares are protected.

## Interaction With Flanking

Rear-arc off-guard is not automatically flanking.

A creature attacked from its rear arc is off-guard to that attack. However, effects that require the attacker to be flanking do not trigger unless the normal PF2e flanking requirements are also met.

This distinction is important for class features, feats, and abilities that care about flanking specifically.

## Interaction With Reactive Strike and Similar Reactions

For this variant, a reach-based reaction should require both:

- the triggering creature is within reach;
- the triggering creature is in the defender's active arc.

This prevents Reactive Strike and similar abilities from recreating omnidirectional threat unless a specific creature, feat, or ability is meant to do so.

## Creature Exceptions

Some creatures should ignore rear-arc off-guard or modify the facing rule.

Likely exceptions:

- all-around vision;
- amorphous bodies;
- swarms;
- oozes;
- creatures with no meaningful front or back;
- creatures with explicit supernatural awareness;
- huge or unusual body plans where facing should be adjudicated by the GM.

These exceptions should be recorded in the relevant creature or NPC conversion brief when they matter.

## Larger Creatures

The one-square version is the default pilot rule.

For Large or larger creatures, the GM should define active arc and rear arc from the creature's occupied footprint. Do not over-measure unless the scene requires it.

Open question: whether large creatures should use broad side arcs, distinct front/rear bands, or creature-specific facing diagrams.

## Foundry / VTT Notes

Foundry token rotation can likely represent facing visually.

Automation should not be assumed for the first pilot. Early use should be manual:

- rotate token to show facing;
- manually apply off-guard for rear-arc melee attacks;
- manually adjudicate active-arc limits for melee Strikes, flanking contribution, and reach-based reactions.

Later automation can be explored if PF2e conversion is adopted and the rule survives table testing.

## Balance Risks

Rear-arc off-guard makes off-guard more common.

Likely effects:

- positioning becomes more valuable;
- surrounding a creature becomes more dangerous;
- walls, corners, formations, rails, and chokepoints become more important;
- mobile melee characters gain more tactical reward;
- rogues and other precision / off-guard-dependent characters may gain reliability;
- poorly positioned creatures may be crit more often because PF2e's math makes a -2 AC penalty meaningful.

This is probably desirable for gritty shipboard combat but should be tested before campaign-wide adoption.

## Recommended Pilot

Test this variant in one contained PF2e scene before approving it:

- tight shipboard deck or below-deck fight;
- 4 PCs;
- 4-6 enemies;
- at least one reach-based reaction user;
- meaningful terrain such as rail, mast, hatch, doorway, wall, or stacked cargo;
- at least one opportunity for a creature to put its back to an obstruction.

Success criteria:

- facing creates interesting tactical choices;
- players understand the active arc quickly;
- off-guard from rear attacks feels fair rather than punitive;
- the rule does not slow play beyond acceptable limits;
- Foundry/manual adjudication is manageable.

## Open Questions

- Should choosing facing at the end of turn be free, or should facing only change as part of an action/reaction?
- Should Step, Stride, Fly, Swim, Climb, Leap, and Crawl all allow facing changes under the general "move action" clause?
- Should ranged attacks care about facing, or should the rule remain melee-only?
- Should shields interact with side arcs, or is that too much complexity?
- How should Large and larger creatures be diagrammed?
- Which PF2e creatures or traits should ignore the rear-arc rule by default?
- Can Foundry PF2e support this cleanly through token rotation plus manual off-guard, or does it need a macro/module for serious use?

## Status

Draft preserved for later PF2e conversion testing.

Not approved relaunch mechanics until GM confirms after pilot play.