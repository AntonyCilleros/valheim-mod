---- All credit for htis mod goes to  Kyresel for the original mod and YperiteFairy for making the mod work with the H&H update. This is just uploaded to thunderstore for convenience installing it. ----


---------------------------------------------------------------
CombatOverhaul-HH patch - version 0.0.1.0 by YperiteFairy
https://www.nexusmods.com/valheim/mods/1786
---------------------------------------------------------------

Update 0.0.1.0

    Some (most? I don't know) functionality seems to work
    Mod definitely didn't crash while I tested it
    It definitely loads, as well. No more "it's not even in the BepInEx loaded plug-ins"

Issues:

    Going to negative stamina may or may not work
    Thunderheim compatibility is unknown as of yet



Release 0.0.0.1

    Hex-edited a broken reference

Issues:

    Didn't work﻿



Ok, so... long story short.

I really wanted to play the mod.
However, it's dead since the H&H update.
I've never played it before but it sounded great. The dreadful "stuck on load" issue felt like this is the end.
Welp, I disassembled both the game and the mod and tried to mess around a bit to make it work. I've no idea whether it works as it did before, but at least it doesn't get stuck on load anymore.

How to install:

!!! Don't forget to install BepInEx (see requirements) !!!

Thunderstone:
1. Go to settings
2. Import local mod
3. Choose the .dll

Manually:
1. Go to your Valheim folder
2. Open BepInEx/plugins
3. Drop the .dll there


Original mod: Valheim Combat Overhaul﻿ by leseryk.

I do not claim any rights to anything, the author's name is different just so you guys know leseryk didn't magically come back and fix his own mod.
I do not have the source code to be able to support the thing.
All I did was spend literally 10 minutes to modify someone's DLL in hopes of making it work.
No promises either, but if it works let me know. In theory this should work.
If you find weird bugs try sending me logs and I'll maybe try to fix it but I may not be able to.




Original README text
---------------------------------------------------------------
CombatOverhaul - https://valheim.thunderstore.io/package/Kyresel/CombatOverhaul/
---------------------------------------------------------------

## 1. Index

1. Index
2. Requirements
3. Mod Rationale
4. Recommended Mods
5. Features
6. To Do
7. Installation
8. Uninstallation
9. Also available on
10. Changelog


## 2. Requirements

- A non-pirated copy of Valheim updated to version 0.148.7 or higher
- BepInExPack Valheim version 5.4.9 or higher, available
    here: https://valheim.thunderstore.io/package/denikson/BepInExPack_Valheim/

	
## 3. Recommended Mods

While I haven't personally played with all of the mods listed below yet, I am sure they are compatible and should go
well with my changes:

- Terraheim by DasSauerkraut - https://www.nexusmods.com/valheim/mods/803
- Better Archery by Ishid4 - https://www.nexusmods.com/valheim/mods/348


## 4. Mod Rationale

The purpose of this mod is to balance various combat options provided to the player in Valheim without straying too far
from developers' original intent and vision of the game.
All of the changes are meant to remedy problems identified by me (or pointed out in discussions) while playing the game
as normal. Changes themselves are a result of well thought out (or so I would like to believe) decisions made after
extensive testing, research (inside and outside of the game), and comparisons of found key balancing factors between
available strategies.

TL;DR Why use tower shields if regular ones are objectively better - and why consider either in the first place, if bows
solve problems both faster and safer?
So these are the first two issues addressed by the mod.


## 5. Features

### 5. 1. General

- Allow for negative stamina values (by default capped at -50)
- Rotate character in the direction that player is aiming while wielding any weapon
- Allow character rotation (at reduced speed) during weapons' special attacks
- Lock character's movement/rotation during recovery frames of any melee attack
- Introduce new backstab damage bonus for all weapons (with old "backstab" mechanic renamed to "sneak attack")
- Introduce new counter damage bonus for all piercing damage (1.3x damage multiplier for piercing damage attacks on enemies in attack animation)
- Adjust critical damage (damage on staggered enemies) values for all weapons
- Adjust stagger damage multiplier values for all weapons
- Change stagger damage reset timer on enemies (3 sec -> 4 sec)
- Change existing armour formula to a new one, that preserves the most important aspects of the original, but also behaves better in "extreme" cases 

The first change that allows for negative stamina values provides players with an option to perform actions that require
certain amounts of stamina without meeting their stamina cost requirements - at the cost of longer time needed to wait
for stamina to recover afterwards, of course. The effect this has on general gameplay however is rather negligible, and
serves more as another tool in stamina management during combat rather than a nerf or a penalty. For example, if you
have ever found yourself in a situation where you were just a few points of stamina short to follow a parry with an
attack... That should happen significantly less often now.

Allowing for zero movement during any weapon's special attack felt like an odd design choice to me, severely limiting
those attacks' usability.
Locking character's movement/rotation during recovery frames of attacks provides a slightly better feel while using
certain weapons.
As for rotating the character with camera/mouse movement... With vanilla's restrictions on character's rotation during
attack animations or block arcs, it felt like a missing feature. While lack of it could be solved by e.g. blocking and
forcing the character to rotate in the direction the player's aiming, it felt awkward and resulted in having to fight
own character's movements rather than the environment's.

Changes to stagger damage values on weapons (described in more detail in 1.7.0 changelog) make combat less reliant on staggering enemies and make stunlocking enemies significantly more difficult. To make up for the overall lower stagger damage values (at least for most attacks), the timer after which enemy's "stagger bar" recovers has been increased. So while more hits are now needed to stagger an enemy on average, there is also more time available between attacks.

Newly introduced damage modifiers and changes to existing ones are meant to reward more tactical positioning in co-op and incentivize more varied playstyles depending on weapon type used. Damage on staggered enemies was reduced for most weapons. In general:

- Swords offer now higher than average critical and flanking bonuses in exchange for lowered stagger damage. With their secondary attack now also dealing piercing damage, they are more versatile against different enemy types.
- Sledgehammers remain for the most part unchanged, with their stagger damage slightly toned down.
- Battleaxes, on top of the changes listed in a section below, now offer stagger damage on their standard attacks.
- Atgeirs now have slightly less stagger damage on their regular attacks, and significantly less on their special attack, which no longer is almost guaranteed to stagger any enemy. However, they can now make use of the newly introduced counter damage bonuses, which synergizes well with their above average reach.
- Knives offer the highest damage bonuses out of all the weapons in the game, and are slightly easier to make use of the new backstab mechanic with.
- Axes and maces remain for the most part unchanged - expect for their critical damage bonuses reduced to the new base. They also offer now higher than average stagger damage multipliers on their attacks.
- Spears, similar to Atgeirs, can now make use of the counter damage bonuses. They also offer higher critical and flanking damage bonuses.
- Bows deal significantly less stagger damage now, but can now also benefit from the counter mechanic.

New armour formula shares some properties with the original, like e.g. needing armour rating equal to half the incoming damage to reduce it by 50%. But it doesn't reduce damage taken by 75% while the armour rating is exactly same as incoming damage, but by 66,(6)% instead. For damage equal to half the armour rating - that's 90% damage reduction, rather than around vanilla's 94,7%. And for damage quadruple the amount of armour... That's now 33,3% damage reduction, rather than just 25%.
In short: incoming damage values significantly below player's armour rating value are reduced less, and those significantly above - more. 
This change should both turn early game opponents into a slightly bigger threat, and adjust the difficulty for use with mods such as Creature Level and Loot Control - https://www.nexusmods.com/valheim/mods/495
The likelihood of surviving a 2-star or 5-star enemy hit is higher, and damage received from no-star or early game opponents slightly more threatening.


### 5. 2. Shields

- Lower stamina drain when blocking with a tower shield (40% less compared to regular shields)
- When blocking with a tower shield, surplus damage now reduces stamina rather than health, and no hit should stagger
    the player as long as stamina remains after blocking an attack
- Knockback force applied to the player on successfully blocking with a tower shield is now halved, unless the damage
    from a hit exceeds shield's effective block power.
- Remove enemy stagger and knockback on parrying projectile attacks
- Lower stamina regen while blocking (to 20% by default)

The differences between regular and tower shields within the base game serve only to effectively turn the latter into "
the worse of the two" at best.
The additional block power of tower shields simply does not make up for their movement speed penalty and inability to
parry, at least past the wooden tier of equipment. In the first place, though, there are simply not enough differences
to provide tower shields with their own unique identity within the game.

Through changes introduced by the mod tower shields trade their ability to parry for a unique mechanic of blocking
additional damage beyond their standard block power, at the cost of additional stamina. Additionally, there is lowered
stamina cost when blocking, as well as extra "stickiness" to the opponent on top of the already existing bonus to block
power. All of that at the cost of the significant -20% movement speed penalty from vanilla.
The end result is a new, more defensive playstyle available exclusively to tower shield users.

The change that allows the player's stamina to dip into negative values (from the "5. 1. General" section) is to prevent
the player from blocking bigger hits for significantly lower stamina costs when at low stamina. In worst case scenario,
when blocking a particularly strong hit while at low stamina, player may end up waiting for their stamina up to about 8
seconds (or up to 4 if the player has the Rested buff). Player is unable to perform any actions that require stamina
while it's negative.

This change also allows performing actions that require certain amounts of stamina without meeting their stamina cost
requirements - at the cost of longer time needed to wait for stamina to recover afterwards, of course. The overall this
has on general gameplay however is rather negligible, and serves more as another option in stamina management during
combat rather than a nerf or a penalty. For example, if you have ever found yourself in a situation where you were just
a few points of stamina short to follow a parry with an attack... That should happen significantly less often now.

Changes below are meant to further differentiate between the two types of shields and to slightly reduce the
effectiveness of the regular ones:

- Reduce regular shields' angle of protection to 120° (from 180°)
- Reduce tower shields' angle of protection to 150° (from 180°)
- Halve parry time window (250 ms -> 130 ms)

While a subjective matter, in my honest opinion a successful parry in Valheim is slightly too easy to achieve,
especially considering it's a reward with no risk attached to it. Compared to other games that offer the parry mechanic,
there are no startup frames before the parry nor recovery frames after it, where the player would be left vulnerable. In
vanilla, if you time your parry improperly, most of the time you will just end up blocking the hit instead of parrying
it. And I believe that's perfectly fine and in the spirit of Valheim, where the player is hardly ever penalized.
However, I believe that even after the change parrying still remains a perfectly viable tactic that's not too punishing,
but the reward is slightly harder to achieve. For me personally, that makes pulling off parries more satisfying than
before.


### 5. 3. Bows

- Player's movement speed is now reduced while drawing a bow (50% by default)
- Each level in bows skill now increases draw speed by 1%, rather than reducing draw time by the same amount
    (formula changed **from** BaseDrawTime * (1 - BowSkillFactor) **to** BaseDrawTime / (1 + BowSkillFactor *
    ConfigSkillFactorMultiplier))

There are three main issues I have found with bows in their previous state:

1. Gap closing times extending to infinity - simply backpedaling while shooting was often enough to avoid all damage
   from most melee opponents
2. Too high DPS at higher levels of the bow skill - damage you could deal with bows in a set span of time was comparable
   to that of melee weapons, even with wood arrows
3. Too high ratio of damage dealt to stamina spent - the main offender; you could deal more than tenfold the amount of
   damage you would with a melee weapon using the same amount of stamina

The first change is obviously meant to address the first issue. You can no longer avoid the enemy's attacks by simply
backpedaling while drawing a bow. You will now have to either dodge roll or time your shot with the enemy's attack to
knock them back during their animation. I believe that makes for a much more engaging gameplay.

On the upside, you may also draw your bow during the roll animation. While not intended by me and it's a peculiarity
that exists within the base version of the game, I believe it makes for an additional fun mechanic that might find use
after this particular change.

The second and third issues are a direct result of how the bows scale with their corresponding skill. In the case of
other weapons, each level in their respective skill increases their damage by 1% and lowers their attack stamina cost by
0.5%. Similarly, in the case of bows, their damage is increased by 1% per level. However, stamina cost remains the same,
and it's draw time that is reduced instead. Not by 0.5% per level, but 1%. Leveling the skill leads to 100% draw time
reduction at maximum.
This discrepancy leads to superior scaling of bows with their skill compared to that of other weapons. The draw time
reduction affects both the bow's ability to deal damage and the cost of shooting with one. And at 100% draw time
reduction, since you no longer need to spend time drawing the bow, there is also no stamina cost to speak of whatsoever.

By changing the formula used to calculate bow's draw time both issues are fixed.
In base version, each bows' skill level after the previous one is more of a damage increase (and stamina cost decrease),
with the difference between levels 99 and 100 being the most significant. After the change, this progression is linear
instead. Bows function similarly at lower levels to how they used to in vanilla. But once you get closer to level 100,
they are now more in line with other weapons.


### 5. 4. Battleaxes

- Adjust movement speed penalty from -20% to -10%
- Increase multiplier for turn speed during attack animation from 0.3 to 0.7 (turning during attack animation is now
    significantly easier)
- Chain 2nd and 3rd attacks for as long as you continue attacking

Battleaxes might be the weapon type that requires the most careful positioning, and might be the most difficult to use
properly overall. Reduction in its movement speed penalty to be on par with Atgeirs should help a skillful player in
this regard.
But even outside of game balance's viewpoint it didn't make much sense to me for a weapon that weighs as much as an
Atgeir and doesn't seem that much more unwieldy to slow down the player twice as much.

The new chain mechanic is to address the issue of weapon's surprisingly low DPS without removing its main drawback that
constitutes part of the weapon's uniqueness. And the increased turn speed both partially makes up for that same drawback
and turns continuous chaining of attacks into somewhat of a viable strategy in certain scenarios.
Jumping before the first attack for additional mobility, just like with hammers, might still be recommended - even if
somewhat silly.

Various other tweaks/new features were considered during development, including increased attack speed of the first
attack, introducing "super armor" mechanic that reduces stagger/knockback and possibly damage taken during first or
subsequent attacks animation, faster movement during animation, and so on.
In the end, we've decided that the changes implemented make it the most fun to use while retaining its unique aspects,
but feel free to offer your insights and further suggestions in the comments section.


### 5. 5. Sneak

- Scale sneak attack damage with player's sneak level - by default the sneak attack damage value is at half of vanilla's
    at 0th level, and same as vanilla at maximum
- Award sneak XP on performing a successful sneak attack, amount of XP dependant on weapon's backstab bonus and reduced
    for projectile attacks
- Display current backstab bonus when hovering over a weapon

Issues I've found with sneak in vanilla game:

1. Regular enemies (i. e. not wildlife) detect a sneaking player too effectively at lower skill levels
2. Since sneaking is leveled exclusively by moving while crouched and isn't an effective strategy early on, leveling it
     is more painful than it should be - through either grind or trying to sneak up on enemies knowing the futility of the
     effort
3. Despite the two points above, sneak archery playstyle is still highly rewarding at low risk and investment

In short, sneaking at lower levels feels futile, but sneaking's effectiveness scales rather well with level. So I've
decided to speed up the progression to enable the melee stealth playstyle earlier. The reduction to base value of sneak
attack damage is to balance out the additional reward granted on a successful sneak attack, but also to lower the
effectiveness of sneak archery at early stages of the game.

Modifying AI's detection formula and putting more emphasis on environmental conditions rather than sneak level was one
of the considered solutions, but I have opted not to alter vanilla's system fundamentally yet and playtest more before
deciding to make more drastic changes. However, it is highly probable such a change may appear in future updates.


## 6. To Do

Here follows a list of features planned for future updates of the mod:

- Various QoL features (allow auto-pickup of thrown weapons only by their owner etc.)
- Review weapons' block power and parry bonus values.
- Improve enemy AI.
- Take a look at hitbox verticality.
- Add color-coded visual feedback when stamina is drained on blocking with a tower shield.
- Grant increased rate of HP regeneration to enemies that are out of combat.


## 7. Installation

1. __Vortex Installation__
   This mod supports installation through Vortex.

2. __Manual Installation__
   Extract the downloaded archive in a temporary location.
   Then move the .dll file to your Valheim installation location BepInEx/plugins folder.


## 8. Uninstallation

1. __Vortex Uninstallation__
   If the mod has been installed using Vortex, you may also use Vortex to uninstall it.

2. __Manual Uninstallation__
   Remove files installed during manual installation.
   
## 9. Also Available On:
1. Nexus Mods - https://www.nexusmods.com/valheim/mods/591

## 10. Changelog
##### Version 1.7.8
  - Add a hit effect when the counter damage bonus is applied
  - Players no longer stagger enemies on timed blocks of their area attacks - Lox stomp, unarmed Troll smash attacks
  - Disable flanking bonuses on area attacks
  - Disable flanking bonuses for all weapons except knives by default - configurable
  - Revert critical damage changes - all weapons are now back to 2x critical damage bonus, with exception of swords and knives - which now have 2.2x and 3x bonuses, respectively
  - Revert the name change of backstab mechanic to maintain consistency in labelling between different mods
  - Some performance/compatibility improvements

##### Version 1.7.6
  - Fix issue with sneak attack XP not being correctly issued to the player when playing online
  - Full integration with Terraheim - CO's changes now apply to new weapons added in Terraheim
  - Terraheim's Silver Battleaxe's secondary attack now deals piercing damage
  - Terraheim's Blackmetal Axehammer's secondary now deals blunt damage
  - Terraheim's Blackmetal Axehammer's secondary no longer can damage trees

##### Version 1.7.5
  - Fix issue with enemies not getting harpooned

##### Version 1.7.4
  - This time positively fix the issue with thrown spears being duplicated. For real.

##### Version 1.7.3
  - Fix potential multiplayer issues
  - Fix issue with thrown spears being duplicated

##### Version 1.7.2
  - Fix new weapon stagger bonuses not being applied correctly
  - Fix sneak XP not being applied on sneak attacking with a bow
  - Apply counter damage bonus to hits with bows properly
  - Other bugfixes
  - Disable CO's movement speed penalty while drawing the bow if Terraheim is also installed

##### Version 1.7.1
  - Add config option for setting counter damage bonus
  - Lower default value of counter damage bonus to 1.2x
  - Fix a bug where not all of an appropriate secondary attack's damage would be converted to the expected type

##### Version 1.7.0
  - Reduce all weapons' critical damage multiplier (damage on staggered enemies) to 1.4x - unless specified otherwise below
  - Set all weapons' flanking damage multiplier to 1.5x - unless specified otherwise below
  - Introduce a new counter damage bonus (bonus on targets during their attack animation) for piercing damage type
  - Reduce sword's regular and special attack stagger damage multiplier from 1 to 0.7
  - Set sword's critical damage bonus to 2x
  - Set sword's flanking damage bonus to 1.5x
  - Set sword's special attack damage type to piercing
  - Reduce sledgehammer's regular attack stagger damage multiplier from 2 to 1.6
  - Increase battleaxe's regular attack stagger damage multiplier from 1 to 1.5
  - Reduce battleaxe's special attack stagger damage multiplier from 4 to 2
  - Reduce polearm's regular attack stagger damage multiplier from 1 to 0.8
  - Reduce polearm's special attack stagger damage multiplier from 6 to 1.4
  - Set knife's critical damage bonux to 3x
  - Set knife's flanking damage bonus to 2x
  - Set knife's "flanking arc" to 150°
  - Reduce axe's regular attack stagger damage multiplier from 1 to 0.8
  - Reduce mace's special attack stagger damage multiplier from 2 to 1
  - Reduce spear's regular attack stagger damage multiplier from 1 to 0.7
  - Set spear's critical damage bonus to 2x
  - Set spear's flanking damage bonus to 1.5x
  - Increase pickaxe's stagger damage multiplier from 1 to 1.6
  - Increase the time it takes for an enemy to reset their accumulated stagger damage from 3 to 4 sec
  - Introduce a new armour formula - Damage Taken = 0.5 * Input Damage ^ 2 / (Armour Rating + 0.5 * Input Damage)
  - Set damage type on sword's secondary attack to piercing
  - Set damage type on polearm's secondary attack to slashing
  - Set damage type on battleaxe's secondary attack to blunt
  
##### Version 1.3.2
  - Add a config setting for enabling/disabling character's rotation with camera
  - Add a config setting for battleaxe's movement speed modifier
  - Display various enable/disable config settings as checkboxes rather than true/false drop-down lists
  
##### Version 1.3.1
  - Fixed a bug where the character would keep facing the direction the player is aiming in while running
  
##### Version 1.3.0
  - Rotate character in the direction the player is aiming while wielding any weapon
  - Lock character's movement/rotation during recovery frames of any melee attack
  - Rotation speed during attacks with swords, maces and axes increased (0.3 -> 0.4)
  - Allow for rotation during special attacks with swords and maces (0 -> 0.3)
  - Allow for rotation during special attacks with battleaxes (0 -> 1)
  - Rotation speed during attacks with knives increased (1 -> 2)
  - Allow for rotation during special attacks with knives (0 -> 0.3)
  - Rotation speed during attacks with pickaxes increased (0.3 -> 0.4)
  - Rotation speed during special attacks with pickaxes increased (0.3 -> 0.4)
  - Allow for rotation during attacks with sledgehammers (0 -> 0.3)
  - Rotation speed during attacks with spears increased (0.2 -> 0.3)
  
##### Version 1.2.2
  - Fix how the calculated backstab value is displayed (limit to 2 decimal places)
  
##### Version 1.2.1
  - Fix issue with melee weapons' durability not deteriorating
  
##### Version 1.2.0
  - Lower movement speed penalty for battleaxes (-20% -> -10%)
  - Increase multiplier for turn speed during battleaxe's attack animation (0.3 -> 0.7)
  - Chain 2nd and 3rd battleaxe attacks for as long as player continues attacking
  
##### Version 1.1.0
  - Scale sneak attack damage with player's sneak level - by default the sneak attack damage value is at half of
      vanilla's at 0th level, and same as vanilla at maximum
  - Award sneak XP on performing a successful sneak attack, amount of XP dependant on weapon's backstab bonus and
      reduced for projectile attacks
  - Display current backstab bonus when hovering over a weapon
  - Reduce stamina regeneration while blocking (to 20% by default)
  
##### Version 1.0.5
  - Added configuration setting for toggling the negative stamina feature - recommended to leave it enabled, unless
      you are also using the Exhaustion mod
  
##### Version 1.0.4
  - Fixed BaseDrawSpeed affecting Fishing Rods
  
##### Version 1.0.3
  - Added option to disable staggering enemies on parrying their projectile attacks. This feature is enabled by
      default, but can be disabled in config
  - Fixed the default value for BaseDrawSpeed, which was accidentally set to 1
  
##### Version 1.0.2
  - Added configuration file which allows for enabling features and/or adjusting values
  
##### Version 1.0.1
  - Player's movement speed is now halved while drawing a bow
  - Each level in bows skill now increases draw speed by 1%, rather than reducing draw time by same amount
  - Knockback force applied to the player on successfully blocking with a tower shield is now halved, unless damage
      blocked is higher than player's block power
  
##### Version 1.0.0
  - Allow for negative stamina values
  - Halve parry time window (250 ms -> 130 ms)
  - Reduce regular shields' angle of protection to 120 degrees (from 180 degrees)
  - Reduce tower shields' angle of protection to 150 degrees (from 180 degrees)
  - Lower stamina drain when blocking with a tower shield (40% less compared to regular shields)
  - When blocking with a tower shield, surplus damage now reduces stamina rather than health, and no hit should
      stagger the player as long as stamina remains after blocking an attack
