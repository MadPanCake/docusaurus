---
sidebar_position: 8
title: 'Bedrock'
---



## ⚙️ Setting up Bedrock

1. Ensure you have an extra port available for Bedrock.
2. Set that port in `plugins/Geyser-Spigot/config.yml`

:::warning
Using multiple Bedrock resource packs at the same time may cause conflicts or unexpected behavior.
:::


## Velocity/Bungee Install

1. 🧹 Remove `Geyser-spigot.jar` from your 📁`plugins/` folder.
2. Copy all files from 📁`plugins/Geyser-Spigot/` into either:\
📁`plugins/Geyser-Velocity` or\
📁`plugins/Geyser-Bungee` — depending on your proxy.
3. 🔧 In the Floodgate config, set:
```
send-floodgate-data: true
```