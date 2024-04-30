---
sidebar_position: 6
title: 'Branding'
---

# :gem: Branding

Unlimited Adventures comes with it's own branding package.\
While you can keep using the default textures and logos, it's a good idea to make your server look a bit more unique.\
This page will explain how to change the most important branding features of the setup.



### Tablist

Tablist can be edited in the `plugins/TAB/config.yml`
```
header-footer:
  enabled: true
  header:
  - '%animation:ServerName%'
  - ''
  footer:
  - ''
  - ' &f #31ed96Website: %color_server_name_accent%www.unlimited-adventures.com'
  - ''
  - '%valiant_active_boosters%'
  - '%valiant_active_boosters_2%'
```

### Scoreboard

Scoreboard(sidebar) can be edited in the `plugins/TAB/config.yml`

```
scoreboard:
  enabled: true
  toggle-command: /sb
  remember-toggle-choice: true
  hidden-by-default: true
  use-numbers: false
  static-number: 0
  delay-on-join-milliseconds: 0
  respect-other-plugins: true
  scoreboards:
    scoreboard:
      title: '%color_server_name%🔔 %animation:ServerName% %color_server_name%🔔'
      lines:
      - ''
      - '&f[%color_primary_color%&l%player%&f]'
      - ' &fRank: %luckperms_prefix%'
      - ' &fGold: %color_gold%%vault_eco_balance_fixed% &f'
      - ' &fGems: %color_gems%%valiant_premium_currency% &f'
      - ''
      - '  {%color_server_name_accent%}play.unlimitedadventures.com'
```

### MOTD

Server description is handled by our custom-made Adventure Core. It can be modified in the `unlimited_adventures/AdventureCore/motd` (**NOT** in the `plugins/` folder!)

```
motd_line:
    '1': "            §x&6&d&d&4&4&4&lUNLIMITED ADVENTURES &f[§x&a&c&e&6&7&31.20.4&f]"
    '2': "   §x&f&f&c&8&0&0⭐ Ambient Sounds §x&9&0&e&3&4&e🪣 3D Backpacks §x&f&7&4&1&5&4☠ §x&f&7&4&1&5&4Dungeons"
```

### 'ESC' menu logo

#### Modify logo

'ESC' menu logo can be modified using a resource pack.\
You can find the texture of the logo in: `assets/minecraft/textures/custom/icons/title.png`\
Edit this texture to change how the logo looks.

#### Delete logo

If you for some reason want to delete the logo altogether, please go to: `assets/minecraft/lang/en_us.json` and edit the line to your own custom text, or delete the file altogether to revert default behaviour.


