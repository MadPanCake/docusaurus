---
sidebar_position: 10
id: custom_items
title: 'Custom Items'
---



# 🪃 Custom Items

Unlimited Adventures includes a built-in, powerful custom items system — no extra plugins needed.\
This guide will show you how to create, modify, summon, and texture your own custom items.

:::tip[How to get custom items]
You can access custom items menu by executing: `/getitems`\
To get a specific item, execute: `/giveitem [item name] [player name] [amount]`
:::


## ➕ How to add new items?
It's really easy to add new items, read more below:

#### 🗒️ All custom items are found in: `unlimited_adventures/CustomItems/items.yml`:
```
items:
    traveler_backpack:
        name: "&aTraveler's Backpack"
        item: stick
        custom_model_data: 501
        model_custom_model_data: 101
        lore:
        - ''
        - "&7Basic backpack. Can fit 18 items."
        rows: 2
        item_id: traveler_backpack
    adventure_backpack:
        name: "&aAdventurer's Backpack"
        item: stick
        custom_model_data: 502
        model_custom_model_data: 102
        lore:
        - ''
        - "&7Sizeable backpack. Can fit 36 items."
        rows: 4
        item_id: adventure_backpack
```

➕ You can add new items simply by duplicating an existing item from the config and changing it's name and properties to your liking:
```
dino_sword:
    name: "&6Dinosaur Sword"
    item: diamond sword
    lore:
    - "&7This sword belongs to"
    - "a very cool dinosaur."
```

💎 On Unlimited Adventures, there are accessories you can wear in the gear menu. Let's create one:
```
belt_of_vitality:
    name: "&aBelt of Vitality"
    item: stick
    custom_model_data: 720
    lore:
    - ''
    - "&7Increases health."
    - ''
    - "§x&d&f&5&2&5&2+4 Health ❤"
    - ''
    - "§x&8&f&6&4&d&eᴀᴄᴄᴇssᴏʀʏ ɪᴛᴇᴍ"
    health: 8
    regeneration: 8
    accessory: true
```

As you can see, I have specified the name, item type, custom model data (so the item can have it's own custom texture) and wrote a short lore description.
But the most important things are down below, the `health` and `regeneration` statistics are applied on the player when he's wearing the accessory.

#### ⚙️ Available attributes:
- Strength
- Health
- Regeneration
- Luck
- Wisdom
- Toughness
- Speed
- Fuel
- Night_vision
- Haste
- Oxygen

## 🎨 Give your item a custom texture

#### Upload your new texture to the server resource pack
1. First, you have to add the texture to your resource pack. You need to [download](resource-pack) it on your computer so you can update it.
2. Put your texture in the 📁`assets/minecraft/textures/custom/items/` folder.
3. Now you need to create a model for your texture, no matter whether it's 3D or not, this model allows us to create a brand new texture, instead of having to sacrifice existing Minecraft items:

Go to 📁`assets/minecraft/models/custom/items/`. Create a new `.json` file or just copy the `amethyst_axe.json ` and rename it to your items name.
Edit its content:
```
{
  "parent": "item/handheld",    <---  Change this to "item/generated" if the item you're creating is not held like a tool.
  "textures": {
    "layer0": "custom/items/dino_sword"
  }
}
```

4. Now we need to link this model to a custom model data of an existing vanilla item - I'll use diamond sword.

Go to `assets/minecraft/models/item/diamond_sword.json`
```
{
  "parent": "minecraft:item/handheld",
  "textures": {
    "layer0": "minecraft:item/diamond_sword"
  },
  "overrides": [
  { "predicate": {"custom_model_data": 730}, "model": "custom/items/bone_sword"},
  { "predicate": {"custom_model_data": 731}, "model": "custom/items/emerald_sword"},
  { "predicate": {"custom_model_data": 732}, "model": "custom/items/copper_sword"},
  { "predicate": {"custom_model_data": 733}, "model": "custom/items/amethyst_sword"},
  { "predicate": {"custom_model_data": 734}, "model": "custom/items/crocodile_sword"},
  { "predicate": {"custom_model_data": 735}, "model": "custom/items/venomous_fang_dagger"},
  { "predicate": {"custom_model_data": 736}, "model": "custom/items/dino_sword"}
  ]
}
```
We are linking it to the path of the model we have created in the previous step. Full path is `assets/minecraft/models/custom/items/dino_sword.json`


#### Update the item config
Now we'll add the just assigned custom model data to our custom item's config.

`unlimited_adventures/CustomItems/items.yml`:
```
dino_sword:
    name: "&6Dinosaur Sword"
    item: diamond sword
    custom_model_data: 736   <-----   Add this line! ⚙️
    lore:
    - "&7This sword belongs to"
    - "a very cool dinosaur."
```







## 📜 How to add/change crafting recipes?
You can add your own workshop recipes or modify existing ones.\
Config can be found in: `unlimited_adventures/CustomItems/recipes.yml`

```
recipes:
    dynamite:
    - 1 of tnt
    - 3 of string
    - 3 of iron ingot
    catching_net:
    - 5 of string
    - 3 of slimeball
```

## 🔓 How to unlock a Workshop Schematic?
Players can unlock new schematics by finding them in the chests in Wilderness.

Alternatively, you can also use commands:
- 🔓 Unlock a recipe: `/workshopunlock [player name] [item name]`,\
for example: `/workshopunlock simon catching_net`

- 🔒 Lock a recipe: `/workshoplock [player name] [item name]`,\
for example: `/workshoplock simon catching_net`



## 2 Placeholders available:

| Placeholder | Description |
| - | - |
| `%valiant_craftingunlocked_ITEM%` | returns 'true', if crafting of the specified item is unlocked. |
| `%valiant_cancraft_ITEM%` | returns 'true', if the player has required items to craft the item. |


