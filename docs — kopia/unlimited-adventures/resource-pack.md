---
sidebar_position: 7
title: 'Resource Pack'
---

import ReactPlayer from 'react-player'
import video from './assets/resource_pack.mov';

import resource_pack_zip from './assets/resource-pack-zip.jpg';




# Resource Pack

This guide will explain how to download the Unlimited Adventures resource pack and then update it.


# 📁 Download server resource pack

#### Step 1
Find `server.properties` file in the main server folder.

#### Step 2
Open the file and look for `resource-pack=`

#### Step 3
Notice that there is a backwards slash added in the beginning. **You have to remove it!** ❌
```
https\://download.mc-packs.net/NOT-AN-ACTUAL-LINK.zip
     ⇧
```


Your link should look like that:\
`https://download.mc-packs.net/NOT-AN-ACTUAL-LINK.zip`

#### Step 4
Copy the link and paste it in your browser.

:::warning
This above link is just an example, download the resource pack using a link from your `server.properties` file!
:::

<ReactPlayer playing controls url={video} />


<br></br>
<br></br>
<br></br>

# ⬆️ How to update the server's resource pack?

#### Step 1

ZIP your resource pack, don't ZIP it inside of a folder. Files should be loose. Refer to the image below.
<img src={resource_pack_zip} alt="Image Description" width="400" height="150"/>

#### Step 2

Upload your ZIP to [MCPacks](https://mc-packs.net/).

#### Step 3

Copy resource pack link and the SHA1.

#### Step 4

Locate the `resource-pack` and paste the new link here.\
Locate `resource-pack-sha1=` and paste the new SHA1 here.

`server.properties:`
```
resource-pack=https\://YOUR-LINK.zip
resource-pack-id=INSERT-YOUR-ID
resource-pack-prompt=
resource-pack-sha1=INSERT-YOUR-SHA1
```

Don't worry about the backwards slash being automatically added after server startup. It's normal.