# PF2e Conversion Principles

## Document Status

- Type: PF2e conversion principle note
- Maturity: Working conversion policy
- Scope: System-first conversion posture and GM combat-design intent
- Spoiler scope: Player-safe process note
- Created: 2026-07-07

## Purpose

This document records a GM-level conversion principle for evaluating possible Pathfinder 2e relaunch mechanics for *Chronicles of Golarion*.

It applies across PC, NPC, encounter, item, ship, and campaign-subsystem conversion work.

This file does not rewrite PF1 historical evidence, prior rolls, prior outcomes, or campaign canon.

## Core Principle

Until the GM has a stronger working understanding of PF2e, do not casually edit PF2e's system assumptions.

Use PF2e-native rules first whenever possible.

However, the GM's combat-design intentions are not optional flavor. They are non-negotiable table-design goals that must be fitted into PF2e carefully rather than discarded.

## System-First Rule

For most old PF1 table rules:

1. Check whether PF2e already solves the same problem.
2. Prefer PF2e-native mechanics, feats, conditions, proficiency ranks, afflictions, encounter math, and Foundry-supported implementations.
3. Preserve the PF1 rule as table-history and design evidence when it mattered.
4. Avoid layering old PF1 subsystems on top of PF2e before the core PF2e engine is understood through play.
5. Defer or reject direct ports that would create unnecessary bookkeeping, duplicate PF2e systems, or destabilize PF2e math.

Examples currently treated this way:

- Skill Unlocks -> use PF2e skill proficiency and skill feats first.
- Diseases / Poisons -> use PF2e affliction rules and conversion templates.
- Stamina Pool / Combat Tricks -> defer until baseline PF2e, Facing, and Active Defense are tested.
- Wound Thresholds -> defer and use PF2e wounded/dying rules, visible injury narration, and encounter-specific bloodied behavior first.

## Non-Negotiable Combat Intent

The GM's combat edits were not arbitrary power changes. They came from a table preference for combat that better reflects weapon commitment, guard, line, pressure, and tactical survival.

The combat intent to preserve is:

- combatants should not defend and threaten every direction equally;
- facing, guard, attention, and footwork should matter;
- getting behind a defender should be tactically meaningful;
- putting one's back to a wall, mast, rail, bulkhead, or other obstruction should protect a vulnerable flank;
- prepared defenders should be visibly dangerous to attack;
- weaker or outmatched combatants should be able to survive by committing to defense;
- block, parry, and riposte should exist as tactical options where they fit the system;
- players and NPCs should be able to make meaningful tactical choices beyond trading attacks until someone drops.

These intentions should be adapted into PF2e rather than ignored.

Current combat-intent subsystem candidates:

- `conversions/pf2e/subsystems/facing-variant.md`
- `conversions/pf2e/subsystems/active-defense.md`

## Fit, Do Not Force

The standard for combat homebrew is not "copy the PF1 version."

The standard is:

> Preserve the GM's combat intent, then express it in PF2e's action economy, conditions, reactions, proficiency math, and Foundry implementation constraints.

If the direct PF1 version fights PF2e, rebuild the mechanic from the intent.

Examples:

- Facing should use active arc and rear-arc off-guard rather than PF1-style threatened-square assumptions.
- Active Defense should use actions, reactions, off-guard, Strike DC, and subordinate Strike logic rather than PF1 full-round actions, dodge bonuses, flat-footed AC, and BAB-based block checks.
- Stamina / Combat Tricks should not be ported unless PF2e martial play fails to preserve the desired battlefield flexibility after simpler systems are tested.
- Wound Thresholds should not be ported as quarter-HP global penalties unless PF2e injury and morale tools fail to create enough visible injury pressure.

## Conversion Review Questions

When reviewing any old table rule, ask:

1. Was this rule solving a problem PF2e already solves?
2. Was this rule a table-style preference or a non-negotiable GM intent?
3. Did any PC or NPC identity depend on this rule in actual play?
4. Does a PF2e-native rule, feat, condition, archetype, subsystem, or Foundry tool already cover it?
5. Would direct porting add bookkeeping or destabilize PF2e math?
6. Can the intent be rebuilt more cleanly through PF2e's action economy, reactions, conditions, or encounter procedures?
7. Should the rule be approved, piloted, deferred, or preserved only as historical evidence?

## Status

Working conversion principle.

This principle should guide later PF2e conversion audits until the GM revises it.