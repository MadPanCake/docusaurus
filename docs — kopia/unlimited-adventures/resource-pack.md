---
sidebar_position: 3
title: 'Resource Pack'
---

import resource_pack_zip from './assets/resource-pack-zip.jpg';



# :file_folder:  How to access the resource pack?

This guide will explain how to download the Unlimited Adventures resource pack.

#### Step 1
Find `server.properties` file in the main server folder.

#### Step 2
Open the file and look for `resource-pack=`

#### Step 3
Notice that there is a backwards slash added in the beginning. **You have to remove it!**\
`https\://download.mc-packs.net/pack/afdbe0108c6d2126eddb96c57013829bd00e4300.zip`


Your link should look like that:\
`https://download.mc-packs.net/pack/afdbe0108c6d6126eddb96d57013839bd00e4300.zip`

#### Step 4
Copy the link and paste it in your browser.

:::warning
This above link is just an example, download the resource pack using a link from your `server.properties` file!
:::




<br></br>
<br></br>
<br></br>

# How to update the server's resource pack?

**Step 1**
> ZIP your resource pack, don't ZIP it inside of a folder. Files should be loose. Refer to the image below.
<img src={resource_pack_zip} alt="Image Description" width="400" height="150"/>

**Step 2**
> Upload your ZIP to [MCPacks](https://mc-packs.net/).

**Step 3**
> Copy resource pack link and the SHA1.

**Step 4**
> Locate the `resource-pack` in `server.properties`, paste the new link here.\
> Locate `resource-pack-sha1=` and paste the new SHA1 here.


