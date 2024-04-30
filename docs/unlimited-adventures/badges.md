---
sidebar_position: 13
title: 'Badges'
---



# Player Badges

Badges is our entirely unique feature. Designed to reward the most ambitious players with a satisfying badge award.



#### How to change Badge requirements?

To change the badge requirements, go to:
```unlimited_adventures/Badges/badges.yml```
In there, you can modify various badge categories and their levels.
Please notice that badges use placeholders to reliably track player's progress.



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
