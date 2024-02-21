---
sidebar_position: 8
title: 'Adventure Pass'
---





# :dart: **Adventure Pass**

We take pride in having the best Battle Pass implementation out there.
This guide aims to make the usage of this solution as easy as possible.


### Where is the config?
You can find the Adventure Pass config file in:
`plugins/AdventurePass`

### Adventure Pass Menu
Adventure Pass menu can be configured in:\
`plugins/CommandPanels/battlepass_menu`

### How to start/reset the season?

If you'd like to reset the current season (all players' progress, levels, XP and rewards), you have to execute this command:\
`/adventurepass newseason`


### How to add Adventure Pass XP to a player?

You can easily add Adventure Pass Experience to a player by using the `/adventurepass givexp` command, example:\
`/adventurepass givexp [player] [amount]`



### :package: How to change Adventure Pass rewards?

You can easily add, change or remove rewards from our Adventure Pass system.\
In order to do so, you need to find the `plugins/AdventurePass/rewards.yml` config file.



### 4 Types of rewards available:

#### :moneybag: Gold Rewards
In order to add a gold reward, you have to type in:\
`gold [amount]`, for example: `gold 500`

#### :gem: Gems Rewards:
In order to add a gems reward, you have to type in:\
`gems [amount]`, for example: `gems 500`


#### :hammer: Item Rewards:
In order to add a gold reward, you have to type in:\
`[amount] of [item]`, for example: `5 of iron sword`.

> Enchantments are also supported:\
`iron sword of sharpness 5 and unbreaking 3`

> You can even use names!\
`iron sword named "&6&lPowerful Sword" of sharpness 5 and fire aspect 2 and unbreaking 3`

> You can make the item unbreakable:\
`unbreakable iron sword named "&6&lPowerful Sword" of sharpness 5 and fire aspect 2 and unbreaking 3`


#### :computer: Command Rewards:
You can use commands as rewards, by doing as following:\
`command premiumcurrency PLAYER_NAME add 100`



### 15 Placeholders available:

- `%valiant_battlepass_rewardavailable%` - This placeholder returns "true", if the player has available, unclaimed rewards.
- `%valiant_battlepass_premium%` - This placeholder returns "true", if the player has the Premium Pass.
- `%valiant_battlepass_page%` - This placeholder returns the Adventure Pass Menu page that the player is on (the page that contains his current Adventure Pass level)
- `%valiant_battlepass_rewardavailable_LEVEL%` - This placeholder returns "true", if player has an available, unclaimed reward for the specified Adventure Pass level.
- `%valiant_battlepass_dq_timeuntilreset%` - This placeholder returns the time until the Daily Quest resets.
- `%valiant_battlepass_wq_timeuntilreset%` - This placeholder returns the time until the Weekly Quest resets.
- `%valiant_battlepass_dq_timeuntilexpiration%` - This placeholder returns the time until the Daily Quest expires.
- `%valiant_battlepass_wq_timeuntilexpiration%` - This placeholder returns the time until the Weekly Quest expires.
- `%valiant_battlepass_dq_number%` - This placeholder returns the Daily Quest ID number. (used for display purposes in the CP menu)
- `%valiant_battlepass_wq_number%` - This placeholder returns the Weekly Quest ID number. (used for display purposes in the CP menu)
- `%valiant_battlepass_level_progress_percent%` - This placeholder returns the progress towards the next Adventure Pass level in percentage.
- `%valiant_battlepass_level_progress_graphic%` - This placeholder returns the progress towards the next Adventure Pass level in the form of a colored progress bar.
- `%valiant_battlepass_level%` - This placeholder returns the player's Adventure Pass level.
- `%valiant_battlepass_xp%` - This placeholder returns the player's Adventure Pass experience amount.
- `%valiant_battlepass_xp_need%` - This placeholder returns the player's Adventure Pass experience amount needed to level up.
