---
sidebar_position: 4
title: 'Troubleshooting'
---



# 🔧 Solving common problems

We understand that sometimes working on your server doesn't go as intended and `stuff breaks`.\
This guide has been made to provide quick help in such situations!


### ⚠️ Firstly - Make sure your server is properly installed

1. Make sure you have installed the setup according to the 📗 [**installation instructions**](https://endernerds.netlify.app/docs/unlimited-adventures/installation)
2. Make sure you are on 📄 [**Paper 1.21**](https://api.papermc.io/v2/projects/paper/versions/1.21/builds/130/downloads/paper-1.21-130.jar)
3. Make sure you are using the 🟢 [**latest setup version**](https://builtbybit.com/resources/unlimited-adventures-survival-setup.27917/updates)
4. Make sure you are using ☕ [**Java 21**](https://www.oracle.com/pl/java/technologies/downloads/#java21)


#### 🎨 Texture pack doesn't work?

There are a few possible reasons why the texture pack doesn't work on your server.

1. Have you installed Oraxen or ItemsAdder? If yes, then you have to merge the resource pack. Use the respective guides: [Oraxen](oraxen) [ItemsAdder](itemsadder)
2. Check if `force unicode` setting is disabled in your client language settings.
3. Have you made any modifications to the resource pack or models? Your changes can easily break stuff, please revert to the default files and test your changes one by one to find out what causes issues.
4. If you are using Oraxen or ItemsAdder, you have to remove the `modelengine` folder from your resource pack. Did you do it?
5. Do you have problems with models? Try to swap your `ModelEngine` plugin folder and resource pack files with original files from a clean setup installation.

#### ☠️ Can't access Dungeons or Spawn?

1. Make sure you have all the world folders available in the root directory of your server.
- 'spawn'
- 'dungeons'
- 'world'

2. Make sure your `unlimited_adventures/Dungeons/FloorData` folder is not empty. If it's empty, you have to recover the files from a clean setup installation.

#### ✨ Wilderness Teleport doesn't work

You have most likely removed the `wild_tp` region which indicates an area that teleports players to Wilderness.

#### ✨ I keep getting teleported back to spawn

You have likely removed the `spawn` region from spawn either manually, or by removing the WorldGuard folder.

#### ✨ Random Teleport is slow

Our Random Teleport in itself is completely instant - it doesn't introduce any lag or delay.
But when you are performing a RTP, it might try to generate a new chunk for you. That's what causes the visible lag.\
Easy solution to this problem is to pregenerate your map in a radius that's at least as big as your RTP range.\
If you do this, you will get instantenous Random Teleporting on your server! ⭐

#### 🪶 I see a feather above my head

Seeing feather above your head means the [Adventure Apparel](adventure_apparel) resource pack files have broken.\
Try to revert any resource pack changes you did to fix the issue.

#### 🧔🏽 NPC's have an unwanted text above their head

Please restart your server.