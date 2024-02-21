---
sidebar_position: 10
title: 'Dungeons'
---



# :skull: **Dungeons**

Our very own, custom-developed Dungeons system. It features 10 unique floors and 2 boss arenas.\
Dungeons are filled with monsters, ores and chests to loot. In order to progress to another floor, you have to find a Dungeon Key.


#### :computer: Commands

To get all the Dungeons commands, please execute: `/dungeons help`

- `/dungeons unlock [player] [floor number]` - unlocks a floor for the player
- `/dungeons resetkey` - resets your unlocked floors

#### :closed_book: Dungeons Menu

Configure Dungeons menu in:\
```plugins/CommandPanels/dungeons```


#### :gear: How to configure Dungeons?

You can find Valiant Dungeon's configuration file at:
```plugins/Dungeons/config.yml```



#### :crossed_swords: How to create a new Dungeon?

In order to create a new Dungeon, first, you have to create a location and a portal leading to the location.

> 1. To create the Dungeon's spawn location:\
```/dungeons setlocation [floor number]```

> 2. Next, you need a portal that will teleport a player inside of the Dungeon.\
Portals are built with Black Concrete block. You should build a portal, aim at the Black Concrete block and insert this command:\
```/dungeons setportal [floor number]```

:lock: If you'd like the portal to require a key to be unlocked (like the default Dungeons do), you need to add '1' at the end of the command, like this:\
```/dungeons setportal [floor number] 1```\
Example:
```/dungeons setportal 11 1```




#### :boar: How to create a monster spawn in my Dungeon?

In order to create a new monster spawn, you need to insert this command:
```/dungeons setmonsterspawn [monster type] [floor number] [spawn number]```
For example:
```/dungeons setmonsterspawn zombie 11 1```
> Available monster types are: `zombie`, `skeleton` & `spider`



#### :dragon: How to create a BOSS spawn in my Dungeon?

In order to create a new BOSS spawn, you need to insert this command:\
```/dungeons setbossspawn [bosstype] [floor number]```\
For example:\
```/dungeons setbossspawn zombie_brute  5```

Available BOSS types are: `zombie_brute`, `skeleton_king`

#### :package: How to create a respawnable chest?

In order to create a chest that will respawn, with random content, you need to:
> 1. Place the chest
> 2. Fill the chest with items
> 3. Insert the `/dungeons setchest` command.

By default, the chest will respawn with 3 random items from it's initial inventory.
You can easily change that in the Valiant Dungeon's config.


#### :bricks: How to create a respawnable block?

In order to create a block that will respawn, you need to:
> 1. Hold the block that you'd like to respawn.
> 2. Insert the `/dungeons respawnableblock` command.
> 3. Place the block wherever you'd like.
> 4. You'll know that it's working if you see a message on chat `'[Dungeons] Block placed!'`

:moneybag: **How to set Boss Loot?**

In order to set the possible loot from a Boss, you need to:
> 1. Place the chest
> 2. Fill the chest with items
> 3. Insert the `/dungeons setbossloot [bosstype]` command.
Available BOSS types are: zombie_brute, skeleton_king

### 3 Placeholders available

`valiant_dungeon_unlocked_FLOORNUMBER` - returns `'true'`, if specified floor is unlocked, `'false'` if not.
`valiant_zombie_brute_timeuntilrespawn` - returns the time until Zombie Brute BOSS respawns.
`valiant_skeleton_king_timeuntilrespawn` - returns the time until Skeleton King BOSS respawns.


