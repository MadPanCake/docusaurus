---
sidebar_position: 15
title: 'Daily Rewards'
---



# :gift: Daily Rewards Config

Valiant Survival utilizes our own, powerful, custom-developed Daily Rewards system.
Thanks to this, you can use: up to 4 different reward types, 4 placeholders and 2 variables!



#### :package: How to change rewards?

You can easily add, change or remove rewards from our Daily Rewards system.
In order to do so, you need to find the `plugins/DailyRewards/rewards.yml` config file.



### 4 Types of rewards available:

#### :moneybag: Gold Rewards:
In order to add a gold reward, you have to type in:
`gold [amount]`, for example: `gold 500`

#### :gem: Gems Rewards:
In order to add a gems reward, you have to type in:
`gems [amount]`, for example: `gems 500`


#### :hammer: Item Rewards:
In order to add a gold reward, you have to type in:
`[amount] of [item]`, for example: `5 of iron sword`.

:::tip
Enchantments are also supported:
`iron sword of sharpness 5 and unbreaking 3`

You can even use names!\
`iron sword named "&6&lPowerful Sword" of sharpness 5 and fire aspect 2 and unbreaking 3`

You can make the item unbreakable:\
`unbreakable iron sword named "&6&lPowerful Sword" of sharpness 5 and fire aspect 2 and unbreaking 3`
:::

#### :computer: Command Rewards: You can use commands as rewards, by doing as following:
`command premiumcurrency PLAYER_NAME add 100`



### 4 Placeholders available:

`%valiant_dailyrewards_canclaim%` - This placeholder returns "true", when player has an unclaimed Daily Reward.
`%valiant_dailyrewards_timeuntilclaim%` - This placeholder returns the time left until a player can claim his Daily Reward.
`%valaint_dailyrewards_timeuntilexpiration%` - This placeholder returns the time left until the unclaimed Daily Reward expires and the strike resets.
`%valiant_dailyrewards_daynumber%` - This placeholder returns the Daily Rewards day, the player is at.



### 2 Variables available:

`PLAYER_NAME` - the player's nickname.\
`DAY_NUMBER` - the player's daily reward number.