---
sidebar_position: 8
id: bedrock
title: 'Bedrock'
---



# ⚙️ Bedrock Support
**Unlimited Adventures can be expanded with full Minecraft Bedrock support through an optional paid add-on.**

Once enabled, players can join your server from PC, consoles, mobile devices, and Nintendo Switch. The add-on also includes a dedicated Bedrock resource pack with adapted menus, custom mobs, and other cross-platform features.

---

## ⚙️ Setting up Bedrock
1. Make sure you have an **extra port available** for Bedrock connections.
2. Set that port in `plugins/Geyser-Spigot/config.yml`

:::warning
Using multiple Bedrock resource packs at the same time may cause conflicts or unexpected behavior.
:::


## 🔁 Velocity / BungeeCord Installation

1. Delete `Geyser-Spigot.jar` from your 📁`/plugins/` folder.
2. Copy all files from 📁`/plugins/Geyser-Spigot/` into one of the following (depending on your setup):\
📁`/plugins/Geyser-Velocity/`\
📁`/plugins/Geyser-Bungee/`
3. In the Floodgate config, set the following:
```
send-floodgate-data: true
```

## ⚠️ Known Issues
These features will not work on Bedrock due to Geyser limitations:
- Clickable links in chat
- Custom enchantments

For a full list, please visit [Geyser's wiki](https://geysermc.org/wiki/geyser/current-limitations)