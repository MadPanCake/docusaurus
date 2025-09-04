---
sidebar_position: 12
title: '💀 Dungeons'
---



# :skull: **Dungeons**

> *“Beneath the earth lie forgotten realms… places where shadows breathe, monsters lurk, and treasures gleam for those bold enough to claim them. Many enter—few return.”*  

In **Unlimited Adventures**, Dungeons are more than just rooms full of monsters—  
they are **living trials** of wit, courage, and survival. Each one is crawling with :spider: enemies, laced with :boom: traps, and hiding 💰 rewards beyond imagination.  
Only the bold will return alive.

## 🔒 Locked Dungeons

Ancient strongholds sealed by powers unknown. To enter, you must first claim a 🔑 **Dungeon Key**, earned by defeating rare **Mini Bosses** hidden across the Wilderness.

### 👹 Mini Bosses
- Skeleton Chieftain - Haunts all types of forests.
- Nosferatu - lurks in the high mountain peaks. 
- Desert Outcast - roams the burning sands.

### 🏰 Locked Dungeon Realms
Each Dungeon spans **three perilous floors**, with gates that only open once enough foes have been slain.

**⛏ Abandoned Mining Site**  
- Forgotten Tunnels  
- Overgrown Mineshaft  
- Forbidden Cavern *(Boss: Miner’s Wrath)*  

**🦇 Dracula’s Manor**  
- Haunted Cemetery  
- Crypt  
- Dracula’s Castle *(Boss: Lord Dracula)*  

**🏺 Ancient Ruins**  
- Desert Canyon  
- Ancient City  
- Pyramid *(Boss: Pharaoh)*


## Wilderness Dungeons

The **wildest test of adventure**—designed for explorers who crave more than mindless battle. Here, you’ll face :brain: riddles, :exclamation: traps, and :crossed_swords: foes in equal measure.

Seek out shimmering portals deep in the Wilderness to uncover them… if you dare.  

### 🕷 The Crawling Depths

**Backstory**  
> *“Long ago, settlers carved a home in a vast cave. They built shrines, grew crops among fungi, and children laughed in the dark.  
> Then the ground split. **Spiders the size of wolves** poured out, dragging settlers into the abyss. Their homes remain untouched—tables still set, toys abandoned… and whispers of laughter still echo through the tunnels.”* 

**The Dungeon**  
The Crawling Depths spans **eight massive, procedurally generated chambers**, each steeped in danger and mystery:
- 🍄 Fungal Cavern  
- 🌊 Flooded Catacombs  
- 🍄 Fungal Storage  
- 📚 Labyrinthine Archive  
- 🕸 Silken Bridge  
- 🏴‍☠️ Bandit Camp  
- 🏚 Abandoned Village  
- 👑 Queen’s Lair

### Features
- :sparkles: Entrance lies **underground, below Y:0**.  
- :spider: Four unique spider foes—including eggs that hatch if disturbed.  
- :scroll: Each room has its own **story, ambient sounds, and atmosphere**.
- 🧩 Devious **riddles** to solve, :boom: **traps** to survive, and ⚔️ **challenges** to overcome.  
- 🎁 Loot hidden in pots, barrels, and treasure chests.  


-----


# For Admins

## Locked Dungeons

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

