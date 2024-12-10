---
sidebar_position: 13
title: 'Badges'
---



# 🎖️ Player Badges

We have designed Badges to reward the most ambitious players with a satisfying award.\
Progress and unlocked badges can be viewed in the Badges menu.\
The total amount of badge levels is displayed below player's name, along with a star icon, for example: `17 ⭐`

## ➕ How to add new badges?

You can easily add new badges by editing the Badges config file:

`unlimited_adventures/Badges/badges.yml`:
```
your_badge:
    '1':
        requirement: statistic_mine_block:STONE
        value: 100
    '2':
        requirement: statistic_mine_block:STONE
        value: 500
    '3':
        requirement: statistic_mine_block:GRAVEL
        value: 100
    '4':
        requirement: statistic_mine_block:SAND
        value: 150
```

Add rewards in the rewards config - `unlimited_adventures/Badges/rewards.yml`:
```
your_badge:
    '1':
        '1': command eco give PLAYER_NAME 100
    '2':
        '1': command eco give PLAYER_NAME 150
    '3':
        '1': command eco give PLAYER_NAME 200
    '4':
        '1': command eco give PLAYER_NAME 250
```

Set the badge messages in `unlimited_adventures/Badges/messages.yml`:

```
your_badge_level_up: "§x&f&f&e&8&1&7&lBadges ▶ §x&3&1&e&d&9&6Your Badge is now: LEVEL Badge!"
your_badge_badge_level: "§x&f&f&e&8&1&7&lBadges ▶ LEVEL Your Badge"
```

## ✏️ Editing badges

#### ⚙️ How to change Badge requirements?

To change the badge requirements, go to:
```unlimited_adventures/Badges/badges.yml```
In there, you can modify various badge categories and their levels.
Please notice that badges use placeholders to reliably track player's progress.\
You can find a rich list with a lot of placeholders [here](https://github.com/PlaceholderAPI/PlaceholderAPI/wiki/Placeholders).\
(Please note that some of them require you to install them with `/papi ecloud download name`)



#### :package: How to change Badge rewards?

You can easily change the badge rewards. To do it, head to:
```unlimited_adventures/Badges/rewards.yml```
In there, you can modify the rewards for different badge categories and tiers.





### 4 Types of rewards available:

#### :moneybag: Gold Rewards:
In order to add a gold reward, you have to type in:
`gold [amount]`, for example: `gold 500`

#### :gem: Gems Rewards:
In order to add a gems reward, you have to type in:
`gems [amount]`, for example: `gems 500`


#### :hammer: Item Rewards: In order to add a gold reward, you have to type in:
`[amount] of [item]`, for example: `5 of iron sword`.

:::tip
Enchantments are also supported:\
`iron sword of sharpness 5 and unbreaking 3`

You can even use names!\
`iron sword named "&6&lPowerful Sword" of sharpness 5 and fire aspect 2 and unbreaking 3`

You can make the item unbreakable:\
`unbreakable iron sword named "&6&lPowerful Sword" of sharpness 5 and fire aspect 2 and unbreaking 3`
:::

#### :computer: Command Rewards:
You can use commands as rewards, by doing as following:\
`command premiumcurrency PLAYER_NAME add 100`
