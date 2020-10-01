# GlobalWarming-![](https://travis-ci.org/nsporillo/GlobalWarming.svg?branch=master) - Supports Minecraft 1.14+
Minecraft Server Java Edition (Spigot) plugin which adds game-changing climate change mechanics.

<a href="https://discord.gg/VR96VvC"><img src="https://discordapp.com/assets/fc0b01fe10a0b8c602fb0106d8189d9b.png" height="50"></a>

Table of Contents
=================

   * [GlobalWarming - <a target="_blank" rel="noopener noreferrer" href="https://camo.githubusercontent.com/259d74d6a1c5d317c8f7b10d09183313da539383/68747470733a2f2f7472617669732d63692e6f72672f6e73706f72696c6c6f2f476c6f62616c5761726d696e672e7376673f6272616e63683d6d6173746572"><img src="https://camo.githubusercontent.com/259d74d6a1c5d317c8f7b10d09183313da539383/68747470733a2f2f7472617669732d63692e6f72672f6e73706f72696c6c6f2f476c6f62616c5761726d696e672e7376673f6272616e63683d6d6173746572" alt="" data-canonical-src="https://travis-ci.org/nsporillo/GlobalWarming.svg?branch=master" style="max-width:100\x;"></a> - Supports Minecraft 1.14 ](#globalwarming------supports-minecraft-114)
      * [Contributing](#contributing)
      * [Builds](#builds)
      * [Overview](#overview)
      * [Purpose](#purpose)
      * [Mechanics](#mechanics)
      * [Challenges](#challenges)
      * [(Planned) Features](#planned-features)
      * [Negative Climate Damages (Sample Model)](#negative-climate-damages-sample-model)
      * [Roadmap](#roadmap)
      * [Related Science of Climate Change](#related-science-of-climate-change)
         * [Atmosphere warms with more CO2 because of Greenhouse Effect](#atmosphere-warms-with-more-co2-because-of-greenhouse-effect)
         * [Atmospheric Energy Budget](#atmospheric-energy-budget)
         * [Impact on Oceans](#impact-on-oceans)
         * [Ecological Niche](#ecological-niche)
      * [Suggestions](#suggestions)


## Contributing
- [Developer Setup](https://github.com/nsporillo/GlobalWarming/wiki/Developer-Setup-and-Installation)
- There is a Kanban board on Github where I'll be prioritizing work, feel free to help work on any of the tasks.
- Pull requests welcome! This is a very new project and I appreciate contributions.

## Overview
+ Adds the concept of greenhouse gases (CO2) in the worlds atmosphere 
+ Furnaces emit CO2 when players smelt items
+ Farmed Animals emit CH4 when they are killed
+ Trees (instantly) absorb CO2 when they grow from a sapling
+ As CO2 levels rise, global temperature rises because of the [Greenhouse Effect](http://hyperphysics.phy-astr.gsu.edu/hbase/thermo/grnhse.html)

## Purpose
+ Ever had the hankering to turn a game meant for fun into an emulator of one of the modern world's toughest challenges?
+ Observe the [Prisoner's Dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma#In_environmental_studies) first hand! 
+ Players are best off when they co-operate and agree to reduce their emissions
+ However, each player typically believes they are better off for themselves to emit as much as they wish. 
+ Avoiding a [Tragedy of the Commons](https://en.wikipedia.org/wiki/Tragedy_of_the_commons) might be fun! If the players don't play nice and end up dealing with the consequences, they might decide to agree to fix the planet. 

## Mechanics 
+ Every furnace burn causes a "Contribution" to emissions with an associated numerical value (based on the model)
+ Every tree growth causes a "Reduction" from emissions with an associated numerical value (based on the model)
+ The global temperature is a function of the net global carbon score. 
+ As the global temperature rises, the frequency and severity of negative climate damages increases.
+ Players can purchase "carbon offsets" which creates a tree-planting bounty for other players to fulfill. 

## Challenges
+ Designing a default model that doesn't quickly destroy worlds
+ Efficiently applying in-game mechanics changes

## Features
+ Scoreboard Integration - Players can compete for carbon neutrality! The worst polluters can be shamed.
+ Economy Integration - Set up tree-planting bounties 
+ Carbon Scorecard - Each player can see their latest carbon footprint trends via the command line.
+ Multi-world - Associate emissions in the end or nether worlds to the primary overworld with ease.
+ Custom Models - The inner numerical workings are as configurable as possible. Set thresholds, probabilities, and distributions.
+ Database storage - Load data on startup, queue DB changes to be done async and at intervals (instead of as they happen, that'd kill performance), and empty queue on shutdown. 
+ Highly configurable - Almost everything will have some degree of configuration to suit your server's needs.
+ Efficient - Despite major mechanics changes and an extensive event listening setup, GlobalWarming is fast.

## Negative Climate Damages (Sample Model)
Higher temps inherit the damages from the lower temps

| Global Temp | Effect 1 | Effect 2 | Effect 3 | Effect 4 |
| ------ | ------------ | ------- | --------|-----------|
| 14.0 C | None | | | |
| 15.0 C | Some mobs spawn less | some mobs spawn more | | |
| 16.0 C | +1 Sea level rise | Some fish die | Ice/Snow stops forming | |
| 17.0 C | +1 Sea level rise | Flora species growth stunted | Aquatic life stops spawning | Ocean flora/fauna die |
| 18.0 C | +1 Sea level rise | Area Potion Effect Clouds | Farm yields lower | Snow/Ice melts |
| 19.0 C | +1 Sea level rise | Forest Fires | Slower Health Regen | Frequent T-Storms | |
| 20.0 C | +1 Sea level rise | Severe Forest Fires | Violent T-Storms | Permanent Slowness Effect |

These are just a sample of the possible effects, these will be configurable and implement randomness and probabilities.

##Method for save earth from global worming
The heat-trapping greenhouse gases are increasing,  global temperature is rising, planet is warming, the glaciers are melting and the sea level is rising. This weather change is drastically affecting wildlife and forests. Yes, global warming is happening due to the greenhouse effect. Some of the contributing factors are burning of fossil fuels, deforestation, livestock production and industrialisation. Consequently, it leads to drought, incessant rainfall, hurricanes, extreme heatwaves and other extreme weather conditions. With these adverse effects of global warming happening across the planet, we need to implement ways to stop global warming and protect the planet.

Recycle more

The aim is to cut down the amount of carbon dioxide released in the environment. If you even recycle half of the waste produced at home, you can save up to 2000 pounds of CO2 every year.

Drive less

Air pollution is one of the major factors that lead to an increase in greenhouse gases. Minimise the use of cars and make use of public transportation. Try walking, biking or carpooling whenever possible. If you reduce the driving hours, you will end up saving one pound of CO2 for every mile.

Plant trees

Deforestation plays an important role in global warming and climatic changes. Planting trees is helpful as they absorb carbon dioxide from the atmosphere and regulate the climate. Hence, there is a dire need to plant more trees because a single tree can absorb one ton of CO2 in its lifetime.

Switch to renewable energy

One of the most effective ways to prevent global warming is to start using renewable energy sources such as solar, geothermal, wind and biomass, and stop using fossil fuels. Use renewable energy resources to supply power to your home.

Use energy-efficient devices

By investing in energy-efficient devices such as bulbs, LED lights or solar-powered shower system, you can reduce the energy consumption and help in the production of clean energy. It is not only the cheapest way to reduce greenhouse gas emissions but it also reduces the amount of carbon dioxide released in the atmosphere.

Use less hot water

Do you know you can save 500 pounds of CO2 per year if you switch to cold showers and stop using hot water to wash clothes? Try installing energy-efficient geysers that consume less energy.

Turn off electronic devices

Ensure turning off your electronic devices such as television, computer, stereo, music player when not in use. This can help in saving fuel that is used to generate electricity which in turn can reduce thousand tons of carbon dioxide released in the atmosphere.

Spread awareness

Speak up about global warming, its consequences, causes and what steps we can take to prevent global warming with your friends, family and colleagues. Use the power of social media to voice out your concerns about climate change.

Save water

Make sure to turn off taps while brushing, go for shorter showers and do not waster water by cleaning your cars or bikes.

By following these easy tips, all of us can play a significant role in reducing carbon dioxide emission and preventing global warming, thus, preserving the planet for future generations.


## Related Science of Climate Change
### Atmosphere warms with more CO2 because of Greenhouse Effect
![Greenhouse Effect](https://i.imgur.com/XsWJGz9.png)
### Atmospheric Energy Budget
+ ![Earth's Global Energy Budget](https://i.imgur.com/aHdJxXc.png)

Source: RIT "Climate Change: Science, Technology, and Policy" lecture slides
### Impact on Oceans
![Oceans](https://i.imgur.com/dJPkYAo.png)

Source: RIT "Climate Change: Science, Technology, and Policy" lecture slides
### Ecological Niche
![Niche](https://i.imgur.com/e6pwXlI.png)
- Species have a temperature range in which they can survive
- Plants also have niches (Sunlight, Temperature, Water, Nutrients, CO2, Soil, vehicle etc)


Source: RIT "Climate Change: Science, Technology, and Policy" lecture slides

## Suggestions 
Feel free to create issues on this GitHub project, or join the discord
