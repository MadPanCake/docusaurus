---
sidebar_position: 4
id: troubleshooting
title: '🛠️ Troubleshooting'
---



# ⚙️ Troubleshooting Guide

Running into issues? This page will walk you through the most common problems and how to solve them.

### ✅ First Things First: Is Your Server Set Up Correctly?

Before anything else, double-check these essentials:
- 🧱 You followed the official [**installation instructions**](https://docs.endernerds.com/installation)
- 🧾 You're running [**Paper 26.2**](https://papermc.io/downloads/paper) as your server jar
- 🆕 You're using the latest version of the setup ([check on BuiltByBit](https://builtbybit.com/resources/unlimited-adventures-survival-setup.27917/updates))
- ☕ You're running Java 25 ([download here](https://www.oracle.com/pl/java/technologies/downloads/#java25))

### ⚠️ Potentially Unsupported Features
Some setups may cause unexpected behavior:
- 🛑 Engines **other than Paper** (like Purpur) — while they may work, only Paper is officially supported.
- ❌ **Unofficial Minecraft clients** — third-party launchers or custom clients can break functionality.
- 🔄 **ViaVersion / ViaRewind / etc.** — allow unsupported versions to join, which may cause bugs or visual issues.

### ⚠️ Check Your Minecraft Client
- ✅ Use **Minecraft 26.2** — other versions aren’t guaranteed to work.
- 🎮 Use the **official launcher**, and avoid mods or custom launchers - those are not guaranteed to work.



-------



## 🎨 Texture Pack Doesn’t Work?

A few things could be causing this:

- 🧩 **Using ItemsAdder or Oraxen?**\
You’ll need to merge the resource pack properly. Use the official guides:\
→ [ItemsAdder Guide](itemsadder)\
→ [Oraxen Guide](oraxen)
- 🈲 **Check the “Force Unicode Font” setting** in your client (disable it).
- 🛠️ **Modified the resource pack or models?**\
Revert to the default files, then reapply changes one by one to find what broke.
- 📁 **Using Oraxen/ItemsAdder?**\
Remove the 📁`modelengine/` folder from the resource pack.
- 🔁 **Broken models?**\
Replace your ModelEngine plugin folder and resource pack with clean files from the original setup.

-----

#### 🔒 "Chat disabled due to missing profile public key. Please try reconnecting."

Open your `server.properties` file (main server folder) and make sure that `enforce-secure-profile` is set to `false`.
```
enforce-secure-profile: false
```

---

#### ☠️ Can't access Dungeons or Spawn?

Make sure these folders exist in your server’s root directory:
- `spawn`
- `dungeons`
- `world`

Also check that:\
📁 `plugins/unlimited_adventures/Dungeons/FloorData` is **not empty**.\
If it is, restore it from a clean setup.

---

#### ✨ Wilderness Teleport doesn't work?

You've probably deleted the `wild_tp` region.\
→ Recreate it to restore teleportation to the Wilderness.

---

#### ✨ Keep getting teleported back to spawn?

The `spawn` world might be missing — possibly deleted manually or when removing the WorldGuard folder.\
→ Recreate it or restore your WorldGuard data.

---

#### 🐢 Random Teleport is slow

The teleport itself is instant — lag comes from new chunk generation.

✅ Fix: Pre-generate your map in a radius equal to (or larger than) your RTP range.
This ensures RTP is truly instantaneous ⭐

---

#### 🪶 Feather above your head?

This means the [Adventure Apparel](adventure_apparel) resource pack is broken or the Adventure Apparel is misconfigured.\
🔁 Revert any changes you made to the resource pack and Adventure Apparel to fix the issue.

---

#### 🧔🏽 Default NPCs Have Weird Text Above Their Heads?

🧼 Just restart your server — this will clear any unwanted NPC text overlays.

---