---
sidebar_position: 2
title: 'Updating'
---


import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';




# :bulb: **How to update your server?**

If you're already using the setup, but would like to install the update, you can easily do it!

:::warning[Don't skip versions!]
You can't skip setup versions! For example, you can't go from 2.0 to 2.4\
If you are on 2.0, download 2.1, finish all the steps and only then update to 2.2, then 2.3 and so on, until you are on the latest version.
:::

:::warning[Backup first!]
You should **always** backup your files first, before doing any changes or updates.
:::

:::


<Tabs>
  <TabItem value="2.6.1" label="Update 2.6.1">

#### Step 1
Stop your server.

#### Step 2
Remove folders:
- `spawn`
- `plugins/CommandPanels/panels`

#### Step 3
Remove files:
- `plugins/worldedit.jar`
- `plugins/AureliumSkills.jar` 
- `plugins/Skript/scripts/rtp.sk`

#### Step 4
Download [Paper 1.20.4](https://api.papermc.io/v2/projects/paper/versions/1.20.4/builds/485/downloads/paper-1.20.4-485.jar)

#### Step 5
Update [Citizens](https://ci.citizensnpcs.co/job/citizens2/3373/artifact/dist/target/Citizens-2.0.33-b3373.jar).


#### Step 6
Copy all contents of `Update Files` to your main server folder.\
(Click "Change files in the destination")

  </TabItem>
    <TabItem value="Other versions" label="Other versions">

#### Step 1
Stop your server.

#### Step 2
Copy all contents of `Update Files/` folder to your main server folder.\
(Click "Change files in the destination")

  </TabItem>
</Tabs>

:white_check_mark: Done! You can enjoy the latest version of Unlimited Adventures!

