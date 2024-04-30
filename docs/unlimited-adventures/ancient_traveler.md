---
sidebar_position: 14
title: 'Ancient Traveler'
---



# :briefcase: Ancient Traveler

Ancient Traveler is our custom-made, limited-time offer shop system.
Every day, the Ancient Traveler offers a set of 3 different, unique items that he sells for a hefty price.
His items stock is unique, you cannot purchase them through the regular Buy Shop.



#### How to change Ancient Traveler's items?

In order to change the Ancient Traveler's item stock, you need to go to:\
`unlimited_adventures/AncientTraveler/config.yml`\
This file contains the item tags to the items configured in Command Panels' Ancient Traveler's menu.
That list can be used to add, remove or rename tags.



#### In order to modify the actual items, you need to go to:
`plugins/CommandPanels/panels/ancient_traveler_menu.yml`\
In that file, you will find the 'custom-item' node, that contains all of the items sold by the Ancient Traveler.\
That's the spot in which you can modify them.