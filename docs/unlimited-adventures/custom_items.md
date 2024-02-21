---
sidebar_position: 9
title: 'Custom Items'
---



# :hammer:  The Forge & Custom Items

The Forge is a very special feature that let's players craft new powerful items.

:::tip
You can get all custom items by executing `/getitems`
:::

#### How to edit items?
> You can edit the parameters of custom items by going to:
```plugins/CustomItems/items.yml```

#### How to change recipes?
> Edit recipes for custom items by going to:
```plugins/CustomItems/recipes.yml```


#### How to unlock a recipe?
> If you have it enabled in the config, players will be required to unlock a recipe first, before they can forge an item.\
> In that case, you can unlock items for the players by executing `/forgeunlock [player name] [item name]`, for example: `/forgeunlock Steve1337 adventure_backpack`

### 2 Placeholders available:

`%valiant_craftingunlocked_ITEM%` - returns 'true', if crafting of the specified item is unlocked.\
`%valiant_cancraft_ITEM%` - returns 'true', if the player has required items to craft the item.


