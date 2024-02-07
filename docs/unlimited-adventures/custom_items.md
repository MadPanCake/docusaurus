---
sidebar_position: 9
title: 'Custom Items'
---



# :hammer:  The Forge & Custom Items

The Forge is a very special feature that let's players craft new powerful items.

#### How to edit Forge Items?
> You can edit the parameters of custom items by going to:
```plugins/TheForge/items.yml```

#### How to change recipes?
> Edit recipes for custom items by going to:
```plugins/TheForge/recipes.yml```

#### List of custom items
> You can get custom items without crafting them by executing `/getitems`

#### How to unlock a recipe?
> If you have it enabled in the config, players will be required to unlock a recipe first, before they can forge an item.
> In that case, you can unlock items for the players by executing `/forgeunlock PLAYER_NAME ITEM_NAME`, for example:
```/forgeunlock Steve1337 adventure_backpack```

### 2 Placeholders available:

`%valiant_craftingunlocked_ITEM%` - returns 'true', if crafting of the specified item is unlocked.\
`%valiant_cancraft_ITEM%` - returns 'true', if the player has required items to craft the item.


