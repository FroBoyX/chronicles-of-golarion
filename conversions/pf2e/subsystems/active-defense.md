# PF2e Active Defense

## Document Status

- Type: PF2e campaign subsystem conversion note
- Maturity: Draft / GM-originated homebrew candidate
- PF2e status: Conversion candidate, not approved relaunch mechanics
- Spoiler scope: Player-safe rules draft
- Created: 2026-07-07

## Purpose

This document preserves the GM's preferred active-defense concept for possible use in a PF2e relaunch of *Chronicles of Golarion*.

This is a homebrew tactical overlay. It does not rewrite PF1 historical evidence, prior rolls, prior outcomes, or campaign canon.

## GM Design Rationale

The GM added Active Defense because omnidirectional passive AC does not fully capture weapon defense, guard, commitment, and the danger of attacking a prepared opponent.

The design intent is:

- allow tactical survival for both PCs and NPCs;
- let a weaker or outmatched combatant survive by committing to a guarded stance;
- make a prepared defender visibly dangerous rather than only passively harder to hit;
- preserve block, parry, and riposte play;
- make attackers think twice before engaging someone who is set, guarded, and ready to counter;
- connect naturally to the PF2e facing variant, where active defense protects the guard line but not the rear arc.

## PF1 Historical / Homebrew Basis

The GM's PF1-era Active Defense rule used:

- full-round action to enter Active Defense;
- +2 Dodge bonus to AC;
- no attacks of opportunity while on Active Defense;
- one block attempt per round by default;
- block check declared before the opponent's attack roll;
- block modifier based on BAB plus Strength or Dexterity plus size;
- block check against the opponent's attack roll;
- blocked attack damages weapon or shield as if sundered;
- failed block by 5 or more adds extra damage;
- beating the DC by 5 or more permits a counterattack against flat-footed AC.

These mechanics are historical design evidence only. They should not be ported one-for-one into PF2e.

## PF2e Source Basis Checked

Rules basis checked against Archives of Nethys PF2e pages on 2026-07-07:

- Actions and reactions — Player Core encounter rules; creatures normally get 3 actions and 1 reaction each turn.
- Degrees of Success — Player Core; critical success and critical failure normally occur at 10 above or below the DC.
- Off-Guard condition — Player Core pg. 445; off-guard imposes a -2 circumstance penalty to AC and can apply only against certain creatures or attacks.
- Raise a Shield — Player Core basic action; using a shield defensively is normally a 1-action commitment.
- Shield Block — Player Core general feat / reaction; reduces damage using shield Hardness and can damage both shield and bearer.
- Parry weapon trait — Player Core equipment trait; supports a defensive weapon posture through a circumstance bonus to AC.
- Reactive Strike — Player Core fighter reaction; establishes PF2e's non-universal opportunity-attack model.
- Subordinate actions — Player Core action rules; if an action/activity includes a subordinate action, the cost is included in the containing action/activity.

## Design Position

This variant should not replace PF2e's shield, parry, or reaction economy.

Instead, it adds a universal guarded posture that:

- costs actions to enter;
- grants a small AC benefit;
- grants a limited defensive reaction;
- allows a riposte when the defender either cleanly blocks or the attacker badly overcommits;
- does not protect the rear arc;
- does not preserve omnidirectional threat.

## Core Rule Draft

### Active Defense [two-actions]

You settle into a guarded stance, narrowing your attention to survival, weapon line, and counterattack.

**Requirements:** You are wielding a melee weapon, wielding a shield, or have at least one free hand suitable for an unarmed guard.

**Effect:** Until the start of your next turn:

- You gain a +1 circumstance bonus to AC against melee attacks from creatures in your active arc.
- You can use the Guarded Block reaction.
- You can use the Riposte reaction if its trigger occurs.
- You cannot use Reactive Strike or other offensive reactions except Riposte.
- Active Defense does not protect your rear arc.

## Guarded Block

### Guarded Block [reaction]

**Trigger:** A creature in your active arc hits you with a non-critical melee Strike.

**Requirement:** You are in Active Defense and are wielding a melee weapon, wielding a shield, or have a free hand suitable for an unarmed guard.

**Effect:** Attempt a block check against the attacker's Strike DC.

Your block check uses one of the following, chosen when you enter Active Defense:

- melee weapon attack modifier, if blocking or parrying with a weapon;
- shield attack modifier or Athletics modifier, if blocking with a shield;
- unarmed attack modifier or Athletics modifier, if blocking with an open hand / body guard.

**Critical Success:** You block or parry the attack cleanly. The triggering Strike deals no damage. You may change facing or Step 5 feet. You may also make a riposte Strike against the triggering creature as part of this reaction. The triggering creature is off-guard against this Strike.

**Success:** You turn the attack into a glancing blow. Reduce the damage by your level plus the Strength or Dexterity modifier used for the block check. If using a shield, you may use normal Shield Block rules instead if they would be better.

**Failure:** The attack resolves normally.

**Critical Failure:** The attack resolves normally, and you are off-guard against the triggering attack.

## Riposte

### Riposte [reaction]

**Trigger:** While you are in Active Defense, a creature in your active arc critically fails a melee Strike against you.

**Effect:** You make a melee Strike against the triggering creature. The triggering creature is off-guard against this Strike.

This Strike counts toward your multiple attack penalty, but your multiple attack penalty does not increase until after the Riposte resolves.

## Double-Reaction Clarification

A clean Guarded Block does not require a second reaction to riposte.

If Guarded Block critically succeeds, the riposte Strike is a subordinate Strike included inside the Guarded Block reaction.

Riposte as a separate reaction exists for a different trigger: when an attacker in the defender's active arc critically fails a melee Strike against the defender while the defender is in Active Defense.

Do not spend both Guarded Block and Riposte on the same triggering attack unless a later approved rule explicitly allows it.

## Interaction With Facing Variant

Active Defense assumes the PF2e Facing Variant may be in use.

If using facing:

- Active Defense protects only the defender's active arc;
- Active Defense does not protect the rear arc;
- Guarded Block and Riposte can only be used against creatures in the defender's active arc;
- attackers can defeat Active Defense by flanking, forcing movement, repositioning the defender, or attacking from behind;
- putting one's back to a wall, mast, bulkhead, or other obstruction can make Active Defense much stronger by protecting the rear arc.

If not using facing, the GM must decide whether Active Defense applies against all adjacent melee attacks or only against a declared guarded side / chosen target.

## Interaction With Shields and Parry

This subsystem should not make shields irrelevant.

Open balance position:

- A shield user may use normal Shield Block if it is better than Guarded Block's success effect.
- The +1 circumstance bonus from Active Defense should not stack with another circumstance bonus to AC from Raise a Shield, Parry, cover, or similar sources unless the GM explicitly approves.
- Shield users may still have stronger protection through official PF2e shield mechanics.
- Weapon parry users may use their weapon attack modifier for Guarded Block, preserving parry/riposte identity.

## Interaction With Critical Hits

The draft trigger only allows Guarded Block against a non-critical melee Strike.

This preserves the PF1-era intent that a critical hit cannot simply be blocked away by the basic Active Defense reaction.

Open question: whether a later feat, class feature, shield, weapon trait, or heroic option should allow a critical hit to be reduced to a normal hit or otherwise partially blocked.

## Balance Risks

Likely effects:

- attacking a prepared defender becomes riskier;
- weaker NPCs and PCs gain a way to survive briefly against stronger melee attackers;
- characters who give up offense for defense gain meaningful counter-threat;
- shipboard chokepoints, doorways, hatches, rails, and walls become more tactically important;
- fights may slow down if block checks are too frequent;
- riposte can increase damage output if triggers are too generous;
- +1 AC is small but meaningful in PF2e because it can change both hit and critical-hit thresholds.

## Recommended Pilot

Do not approve Active Defense as campaign-wide relaunch mechanics until after testing the simpler PF2e conversion assumptions.

Suggested pilot order:

1. Test baseline PF2e combat.
2. Test PF2e Facing Variant.
3. Add Active Defense to one contained scene with mixed PCs and NPCs.

Recommended test scene:

- tight shipboard or below-deck fight;
- 4 PCs;
- 4-6 NPCs;
- at least one outmatched defender using Active Defense;
- at least one aggressive attacker choosing whether to engage or reposition;
- meaningful terrain such as walls, mast, hatch, rail, table, crates, or doorway.

Success criteria:

- prepared defenders feel dangerous but not unhittable;
- block and riposte preserve the intended martial feel;
- players understand when a riposte costs a separate reaction and when it is part of Guarded Block;
- NPCs can use the rule without overcomplicating the GM's turn load;
- the rule does not overshadow official shield, parry, or class features.

## Open Questions

- Should Active Defense be two actions, or should there be a three-action stronger version?
- Should the +1 AC be limited to melee attacks only, as drafted, or also apply to thrown/ranged attacks from the active arc?
- Should Guarded Block use a weapon attack modifier, Athletics, Reflex, or a fixed class/level DC?
- Should unarmed/open-hand guards be available to all characters or require martial/unarmed proficiency?
- Should a shield user always be allowed to choose Shield Block after seeing Guarded Block's result, or must the choice be made before rolling?
- Should a critical success on Guarded Block allow both Step and riposte, or should the defender choose one?
- Should the riposte Strike apply MAP normally, or should the drafted MAP delay be removed for balance?
- Should certain classes, feats, monsters, or NPC roles receive improved Active Defense options?
- Can Foundry PF2e support Active Defense through temporary effects and manual reactions, or does it need a macro/module?

## Status

Draft preserved for later PF2e conversion testing.

Not approved relaunch mechanics until GM confirms after pilot play.