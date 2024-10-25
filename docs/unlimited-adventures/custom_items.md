---
sidebar_position: 10
title: 'Custom Items'
---



# 🏹 Custom Items

Unlimited Adventures is equipped with a powerful, built-in custom items system.\
This page will explain how to create new custom items, modify them and how to summon them.

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

#### Available statistics:
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




### :pencil2: How to change crafting recipes?
Edit the Forge Block recipes for custom items by going to: `unlimited_adventures/CustomItems/recipes.yml`

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

### :unlock: How to unlock a recipe?
If you have enabled it in the config, players will be required to unlock a recipe first, before they can forge an item.\
In that case, you can unlock items for the players by executing:\
`/forgeunlock [player name] [item name]`, for example: `/forgeunlock Simon adventure_backpack`



## 2 Placeholders available:

| Placeholder | Description |
| - | - |
| `%valiant_craftingunlocked_ITEM%` | returns 'true', if crafting of the specified item is unlocked. |
| `%valiant_cancraft_ITEM%` | returns 'true', if the player has required items to craft the item. |


