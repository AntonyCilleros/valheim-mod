# WolfPack

## Control all your tame wolves at the same time!

### Now with Strict Obedience!

You've tamed them, fed them, bred them and love them. They love you too, but they're always looking for attention and getting in the way. And you have to pet each of them to get them to do what you want. 

What you need is a little obedience training. With WolfPack, one keystroke will get all your tame wolves (or other creatures) to follow or stay at the same time. 

## What's new

### 0.9.8

- Added configuration for strict obedience. Now when you say "Stay", they really _stay_. In one place.
- More flexible configuration for custom creatures
- Synchronize 'following' creatures with new players on load (multiplayer)

## Features

- Multiplayer 3D audio for pack calls
- Multiplayer support on local and dedicated servers
- In-game reconfiguration
- Supports all tame creatures including those from PopVillages, DoD, and other mods
- Configure a list of creatures to call by name, (e.g., Wolf, Boar, Lox)
- Configure groups of creatures to call with wildcards (e.g., Human*, \*Spider*, *)
- Configure a single key Follow/Stay toggle, or separate Follow & Stay keys
- Cycle through creatures to call using keyboard or mouse wheel
- Filter creatures to call by number of "stars"

## Configuration

### General

- **DetectionRange**: The maximum distance from a player that creatures will be affected by a Follow or Stay command. Default value is 50. Can be set from 1 to 150.

- **TrainableCreatures**: a comma delimited list of creature names that will respond to Follow and Stay. Only tamed creatures will be affected. Default value is "wolf". **NOTE**: Values can be a creature, display, or prefab name. (see _LogCreatureNames_ below)

    - Example 1: [ wolf,boar,lox ] Calls either wolves, boars, or loxes (loxen?), depending on which was the current selection (see _CharacterSelectionKey_ below). 
    
    - Example 2: [ Human*,\*dwarf,\*spider* ] You can add an asterisk (*) as the _first and/or last_ character in a partial creature name to include all creatures who's name begins with, ends with or contains the partial text.
		- Human*: calls all creatures whose name begins with "Human", e.g., Human Commoners and Human Guards, etc. 
		- \*dwarf: calls all creatures who's name ends with "dwarf", e.g. Dwarf, Greydwarf, etc.
		- \*spider*: calls all creatures who have "spider" somewhere in their name, e.g., Spider, Tree Spider, Jumping Spider, etc.
       
    - Example 3: [ * ] Calls all tamed creatures.
	

- **PackBehaviorShortcut**: The keystroke to toggle between Follow and Stay for the currently selected creature. If you set _UseTwoKeys_ to True (see below), this key will only issue the Follow command. Default is LeftAlt+T

- **UseTwoKeys**: If set to True will use a separate keystroke for the Stay command as configured in _AlternateStayShortcut_ (see below). Default is False

- **AlternateStayShortcut**: The keystroke to call creatures to Stay. Only used if _UseTwoKeys_ (above) is set to True. Default is LeftAlt+Y

- **CreatureSelectorShortcut**: The keystroke to rotate through the list of _TrainableCreatures_ (above). Pressing this key repeatedly will cycle through the configured list. If _UseMouseWheel_ (see below) is set to True, holding this key down while spinning the mouse wheel will cycle through the configured list. The current selected creature will appear in the message area in the center of the screen (or top left under the hot bar as configured by _Notifications_ below). Default is LeftAlt+U

- **MinimumCreatureLevel**: The \'lowest' level of creature (in \'stars') affected by Follow and Stay. Default is 0. Can be set from 0 to 2. Affects all creatures.

- **UseMouseWheel**: If set to True, the mouse wheel is used to cycle through the _TrainableCreatures_ list to set the current creature. Hold down the _CreatureSelectorShortcut_ key while spinning the mouse wheel. If you don't have a mouse with a wheel or use another input device that makes this difficult, set to False. Default is True

- **Notifications**: The location of the creature selector message. Default is "Center" in the middle of the screen.  You can also set this value to TopLeft under the hot bar, however the center text has a much quicker response.

- **StrictObedience**: Sets the amount of 'wandering' when creatures are 'stayed'. If set to 0, creatures will obediently remain in one place. Default is 10. Can be set from 0 to 30. Affects all creatures.

### Audio

- **UseSound**: If set to True, will use the sound configured in _PackCallSound_ (below) whenever creatures are called to follow.

- **PackCallSound**: The audio clip played when creatures are called to Follow. Default is Whistle.wav. WolfPack is distributed with three audio clips; Whistle.wav, Horn1.wav, and Horn2.wav.

    - Whistle is a sharp finger whistle, Horn1 is a traditional hunting horn, and Horn2 is a deeper battle horn. These clips are located in the same folder as WolfPack.dll (...\BepInEx\plugins\Neobotics-WolfPack)
    
    - **NOTE**: You can put your own audio clips in this folder, and set _PackCallSound_ to your file name. Be advised, however, this is 'at your own risk'. WolfPack has only been tested with the three included files, which are 16-bit uncompressed PCM .wav files sampled at 44100. WolfPack will attempt to load .wav, .mp3 and .wma files.

    - If you add your own clips, all players in multiplayer must have the same clip installed locally if they want to hear the calls of their fellow players. WolfPack will play the clip configured by each player, as long as it has that clip present locally in the mod folder.

### Utility

- **MouseWheelLatency**: Controls the mouse wheel spin behavior so 'big' spins don't 'overshoot' the next creature in the configured list. The default is 3, which should be sufficient for most users. Increase this value if the wheel spin is too sensitive and you find yourself \'skipping' over creatures in the list. Decrease this value if you find the wheel's response is too 'sluggish'. Can be set from 0 to 10. 

- **LogCreatureNames**: If set to True, will log all 'found' creatures called with Follow and Stay. This may be useful to identify the creature name when configuring the _TrainableCreatures_ list. 

### In-game reconfiguration

- You can edit the config file, or use Configuration Manager (or similar) to change the configuration without exiting the game, and then have WolfPack reload it's configuration from the chat window (Enter) by typing `/wolfpack config`. 
- You can also modify many of WolfPack's settings directly from the chat window using this syntax: `/wolfpack command_name=value`, e.g., `/wolfpack PackCallSound=Horn2.wav` would change the configured wolf call sound to "Horn2".

    - The following config items can be changed using this method: _PackCallSound_, _UseTwoKeys_, _DetectionRange_, _MinimumCreatureLevel_, _UseMouseWheel_, _LogCreatureNames_, _UseSound_, _Notifications_, _MouseWheelLatency_, _StrictObedience_

## Multiplayer

- Multiplayer is supported on local and dedicated servers as of 0.9.7
- Wolves are sometimes a bit finicky. It may take a few seconds for them to respond, especially on your first call.
- Wolves are generally loyal and will remain with whomever called them until released, but wait a few seconds after joining before calling them, otherwise some of them may get too excited and leave their current master. 


## Compatibility issues & defects

- While every effort goes into ensuring it works as described, there's no way to test every possible game scenario, especially with other mods or multiplayer.

- WolfPack tries to "play nice", and shouldn't be doing anything that interferes with other mods. That being said, if another mod has its own method for controlling tames, you may experience conflicts. If you find a compatibility issue you can post it on NexusMods at: https://www.nexusmods.com/valheim/mods/1549?tab=posts. Be sure to include the mod name and version you think may be incompatible.

- If you have a bug please report it on NexusMods at https://www.nexusmods.com/valheim/mods/1549?tab=bugs. If you do post a bug report, please make sure to include the following:
   - Your version of WolfPack
   - What you were doing, or attempting to do when it happened
   - If it's repeatable - i.e., can you duplicate it?
   - The exact behavior you observed (or didn't observe)
   - Any errors in the log file (WolfPack errors always begin with "WolfPack ...")

## Notes

WolfPack does not modify any 'pet' interactions with creatures. In other words, you can't use WolfPack to pet individual creatures, such as Lox to Follow or Stay (like Wolves) without some other mod to tame them such as AllTameable (https://www.nexusmods.com/valheim/mods/1571). 

You may find a 'wander' limit (set by _StrictObedience__) of 0 too restrictive. A low, non-zero number gives the creatures a bit of 'wiggle room' while still keeping them grouped together.

'Petting' a 'following' wolf will cause it to Stay, regardless of who it's currently following. This is by design to allow players to 'trade' creatures.

Wolves have a limited attention span. If you leave the game, wolves will get bored and start wandering again, regardless of your _StrictObedience_ settng.

You can mount up and ride at the forefront of a herd of charging Lox!

Shout out to **meldurson** for help and ideas for improving the config for custom creatures.

Your comments and feedback are always welcome. Please feel free to post on NexusMods or send a personal note.

Shameless plug for RequipMe. Instantly re-equip your best gear from your tombstone! https://www.nexusmods.com/valheim/mods/1615