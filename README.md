# BattleTechGame-Rebalance-Mod

## Overview

This mod aims to make all weapons viable. It does this by buffing weaker weapons (smaller ACs, certain energy weapons), nerfing missiles and otherwise tweaking weapon values. In addition, Guarded was nerfed, the visual and radar range was increased, the morale system was tweaked, and hit chances are calculated slightly differently to make lights harder to hit and assaults easier.

## Requirements

You will need [ModTek](https://github.com/Mpstark/ModTek) and [BTML](https://github.com/Mpstark/BattleTechModLoader).

## Conflicts
This mod edits almost all weapon files, AC2 ammo and AC5 ammo, almost all mech chassis and CombatGameConstants.json. As such, installing this with other mods that edit these files can produce unwanted results.

## Installation

Download the .zip and simply extract the contents into your Mods folder.

## Main Features

- Large Lasers and PPCs less stupidly hot.
- AC2s and AC5s made more useful.
- LRMs and SRMs less powerful.
- LRMs no longer cluster.
- Guarded nerfed.
- Precision shot nerfed.
- Morale system more natural, can lose morale.
- Light mechs made easier to knock down, heavy mechs made harder to knock down.
- To hit modifiers... modified to make shooting at targets that should be easier to hit easier, and targets that should be harder to hit harder.

## Details

**IMPORTANT: +hit chance makes a target harder to hit, -hit chance makes a target easier to hit.**

### Abilities

Guarded nerfed - 50% to 33% damage reduction.

Precision shot now has +3 to hit instead of -4.

### Morale

Morale now has a max capacity of 100 instead of 50.

Morale abilities cost more numerically but less proportionally (both cost 30, increased from 20).

Initial morale is 10 instead of 5.

Morale is no longer gained at the start of each turn for no reason.

Morale is now additionally gained from:
- Causing critical damage (+1 morale).
- Causing ammo explosions (+1 morale).
- Causing weapon destruction (+1 morale).
- Dealing major armour damage (+1 morale).

Morale is now lost from:
- Ally ammo explosions (-1 morale).
- Ally weapon destruction (-1 morale).
- Taking critical damage (-1 morale).
- Taking major armour damage (-1 morale).
- Being knocked down (-5 morale).
- Being DFA'd (-5 morale).
- Ally being destroyed (-10 for lights and mediums, -15 for heavies, -20 for assaults).
- An ally being destroyed by melee causes an additional -5 morale.

### Mechs

Chassis stability is now calculated by the formula (50 + tonnage).

### Weapons

LRMs:
- Base damage reduced from 4 to 3.
- Stability damage reduced from 2 to 1.

SRMs:
- Base damage reduced from 8 to 6.

Small Laser:
- Base damage reduced from 20 to 15.

ER Small Laser:
- Base damage reduced from 20 to 15. 
- Heat reduced from 15 to 10.

Small Pulse Laser base damage reduced from 25 to 15. Heat reduced from 10 to 8. Now ignores 1 evasion pip.

Medium Laser base damage reduced from 25 to 20.

ER Medium Laser base damage reduced from 25 to 20. Heat reduced from 25 to 15.

Medium Pulse Laser base damage reduced from 25 to 20. Heat reduced from 20 to 12. Now ignores 1 evasion pip.

Large Laser heat reduced from 30 to 24.

ER Large Laser heat reduced from 45 to 36.

Large Pulse Laser base damage reduced from 45 to 40. Heat reduced from 40 to 30. Now ignores 1 evasion pip.

PPC heat reduced from 40 to 30.

ERPPC heat reduced from 50 to 40.

Machine Gun crit increased from 50% to 75%.

AC2s now deal 10 damage per shot and fire 3 shots at once, dealing 30 damage total. Shots roll for hit chance and hit location independently. +Dmg (5 and 10) attributes replaced with +Shots (1 and 2).

AC5s now deal 25 damage per shot and fire 2 shots at once, dealing 50 damage total. Shots roll for hit chance and hit location independently.

### Ammo

1 ton of AC2 ammo now contains 75 rounds instead of 25 (to compensate for the AC2 changes).

1 ton of AC5 ammo now contains 30 rounds instead of 15 (to compensate for the AC5 changes).

### Spotting, Hit Chance, Misc

Visual spotting distance increased from 300 to 450.

Radar spotting distance increased from 400 to 500.

Mechs can now shoot at targets a full 180 degrees in front of them.

Assault vehicles have a -1 hit chance modifier.

Light vehicles have a +1 hit chance modifier.

Now for every 20 units of elevation you have on a target, you have -1 hit chance.

Shooting at a target at medium range now gives +1 hit chance instead of 0.

Shooting at a target at long range now gives +3 hit chance instead of +4.

Shooting at an obstructed target now gives +4 hit chance instead of +2.

Indirect fire now gives +4 hit chance instead of +3.

Shooting at a knocked down target now gives -4 hit chance instead of 0.

Overheating gives +2 to hit chance instead of 0.

Walking gives +1 to hit chance instead of 0.

Distances required to gain the first 3 evasion pips decreased from 70, 100, 130 to 20, 80, 120 respectively. That means moving just 1 hex is sufficient for 1 pip of evasion.

Making a mech unsteady now removes Guarded.

Hitting a target with melee now removes Evasive.

Head hits are less common.

LRM clustering removed.