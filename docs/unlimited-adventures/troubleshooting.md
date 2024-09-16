---
sidebar_position: 4
title: 'Troubleshooting'
---



# Solving common problems

We understand that sometimes working on your server doesn't go as intended and `stuff breaks`.\
This guide has been made to provide quick help in such situations!


### ⚠️ Make sure your server is properly installed

1. Make sure you have installed the setup according to the 📗 [**installation instructions**](https://endernerds.netlify.app/docs/unlimited-adventures/installation)
2. Make sure you are on 📄 [**Paper 1.20.4**](https://api.papermc.io/v2/projects/paper/versions/1.20.4/builds/497/downloads/paper-1.20.4-497.jar)
3. Make sure you are using the 🟢 [**latest setup version**](https://builtbybit.com/resources/unlimited-adventures-survival-setup.27917/updates)
4. Make sure you are using ☕ [**Java 21**](https://www.oracle.com/pl/java/technologies/downloads/#java21)


#### 🎨 Texture pack doesn't work?

There are a few possible reasons why the texture pack doesn't work on your server.

1. Have you installed Oraxen or ItemsAdder? If yes, then you have to merge the resource pack. Use the respective guides: [Oraxen](Oraxen) [ItemsAdder](ItemsAdder)
2. Check if `force unicode` setting is disabled in your client language settings.
3. Have you made any modifications to the resource pack or models? Your changes can easily break stuff, please revert to the default files and test your changes one by one to find out what causes issues.
4. If you are using Oraxen or ItemsAdder, you have to remove the `modelengine` folder from your resource pack. Did you do it?
5. Do you have problems with models? Try to swap your `ModelEngine` plugin folder and resource pack files with original files from a clean setup installation.
