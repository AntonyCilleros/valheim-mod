Complete rewrite of Vitality Skill. Credits for the idea go to ﻿Xerepp01. His mod was not being maintained anymore and didn't work in the latest version of Valheim anymore. While this was fixed by Hub, there where still many unwanted quirks in that version of the mod. I have rewritten the whole thing with the aim of removing those quirks, keeping as many of the the ideas of the original mod as I deem reasonable and making the config both complete and understandable.

The vitality skill will have the following effects on your character:

    Increased maximum health
    Increased maximum stamina
    Decreased health regeneration timer
    Increased base stamina regeneration
    Decreased delay before stamina regeneration starts again
    Jump and swim stamina cost reduction
    Walking and running speed
    Swimming speed and turning speed while swimming
    Carry weight increase
    Jump height increase
    Fall damage decrease (both fixed compared to original mod where fall damage was reduced the longer you where in the air and configurable now)
    Wood cutting damage increase (should have been in the original mod but failed to work)
    Mining damage increase (should have been in the original mod but failed to work)


The vitality skill can be increased by:

    Running (unchanged).
    Swimming (not just floating). Compared to original mod no longer gaining this and running gain when running in shallow water...
    Jumping. Increased by almost a factor of 10 since this was doing almost nothing in original mod.
    Wood cutting. Slightly increased skill gain per hit with better axe.
    Mining. Slightly increased skill gain per hit with better pickaxe.
    The amount of gain can be modified in the config file.


Remark: All changes to variables usually constant in vanilla Valheim are now done at character load and whenever the vitality skill is leveled up rather than every 0.02 seconds. This means, that some changes done in Configuration Manager will not a﻿utomatically be applied during the game. You can force an update though via 'vitalityrewrite apply' in the console (does not required devcommands). You can also reload a changed cfg file using 'vitalityrewrite reload' .

### Changelog
1.0.1 Added option to reset your "fall velocity" when doing a jump. Does nothing without other mods but lets you dampen your fall using in-air jumps (EpicLoot offers an enchant to do this, others could as well).

