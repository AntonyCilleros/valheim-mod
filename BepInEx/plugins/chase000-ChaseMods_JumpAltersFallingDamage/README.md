# Jump Alters Falling Damage

Jump skill alters the falling damage calculation by increasing the safe fall height and adding falling damage reduction.



# Installation

1. Install BepInEx.
2. Extract the mod into _Valheim_\BepInEx\plugins folder.
3. Start the game normally.
4. (optional) Configure the damage scaling to your liking using _Valheim_\BepInEx\config\ChaseMods.JumpAltersFallingDamage.cfg.



# Configuration

## MinUnskilledDamagingHeight

The fall height that starts to damage you at Jump skill level 0. Falling from a height lower than this value causes no damage.

Game default: 4

## MinSkilledDamagingHeight

The fall height that starts to damage you at Jump skill level 100. Falling from a height lower than this value causes no damage.

Game default: 4

## MaxDamagingHeight

The fall height that causes you maximum fall damage. Falling from a greater height causes no additional damage.

Game default: 16

## MaxFallDamageReduction

Fall damage reduction factor at Jump skill level 100.

Game default: 1 (no reduction)

## MaxFallDamage

Maximum allowed fall damage (before reduction).

Game default: 100



# Changelog

#### 1.1.1

- Calculation fixes (may result in a small increase in fall damage)
- Configuration sanity checks

#### 1.1.0
- MaxFallDamage
- Configuration option descriptions
- Changelog

#### 1.0.1
- Fixed manifest.

#### 1.0.0
- Initial version
