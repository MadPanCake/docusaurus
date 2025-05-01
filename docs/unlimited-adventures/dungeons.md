---
sidebar_position: 12
title: '💀 Dungeons'
---



# :skull: **Dungeons**

Our very own, custom-developed Dungeons system. It features 3 themed dungeons with 3 floors each.\
Dungeons are filled with monsters, ores and chests to loot. In order to progress to another floor, you have to find a Dungeon Key.\
At the end of every dungeon there is a powerful boss that drops unique items.\
Dungeon Key can be dropped from the Mini-Bosses found in the wilderness.


#### :computer: Commands

To get all the Dungeons commands, please execute: `/dungeons help`

- `/dungeons unlock [player] [floor number]` - unlocks a floor for the player
- `/dungeons resetkey` - resets your unlocked floors

#### :closed_book: Dungeons Menu

Configure Dungeons menu in:\
```plugins/CommandPanels/panels/utility/dungeons```


#### :gear: How to configure Dungeons?

You can find Dungeon's configuration files in:
```unlimited_adventures/Dungeons/```



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

In order to create a new monster spawn, you need to insert this command:\
```/dungeons setmonsterspawn [monster type]```\
For example:\
```/dungeons setmonsterspawn zombie```
> Available monster types are: `zombie`, `skeleton`, `spider`, `husk` & `ghost`.



#### :dragon: How to create a BOSS spawn in my Dungeon?

In order to create a new BOSS spawn, you need to insert this command:\
```/dungeons setbossspawn [bosstype] ```\
For example:\
```/dungeons setbossspawn dracula```

Available BOSS types are: `miner_wrath`, `dracula`, `pharaoh`.

#### :package: How to create a respawnable chest?

In order to create a chest that will respawn, with random content, you need to:
> 1. Place the chest
> 2. Fill the chest with items
> 3. Insert the `/dungeons setchest` command.

By default, the chest will respawn with 3 random items from it's initial inventory.
You can easily change that in the Dungeon's config.


#### Respawnable ores in the dungeons

All ores in dungeons will respawn after a while when being mined.

