# Fix for single player using CLLC

[Creature Level and Loot Control](https://valheim.thunderstore.io/package/Smoothbrain/CreatureLevelAndLootControl/) is a
really nice mod, but the ThunderStore download comes with some defaults enabled that you might want to disable.
Unfortunately those defaults are stored into the mod's PLUGINS folder and therefore you cannot provide other config to
overwrite those in your mod that uses CLLC. The only way I see to make CLLC work with ONLY YOUR DESIRED config is to
simply add this mod, which will just delete the files from the plugins folder on game boot, so even if you download a
CLLC update, those files get wiped again.

If you ever wondered, why you never pickup Ooze, this is the reason ;)

## Changelog

* 1.0.1 -> fix config file name
* 1.0.0 -> initial version

## Contact

* https://github.com/FelixReuthlinger/cllc-fix
* Discord: Flux#0062 (you can find me around some of the Valheim modding discords, too)
