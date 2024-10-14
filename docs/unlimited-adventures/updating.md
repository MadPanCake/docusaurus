---
sidebar_position: 3
title: 'Updating'
---


import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';




# :bulb: **How to update your server?**

If you're already using the setup, but would like to install the update, you can easily do it!

:::warning[Don't skip versions!]
You can't skip setup versions! For example, you can't go from 2.6 to 2.8\
If you are on 2.6, download 2.7, finish all the steps and only then update to 2.8, then 2.9 and so on, until you are on the latest version.
:::

:::danger[Backup first!]
You should **always** backup your files first, before doing any changes or updates.
:::




<Tabs>

    <TabItem value="Other versions" label="Other versions">

#### Step 1
:red_circle: Stop your server.

#### Step 2
Copy all contents of `Update Files/` folder to your main server folder.\
(Click "Change files in the destination")

  </TabItem>


  <TabItem value="2.8" label="Update 2.8">

#### Step 1
:red_circle: Stop your server.

#### Step 2
❌ Remove folders:
- `unlimited_adventures/CustomItems/`
- `unlimited_adventures/Ambients/`
- `plugins/ChatManager`
- `plugins/FastAsyncWorldEdit`
- `plugins/NexEngine`
- `plugins/ExcellentEnchants`

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
💾 Copy all contents of `Update Files` to your main server folder.\
(Click "Change files in the destination")



  </TabItem>
  <TabItem value="2.6.1" label="Update 2.6.1">

#### Step 1
:red_circle: Stop your server.

#### Step 2
❌ Remove folders:
- `spawn`
- `plugins/CommandPanels/panels`

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
Copy all contents of `Update Files` to your main server folder.\
(Click "Change files in the destination")


  </TabItem>

</Tabs>

:white_check_mark: Done! You can enjoy the latest version of Unlimited Adventures!

