---
sidebar_position: 12
id: premium_store
title: '🛒 Premium Store'
---

import tebex1 from './assets/tebex_premium_currency_1.png';
import tebex2 from './assets/tebex_premium_currency_2.png';


# :moneybag: Premium Store Setup

The **Premium Store** is one of our standout features, designed to enhance your server’s economy and boost player engagement. It’s easy to set up, fully customizable, and comes ready with high-quality items out of the box.

### 🚀 Getting Started

The Premium Store comes **pre-configured** with ready-to-sell items.\
All you need to do is **add premium currency** to your webstore.

----

#### 🛒 How to Add Premium Currency to Your Webstore
Using Tebex as an example:
1. Go to your webstore and create a new package.
2. In the package settings, add the following command to be executed on purchase:
```
/premiumcurrency {username} add 1000
```
<img src={tebex1} alt="Image Description"/>
<img src={tebex2} alt="Image Description"/>

4. Click **Create**, and you’re done!

-----


### 💡 Recommended Premium Currency Packages

We recommend you to use the following Premium Currency packages:
| Gems | Price |
| - | - |
| 1000 Gems | $9.99 |
| 2500 Gems | $19.99 |
| 6000 Gems | $44.99 |

You’re free to adjust prices for your audience, but we recommend keeping similar proportions for better conversion.

-----

### ✨ Giving Players Gems Manually
Want to give a player some Gems? Just run one of these commands in-game:
- `/premiumcurrency [player] add [amount]`
- or the shorter version: `/gems [player] add [amount]`

-----

### 💎 Gems Placeholder

Need to display how many gems a player has?\
Use this placeholder: `%valiant_premium_currency%`\
It returns the exact number of Gems a player owns.