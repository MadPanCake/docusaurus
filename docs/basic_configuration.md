---
sidebar_position: 8
title: 'Basic Configuration'
---


# ⚙️ Basic Configuration


We have put in a big effort in order to make our setup as easy to configure as possible. Here are a few example features that you can configure:

### :cloud: Chat System
Features related to chat are controlled by our built-in Chat system. In order to configure them to your own liking, you should head to:
📁`unlimited_adventures/Chat/` folder.
- `config.yml` - allows you to enable specific features.
- `auto-broadcast.yml` - the tips that are sent on chat every 2 minutes.
- `banned-words.yml` - words that will be censored and eventually punished.
- `messages-of-mild-concern.yml` - contains humoristic messages that will completely replace toxic chat messages sent by your players.
- `chat-format.yml` - private message format.
- `messages.yml` - contains various strings that you can translate.


### :bookmark_tabs: Scoreboard, Tablist
Scoreboard & Tablist are managed by the TAB plugin. In order to configure these features, you should head to folder\
📁`plugins/TAB/config.yml`

### :pen: GUI Menus
You can edit all menus in 📁`plugins/CommandPanels/panels/` folder.

### :earth_americas:  How to move the Spawn?

In order to move the spawn, you need to:
- Move the spawn location with `/setspawn`
- Move the NPC's with `/npc select` and then `/npc movehere`
- Move the holograms with `/dh movehere name`
- Move the Wilderness Portal with `/rg redefine wild_tp`
- Optionally: Move the bounce pad with `/rg redefine jump_pad`
- Optionally: Move the Sculk Portal by simply placing it in the new place using Portal Stone item.




