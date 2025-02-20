---
sidebar_position: 13
title: 'Ambients'
---



# 🔊 **Ambients**

Our ambients system is a powerful mechanic designed specifically for Unlimited Adventures. It's a fully original and custom software.\
It's a system which creates a realistic sound atmosphere based on your surroundings, biome, time of the day and even weather!


## ⚙ How to configure ambients?

We are providing incredibly powerful configuration settings for the ambients.\
Things ambient system can take into account when deciding what sounds should the player hear at the moment:
- Biome,
- Levels (Height - Y position),
- Time of the day
- Weather

You can also adjust:
- Volume,
- Delay,
- Amplitude of delay (a randomization of delay),
- Sound overlapping (you can force sound to never play while other sounds are playing)

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
- Go to `assets/minecraft/sounds/custom/`
- Choose one of the folders, or create your own. Your final destination could be, for example: `assets/minecraft/sounds/custom/effect/`

#### ⚙ Add your sound to the `sounds.json` file.
- Go to `assets/minecraft` folder and open the `sounds.json` file.
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


### ⚙ [Step 2/2] Add sound to the ambients sounds list

#### ➕ Just add your sound configuration to the file
You can find the file in `unlimited_adventures/Ambients/sounds.yml`

An example config:
```
hello:
    sound: hello
    biomes:
    - plains
    delay: 20
```

A more advanced example:
```
hello:
    sound: hello
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