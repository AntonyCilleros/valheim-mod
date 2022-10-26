
## Description

Adds new tiers of Weapons, Shields and Kits for the Do or Die SE Modpack (see below).
		
For further assistance you can find me on my Discord:- https://discord.gg/7BcEZXhRbV


## Special Thanx

	Jules for his helpful insight and help with JvL.
  Zarboz, Hugo the Dwarf, Balrond, Shadow84, GoldenJude, ASP and anyone else I have forgotten for their help with issues I posted in the various Valhiem Modding Discords.

## Credits

	VitByr for the Russian Translation.
	Cepepra for Russian Translation and Bug Fixing.
	
## Servers

Required on both server and client, uses JvL Network Compatibility.


## Incompatible Mods

- ValhiemLib and by extension any mod that still uses this defunct library.
- JotunnLib and by extension any mod that still uses this defunct library.

	
## Magic Overhaul Themed Additions

New class item for each class included for use with Magic Overhaul: Essence of *Class* 

**Wands (Shaman, Mage, Warlock)**

	Durability: 150 + 50 per level
	Durability Use: 2 STA
	Max Level: 10
	Knockback: 15/30
	Block Power: 15 + 5 per level
	Deflection Force: 30 + 5 per level
	Primary Attack:
		Type: Projectile
		Lifetime: 1s
		Velocity: 15
		Damage:	10 + 10 per level
		Cost: 12 STA
	Secondary Attack:
		Type: Projectile
		Lifetime: 3s
		Velocity: 30
		Cost: 33 STA
		Damage: 3x Primary
	Crafting Special Requirement: Class Item
	Additional Crafting Mats: Fine Wood, Bronze Bar, Infused Gemstone
	Sounds and VFX: Mostly Placeholders.
	
**Divine Mace (Paladin)**

	Durability: 200 + 50 per level
	Durability Use: 1 STA
	Max Level: 10
	Knockback: 25
	Block Power: 15 + 5 per level
	Deflection Force: 30 + 5 per level
	Primary Attack:
		Type: Default Mace
		Damage:	13 + 8 per level
		Bonus Damage: 3 + 4 per level vs Undead
		Cost: 10 STA
	Secondary Attack:
		Type: Default Mace Secondary
		Special: Static AoE
		Range: 6m
		Duration: 5s
		Interval: 1s
		Cost: 100 STA
		Damage: 3 + 5 per level
		Bonus Damage: 4 + 4 per level vs Undead
	Crafting Special Requirement: Class Item
	Additional Crafting Mats: Fine Wood, Bronze Bar, Infused Gemstone
	
**Assassin's Blade (Rogue)**

	Durability: 200 + 50 per level
	Durability Use: 1 STA
	Max Level: 10
	Knockback: 25
	Block Power: 15 + 5 per level
	Deflection Force: 30 + 5 per level
	Primary Attack:
		Type: Short Sword:
		Range: 2m
		Speed: 0.266 (Sword is  0.3)
		Damage:	13 + 8 per level
		Backstab: x4
		Cost: 10 STA
	Secondary Attack:
		Type: Jump
		Special: Caster Aura
		Range: 6m
		Duration: 5s
		Interval: 1s
		Cost: 100 STA
		Damage: 2 + 2 per level
		Special: Slows Enemies by 50% for 10s
	Crafting Special Requirement: Class Item
	Additional Crafting Mats: Fine Wood, Bronze Bar, Infused Gemstone
	
**Void Sword (Ninja)**

	Durability: 200 + 50 per level
	Durability Use: 1 STA
	Max Level: 10
	Knockback: 50
	Block Power: 12 + 12 per level
	Deflection Force: 30 + 5 per level
	Timed Block Bonus: 75%
	Primary Attack:
		Type: 2H Katana:
		Range: 2.7m
		Speed: 0.25 (Sword is  0.3)
		Damage:	18 + 11 per level
		Bonus Damage: 4 + 4 per level vs Undead
		Backstab: x3
		Cost: 15 STA
	Secondary Attack:
		Type: Jump Attack
		Damage: Landing Area
		Damage: 2x Primary
		Special: Static AoE
		Range: 6m
		Duration: 5s
		Interval: 1s
		Cost: 100 STA
		Damage: 8 + 5 per level
		Bonus Damage: 3 + 2 per level vs Undead
	Crafting Special Requirement: Class Item
	Additional Crafting Mats: Fine Wood, Bronze Bar, Infused Gemstone
	
**Striking Mace (Monk)**

	Durability: 200 + 50 per level
	Durability Use: 1 STA
	Max Level: 10
	Knockback: 60
	Block Power: 15 + 15 per level
	Deflection Force: 30 + 5 per level
	Timed Block Bonus: 25%
	Primary Attack:
		Type: 2H Mace:
		Range: 3m
		Speed: 0.2 (Sword is  0.3)
		Damage:	17 + 11 per level
		Backstab: x2.25
		Cost: 15 STA
	Secondary Attack:
		Type: Frontal Cone (120 degree)
		Damage: 4x Primary
		Knockback: 5x Primary
		Stagger: 3x Primary
		Range: 3m
		Duration: Instant
		Cost: 100 STA
	Crafting Special Requirement: Class Item
	Additional Crafting Mats: Fine Wood, Bronze Bar, Infused Gemstone
	
**Acid Spear (Druid)**

	Durability: 200 + 50 per level
	Durability Use: 1 STA
	Max Level: 10
	Knockback: 60
	Block Power: 12 + 8 per level
	Deflection Force: 30 + 5 per level
	Timed Block Bonus: 50%
	Primary Attack:
		Type: 2H Spear, single stab forward.
		Range: 3m
		Speed: 0.225 (Sword is  0.3)
		Damage:	17 + 11 per level
		Backstab: x2.25
		Cost: 17 STA
	Secondary Attack:
		Type: Spin
		Damage: 1.75x Primary
		Knockback: 6x Primary
		Stagger: 4x Primary
		Range: 3m
		Duration: Instant
		Cost: 100 STA
		Special: Healing AoE on completion of spin.
			Type: Static
			Healing: 5 + 1 per level
			Interval: 5s
			Duration: 60s
	Crafting Special Requirement: Class Item
	Additional Crafting Mats: Fine Wood, Bronze Bar, Infused Gemstone
	
**Raging Battleaxe (Berserker)**

	Durability: 200 + 50 per level
	Durability Use: 1 STA
	Max Level: 10
	Knockback: 70
	Block Power: 15 + 11 per level
	Deflection Force: 30 + 5 per level
	Timed Block Bonus: 75%
	Last Chain Multiplier: 125%
	Primary Attack:
		Type: 2H Spear, single stab forward.
		Range: 2.6m
		Speed: 0.15 (Sword is  0.3)
		Damage:	18 + 12 per level
		Backstab: x2
		Cost: 18 STA
	Secondary Attack:
		Type: Spin
		Speed: 0.2 (Sword is  0.3)
		Damage: 5x Primary
		Knockback: 3x Primary
		Stagger: 6x Primary
		Range: 3m
		Duration: Instant
		Cost: 150 STA
	Crafting Special Requirement: Class Item
	Additional Crafting Mats: Fine Wood, Bronze Bar, Infused Gemstone
	
**Chilling Axe (Deathknight)**

	Durability: 200 + 50 per level
	Durability Use: 1 STA
	Max Level: 10
	Knockback: 35
	Block Power: 15 + 5 per level
	Deflection Force: 30 + 5 per level
	Last Chain Multiplier: 150%
	Primary Attack:
		Type: 1H Battleaxe
		Range: 2.3m
		Speed: 0.2 (Sword is  0.3)
		Damage:	13 + 9 per level
		Backstab: x2.75
		Cost: 14 STA
	Secondary Attack:
		Type: Spin
		Speed: 0.3 (Sword is  0.3)
		Damage: 3.5x Primary
		Knockback: 4x Primary
		Stagger: 3x Primary
		Range: 3m
		Duration: Instant
		Cost: 75 STA
	Crafting Special Requirement: Class Item
	Additional Crafting Mats: Fine Wood, Bronze Bar, Infused Gemstone
				
	
## Resource Crates

**Armor Kits**

	Number of Tiers: 8 Starting with Bronze and ending with Flametal.
	Material 1: 30 Metal of relevant Tier
	Material 2: 5 Hide/Pelt
	Material 3: 5 Lower Tier Hide/Pelt
	Material 4: 10 Resin/Thread
	Weight: Weight of contents - 10%

- Used in Dod Buildables (New Anvils etc) and Items (Shields).
- Can be sold to the Trader for Coins.
- Can be Recycled for 75% of the materials back.
- Can be crafted, bought at the trader or found in chests.

**Weapon Kits**

	Number of Tiers: 8 Starting with Bronze and ending with Flametal.
	Material 1: 15 Metal of relevant Tier
	Material 2: 5 Hide/Pelt
	Material 3: 15 Wood
	Material 4: 10 Resin/Thread
	Weight: Weight of contents - 10%

- Used in Dod Buildables and Items. (Class Weapons)
- Can be sold to the Trader for Coins.
- Can be Recycled for 75% of the materials back.
- Can be crafted, bought at the trader or found in chests.


## Swords

	Max Level: 5 (4 Upgrades)
	Knockback: 30
	Damage: 120 (40 Slash + 3 per level, 80 Elemental + 8 per level)
	Block Power: 20 + 5 per level
	Deflection Force: 30 + 5 per level


## Prefab ID's

**Magic Overhaul Themed Weapons**

- ShamanWand_DoD
- MageWand_DoD
- WarlockWand_DoD
- PaladinMace_DoD
- RogueSword_DoD
- DeathknightAxe_DoD
- NinjaSword_DoD
- DruidSpear_DoD
- BerserkerAxe_DoD
- MonkMace_DoD
- DruidSpear_DoD
- SpartanSword_DoD
- PriestStaff_DoD

**Magic Overhaul Class Unlock Items**

- DeathKnightItem_DoD
- ArcherItem_DoD
- BerserkerItem_DoD
- DruidItem_DoD
- MageItem_DoD
- MonkItem_DoD
- NinjaItem_DoD
- PaladinItem_DoD
- RogueItem_DoD
- ShamanItem_DoD
- WarlockItem_DoD
- PriestItem_DoD
- SpartanItem_DoD
- EngineerItem_DoD

**Resource Crates**

- CrudeArmorKit_DoD
- BasicArmorKit_DoD
- GoodArmorKit_DoD
- GreatArmorKit_DoD
- SuperiorArmorKit_DoD
- ExcellentArmorKit_DoD
- ExceptionalArmorKit_DoD
- ExtraordinaryArmorKit_DoD
- CrudeWeaponKit_DoD
- BasicWeaponKit_DoD
- GoodWeaponKit_DoD
- GreatWeaponKit_DoD
- SuperiorWeaponKit_DoD
- ExcellentWeaponKit_DoD
- ExceptionalWeaponKit_DoD
- ExtraordinaryWeaponKit_DoD

**Shields**

- ShieldEikthyr_DoD
- ShieldRambore_DoD
- ShieldElder_DoD
- ShieldBitterstump_DoD
- ShieldBonemass_DoD
- ShieldSkullGreen_DoD
- ShieldModer_DoD
- ShieldFarkas_DoD
- ShieldSkir_DoD
- ShieldYagluth_DoD

**Shield Unlocks**

- BrokenShieldEikthyr_DoD
- BrokenShieldRambore_DoD
- BrokenShieldElder_DoD
- BrokenShieldBitterstump_DoD
- BrokenShieldBonemass_DoD
- BrokenShieldBhygshan_DoD
- BrokenShieldModer_DoD
- BrokenShieldFarkas_DoD
- BrokenShieldSkir_DoD
- BrokenShieldYagluth_DoD

**Magic Swords**

- SwordFlametal1_DoD
- SwordFlametal2_DoD
- SwordSpirit_DoD
- SwordFrometal1_DoD
- SwordFrometal2_DoD
- SwordFrometal3_DoD
- Stormblade_DoD
- SwordFelmetal1_DoD
- SwordFelmetal2_DoD

## Patch Notes

**0.1.12**

	Fixed Valhallium Ore and Bars getting mixed up.

**0.1.11**

	Added option for anvils to effect Thors Forge from EVA.

**0.1.10**

	Added Config for the single ores.

**0.1.9**

	For reals, config fix.

**0.1.8**

	Config fix.

**0.1.7**

	Minor Bugfix.

**0.1.6**

	Stagger/Block fix for Weapons.

**0.1.5**

	Bug fixing.

**0.1.4**

	Bug fix.

**0.1.3**

	Fix for Felmetal and Frometal Deposits causing NRE's.
	Fixed mocks that were pulling vanilla materials/sounds into the bundle.

**0.1.2**

	Added a check to see if the shields have already been added. 
	
**0.1.1**

- DoD Biomes dependancy removed.

**0.1.0**

- Added/Moved Ores and Metals from DoD Biomes.

**0.0.2**

- Added Priest Essence and Staff.
- Added Spartan Essence and Sword.

**0.0.1**

- Initial Upload