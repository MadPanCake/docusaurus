---
sidebar_position: 10
title: 'Custom Items'
---



# :hammer:  The Forge & Custom Items

The Forge is a very special feature that let's players craft new powerful items.

:::tip[How to get custom items]
You can get all custom items by executing: `/getitems`\
To get any item, execute: `/giveitem [item name] [player name]`
:::


#### :bulb: How to add new items?
> All custom items are found in: `unlimited_adventures/CustomItems/items.yml`\
> You can add new items simply by duplicating an existing item from the config and changing it's name and properties to your liking.\
> Get your newly created with with `/giveitem [item name]` command!


#### :pencil2: How to edit items?
> You can edit the parameters of custom items by going to:
`unlimited_adventures/CustomItems/items.yml`

#### :pencil2: How to change recipes?
> Edit recipes for custom items by going to:
`unlimited_adventures/CustomItems/recipes.yml`

#### :unlock: How to unlock a recipe?
> If you have it enabled in the config, players will be required to unlock a recipe first, before they can forge an item.\
> In that case, you can unlock items for the players by executing `/forgeunlock [player name] [item name]`, for example: `/forgeunlock Steve1337 adventure_backpack`



## 2 Placeholders available:

| Placeholder | Description |
| - | - |
| `%valiant_craftingunlocked_ITEM%` | returns 'true', if crafting of the specified item is unlocked. |
| `%valiant_cancraft_ITEM%` | returns 'true', if the player has required items to craft the item. |


