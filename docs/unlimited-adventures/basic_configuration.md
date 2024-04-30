---
sidebar_position: 6
title: 'Basic Configuration'
---





We have put in a big effort in order to make our setup as easy to configure as possible. Here are a few example features that you can configure:

### :cloud: Rules, Welcome Message, Tips, Chat Prefixes & Colors
Features related to chat are controlled by ChatManager plugin. In order to configure them to your own liking, you should head to:
```plugins/ChatManager/``` folder.
- `AutoBroadcast.yml` - the tips that are sent on chat every 2 minutes.
- `config.yml` - rules, chat prefixes, colors.

### :bookmark_tabs: Scoreboard, Tablist
Scoreboard & Tablist are managed by the TAB plugin. In order to configure these features, you should head to:
```plugins/TAB/config.yml```

### :pen: GUI Menus
You can edit all menus in `plugins/CommandPanels/panels/` folder.

### :earth_americas:  Pre-Generating the World

We suggest you to pre-generate your server's world.
In order to do that, you can use a plugin like [Chunky](https://dev.bukkit.org/projects/chunky-pregenerator/files)\
Pre-generating your world can improve the performance of your server.\
We recommend a world size of 5,000 x 5,000 or 10,000 x 10,000.

### Homes

`/sethome` and `/home` are disabled to increase immersion. Instead, players have to craft Home Teleportation Scrolls if they want to quickly get back to their bases.




