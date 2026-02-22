---
sidebar_position: 3
title: '⬇️ Updating'
---


import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';




# :bulb: **How to update your server?**

If you're already using the setup, but would like to install the update, you can easily do it!

:::warning[Don't skip versions!]
You must update sequentially! For example, you cannot jump directly from 2.8 to 2.9\
You need to go in order, example: 2.8.5 ➡️ 2.8.6 ➡️ 2.8.7 ➡️ 2.9
:::

:::danger[Backup first!]
Make sure to back up your files before making any changes or updates—it's always better to be safe than sorry!
:::




<Tabs>






  <TabItem value="Other versions" label="Other versions">

#### Step 1
:red_circle: Stop your server.

#### Step 2
💾 Copy all contents of 📁`Update Files/` folder to your main server folder.\
(Click "Change files in the destination")

  </TabItem>


  <TabItem value="2.13" label="Update 2.13">

#### Step 1
:red_circle: Stop your server.

#### Step 2
❌ Remove `Paper.jar`

#### Step 3
❌ Remove folders:
- 📁 `world/datapacks/`
- 📁 `plugins/Citizens/`
- 📁 `plugins/floodgate/`
- 📁 `plugins/GeyserModelEngine/`
- 📁 `plugins/Geyser-Spigot/`
- 📁 `plugins/GeyserUpdater/`
- 📁 `plugins/ModelEngine/`
- 📁 `plugins/ExcellentEnchants/enchants/`

#### Step 4
❌ Remove plugins:
- `Citizens.jar`
- `Floodgate.jar`
- `GeyserModelEngine.jar`
- `Geyser-Spigot.jar`
- `GeyserUpdater.jar`
- `GeyserUtils.jar`
- `ModelEngine.jar`
- `MythicMobs.jar`
- `TAB.jar`

#### Step 5
⬇️ Update dependencies:
- Update [TAB](https://github.com/NEZNAMY/TAB/releases/download/5.5.0/TAB.v5.5.0.jar)
- Update [MythicMobs](https://mythiccraft.io/downloads/mythicmobs/free/MythicMobs-5.11.2.jar)
- Download [Paper](https://papermc.io/downloads/paper)

#### Step 6
💾 Copy all contents of 📁`Update Files/` folder to your main server folder.\
(Click "Change files in the destination")

  </TabItem>

  

<TabItem value="2.12" label="Update 2.12">

#### Step 1
:red_circle: Stop your server.

#### Step 2
❌ Remove folders:
- 📁 `plugins/Geyser-Spigot/packs/`
- 📁 `plugins/Geyser-Spigot/custom_mappings/`
- 📁 `plugins/Geyser-Spigot/extensions/`

#### Step 2
❌ Remove plugins:
- `Floodgate.jar`
- `GeyserModelEngine.jar`
- `Geyser-Spigot.jar`
- `GeyserUpdater.jar`
- `GeyserUtils.jar`
- `ViaVersion.jar`

#### Step 3
💾 Copy all contents of 📁`Update Files/` folder to your main server folder.\
(Click "Change files in the destination")

  </TabItem>


<TabItem value="2.10" label="Update 2.10">

#### Step 1
:red_circle: Stop your server.

#### Step 2
❌ Remove file: 📁`plugins/Geyser-Spigot/packs/Bedrock_RP.zip`

#### Step 3
💾 Copy all contents of 📁`Update Files/` folder to your main server folder.\
(Click "Change files in the destination")

  </TabItem>



  <TabItem value="2.9.1" label="Update 2.9.1">

#### Step 1
:red_circle: Stop your server.

#### Step 2
❌ Remove folder: 📁`world/datapacks/`

#### Step 3
❌ Remove plugins:
- `BlueSlimeCore.jar`
- `Citizens.jar`
- `CombatLogX.jar`
- `ConsoleSpamFix.jar`
- `ModelEngine.jar`
- `MythicMobs.jar`
- `PacketEvents.jar`
- `TAB.jar`
- `TChat.jar`

#### Step 4
❌ Remove folders:
- 📁 `plugins/BlueSlimeCore/`
- 📁 `plugins/CombatLogX/`
- 📁 `plugins/ConsoleSpamFix/`
- 📁 `plugins/TChat/`

#### Step 5
⬇️ Update to [1.21.4 Paper.jar](https://api.papermc.io/v2/projects/paper/versions/1.21.4/builds/227/downloads/paper-1.21.4-227.jar)

#### Step 6
⬇️ Update plugins:
- Update [TAB](https://github.com/NEZNAMY/TAB/releases/download/5.2.0/TAB.v5.2.0.jar)
- Update [Citizens](https://ci.citizensnpcs.co/view/Citizens/job/Citizens2/3727/artifact/dist/target/Citizens-2.0.37-b3727.jar)
- Update [Model Engine](https://mythiccraft.io/downloads/modelengine4/free/ModelEngine-4.0.8.jar)
- Update [Mythic Mobs](https://mythiccraft.io/downloads/mythicmobs/free/MythicMobs-5.8.2.jar)


#### Step 7
💾 Copy all contents of 📁`Update Files/` folder to your main server folder.\
(Click "Change files in the destination")

  </TabItem>






</Tabs>

#### :white_check_mark: Done! You can enjoy the latest version of Unlimited Adventures!

