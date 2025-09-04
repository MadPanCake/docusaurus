---
sidebar_position: 13
title: '🔊 Ambients'
---



# 🔊 **Ambients**

The Ambients system is a core feature of Unlimited Adventures, built entirely in-house as a custom software solution.\
It dynamically creates immersive soundscapes that respond to your environment—whether it’s the biome you’re in, the time of day, your altitude, or even the weather—bringing the world to life around you.


## ⚙ Configuring Ambients

Our system comes with powerful configuration options, giving you full control over how ambients behave.\
When deciding which sounds to play, the system can factor in:
- Biome
- Altitude (Y position) [`sky`, `surface` or `underground`]
- Time of the day [`morning`, `noon`, `evening` and `night`]
- Weather [`clear`, `rain`, `thunder`]

Additional adjustable settings include:
- Volume
- Delay (time between sounds)
- amplitude (adds randomness to delay for more natural variation)
- Prevent Stacking (avoids overlapping by ensuring only one ambient sound plays at a time)

**Here's an example sound config:**
```
yellowstone_elk:
    sound: ambient.elk
    biomes:
    - t:yellowstone
    levels:
    - surface
    time_of_day:
    - morning
    - noon
    - evening
    weather:
    - clear
    - rain
    delay: 120
    amplitude: 50
    prevent_stacking: 5
    volume: 0.5
```




## ➕ How to add new sounds?

Adding new sounds is very straightforward. Simply add the sound to the resource pack and update the configuration files!

### 🎨 [Step 1/2] Add sound to the resource pack

#### ✅ Ensure your sound is properly saved:
- Ensure your sound is in the .ogg format (Minecraft doesn't support other formats!).
- Directional Sound: Make it MONO.
- Non-Directional Sound ('plays in your head'): Make it STEREO.

#### ⬆️ Now we need to upload your sound into the [resource pack](resource-pack).
- Go to 📁`assets/minecraft/sounds/custom/`
- Choose one of the folders, or create your own. Your final destination could be, for example:\
📁`assets/minecraft/sounds/custom/effect/`

#### ⚙ Add your sound to the `sounds.json` file.
- Go to 📁`assets/minecraft` folder and open the `sounds.json` file.
- Add your sound to the list. Let's assume your sound name is `hello.ogg`

```
"custom.hello" : {
	"sounds":[
		"custom/effect/hello"
	]
},
```

If you'd like to have multiple sound variants that will be chosen at random, do this:

```
"custom.hello" : {
	"sounds":[
	        "custom/effect/hello_1",
                "custom/effect/hello_2",
                "custom/effect/hello_3"
	]
},
```

Please notice how the last sound doesn't have a comma at the end. It's important!


#### 🔍 Testing Your Sound

Before moving on, make sure your sound works correctly in the resource pack.\
You can test it quickly with the command:\
`/playsound <sound_name>`\
For example: `/playsound minecraft:entity.experience_orb.pickup`


### ⚙ [Step 2/2] Add sound to the ambients sounds list

#### ➕ Just add your sound configuration to the file
You can find the file in `unlimited_adventures/Ambients/sounds.yml`

An example config:
```
hello:
    sound: custom.hello
    biomes:
    - plains
    delay: 20
```

A more advanced example:
```
hello:
    sound: custom.hello
    biomes:
    - green biomes
    - high biomes
    - !t: yellowstone
    levels:
    - surface
    - sky
    weather:
    - clear
    delay: 20
    amplitude: 5
    volume: 0.8
```