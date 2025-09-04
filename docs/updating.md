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


<TabItem value="2.11" label="Update 2.11">

#### Step 1
:red_circle: Stop your server.

#### Step 2
❌ Remove files:
- 📁`unlimited_adventures/CustomItems/items.yml`
- 📁`unlimited_adventures/CustomItems/schematics.yml`
- 📁`unlimited_adventures/RandomEncounters/chests.yml`

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









  <TabItem value="2.8" label="Update 2.8">

#### Step 1
:red_circle: Stop your server.

#### Step 2
❌ Remove folders:
- 📁 `unlimited_adventures/CustomItems/`
- 📁 `unlimited_adventures/Ambients/`
- 📁 `plugins/ChatManager`
- 📁 `plugins/FastAsyncWorldEdit`
- 📁 `plugins/NexEngine`
- 📁 `plugins/ExcellentEnchants`

#### Step 3
❌ Remove plugins .jar files:
- `ChatManager.jar`
- `Chunky.jar`
- `FastAsyncWorldEdit.jar`
- `ExcellentEnchants.jar` 
- `NexEngine.jar`
- `World Edit.jar`
- `World Guard.jar` (don't remove the folder, it contains regions!)


#### Step 4
❌ Remove scripts:
- `plugins/Skript/scripts/chat_manager.sk`
- `plugins/Skript/scripts/ambients.sk`

#### Step 5
⬇️ Download [Paper 1.21](https://api.papermc.io/v2/projects/paper/versions/1.21/builds/130/downloads/paper-1.21-130.jar)

#### Step 5
⬇️ Update plugins:
- Update [TAB](https://github.com/NEZNAMY/TAB/releases/download/4.1.8/TAB.v4.1.8.jar).
- Update [Citizens](https://ci.citizensnpcs.co/job/Citizens2/3580/artifact/dist/target/Citizens-2.0.35-b3580.jar).
- Update [Model Engine](https://mythiccraft.io/index.php?pages/official-modelengine4-download/&download=free&f=4.0.7).
- Update [Mythic Mobs](https://www.mythiccraft.io/downloads/mythicmobs/free/MythicMobs-5.7.2.jar).


#### Step 6
💾 Copy all contents of 📁`Update Files/` to your main server folder.\
(Click "Change files in the destination")



  </TabItem>








  <TabItem value="2.6.1" label="Update 2.6.1">

#### Step 1
:red_circle: Stop your server.

#### Step 2
❌ Remove folders:
- 📁 `spawn`
- 📁 `plugins/CommandPanels/panels`

#### Step 3
❌ Remove files:
- `plugins/worldedit.jar`
- `plugins/AureliumSkills.jar` 
- `plugins/Skript/scripts/rtp.sk`

#### Step 4
⬇️ Download [Paper 1.20.4](https://api.papermc.io/v2/projects/paper/versions/1.20.4/builds/485/downloads/paper-1.20.4-485.jar)

#### Step 5
⬇️ Update [Citizens](https://ci.citizensnpcs.co/job/citizens2/3373/artifact/dist/target/Citizens-2.0.33-b3373.jar).


#### Step 6
💾 Copy all contents of 📁`Update Files/` to your main server folder.\
(Click "Change files in the destination")


  </TabItem>

</Tabs>

#### :white_check_mark: Done! You can enjoy the latest version of Unlimited Adventures!

