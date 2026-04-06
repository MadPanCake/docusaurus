---
sidebar_position: 5
title: '🖼️ Items Adder'
id: itemsadder
---

import ReactPlayer from 'react-player'


# 🖼️ ItemsAdder

In order for the setup to work with ItemsAdder, you need to merge the resource pack with ItemsAdder.\
It's actually a very simple process. Please refer to the text guide and use the video as a supplement.

:::warning
If it's your first time using ItemsAdder, please refer to its [guide](https://itemsadder.devs.beer/first-install) to learn the basics.
:::

#### Step 1
> :red_circle: Stop your server.

#### Step 2
> ❌ Remove `resource-pack=` link from `server.properties`

#### Step 3
> Open `plugins/BetterModel/config.yml`\
> Find:\
> ```build-folder-location: BetterModel/build```\
> replace it with:\
> `build-folder-location: ItemsAdder\contents\BetterModel\resourcepack`

#### Step 4
> Put Unlimited Adventures resource pack into 📁`plugins/ItemsAdder/contents`
:::tip[Find your resource pack]
Don't know how to find your resource pack? Refer to [Resource Pack](resource-pack)
:::

#### Step 5
> Execute the `/iazip` command.

Done! Now start your server and enjoy Unlimited Adventures and ItemsAdder working together :heart:


<ReactPlayer playing controls url="https://youtu.be/2nsQDgKO4oo"/>
Notice: Video guide is missing the step 3.


### Other sources:

- [Items Adder Installation Guide](https://itemsadder.devs.beer/first-install) - you should read it if it's your first time using Items Adder.
- [Items Adder Resource Pack Merging Guide](https://itemsadder.devs.beer/plugin-usage/merge-resourcepacks) - essentially describes the same thing this guide describes.