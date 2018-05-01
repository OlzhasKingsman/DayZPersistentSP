# DayZPersistentSP
Mod for the 0.63 Singleplayer mode that saves characters.

Hello! 
This is the updated, cleaner version of this mod: https://www.reddit.com/r/dayz/comments/8ftcs2/063_persistent_singleplayer_mod_update_10_save/

Everything related to saving characters has now been moved to the init.c file (instead of the independant scripts folder).
It is now a lot cleaner to read and no need for thousands of lines of code in the scritps folder that the Mission script module dependend on.

This should bring a much cleaner, more stable, future-proof build. There is also less work involved with switching to Multiplayer if there is an online stress test happening. (after removing "scripts" folder, you don't need to do anything)

# Installation instructions:

1. Download this repository as a .zip file. Green button, top right. (or clone it directly to your mission folder if you want.)

2. **[IF YOU HAVE ANY OLDER VERSION OF MY MOD, FROM REDDIT]** Delete the "scripts" folder in your DayZ folder entirely. There is no need for it anymore. **I repeat, there should be no folder called "scripts" in your DayZ installation folder. At all.**

3. Place the "init.c" and "CustomLifestateOverride.c" files inside "[DayZ install folder]/Missions/dayzOffline.ChernarusPlus/". Overwrite init.c.

4. Run DayZ from Steam with the "Play DayZ Offline" option.

# Keybinds:

SHIFT+B: Shave your beard. You need to have a knife in your hand.

SHIFT+P: Deletes save file and respawn. (automatically reloads the mission).

# Settings:

In the init.c file there are a few variables you change:

**extendedLoadout:** if this is set to *true* you will spawn with the default offline mode gear. (IZH, Makarov, knife etc.). If this is set to *false* you will spawn with a hoodie, pants and 4 rags. 

**sleepdelay:** Time (in ms) between mission updates. This might be a good idea to set to a higher value of you are having FPS problems.

# Beards:

You heard correct, beards are in this build! As of right now it takes 30 minutes for half beardness, 60 minutes for a full beard.

*Known issues:

1. Some ambient sounds dissappear after restarting mission. Restart the game completely to fix.

2. Some items may spawn in the wrong slot. (Or on the ground, always check the ground below you when you spawn in)

3. Magazine ammo counters and item quantities do not save. They will always be set to max when spawning in.
