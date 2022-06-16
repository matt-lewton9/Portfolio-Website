---
layout: project
title: Lunar Thermoelectric Generator NASA MINDS 
when: "2020-2021"
imgFilename: "nasaMain.jpg"
order: 2
---

<img src="{{ "assets/images/nasaMain.jpg" | relative_url }}" class="articleImg">

## Project Overview

NASA MINDS is a national collegiate competition to develop something novel for the Artemis program.
For this competition, we designed and tested a lunar thermoelectric generator system which uses waste heat 
and the natural temperature gradient of lunar regolith to generate electricity on the moon. We recieved NASA funding to construct and test proposed thermoelectric system, and validated our results with thermal simulations. We recieved first place for our technical paper, and fourth place overall.

After the competition, conduted more comperhensive experiements which investgiatd design characteristics of the heat conductor assembly. We presented an expanded paper at IEEE MIT URTC 2021, which was published in <a href="https://ieeexplore.ieee.org/document/9701608" class="link">IEEE Xplore</a>. The paper consists of full documentation of our methods and results, this article is an overview of the engineering side.

## Concept

<img src="{{ "assets/images/HEAT SINK IMAGE" | relative_url }}" class="articleImg">

There is a large temperature difference, between the soil on the moon's surface, and just a few feet underground. This is because lunar soil's thermal conductivity increases with depth as it becomes more compact and dense (like sand at the beach). This project therorized that the lunar soil could be used as a heat sink for thermoelectric generator powered by solar radiation or waste heat from a lunar base.

This is done by extending the cold side of the thermolelectric plates with a copper "radiator cylinder" to reach depths with a high thermal conductivity, which is insulated from the sides.

## Design 

To test this concept experimentally, we built a prototype device and test apparatus to simulate the thermal conditions of the moon by conduting the experiment in a vaccum, providing heat to the surface via radiation, and creating a heat sink in the soil similar to what exists on the moon.

<img src="{{ "assets/images/DEVICE IMG" | relative_url }}" class="articleImg">

The prototype device consisted of thermoelectic generatior modules at the surface, sittig on a modular radiator cylinder assembly, consisting of concentric copper cylinders which could be reconfigured for different experiments. The radiator cylinders were insulated with aerogel and enclosed in a steel pipe.

<img src="{{ "assets/images/BOX IMG" | relative_url }}" class="articleImg">

For the test aparatus, we made the 16"x16"x48" vaccum chamber with 1/2" acrylic sheets, with holes for wires, pipes, and bolts precut by the supplier. The radiative heat source was three  heat lamps that hung above the surface. Our lunar soil simulant was sand, which has the key propety of increasing it's thermal conductivity with depth. Lasty, the "heat sink" was created by water in copper coils cooled at to room temperature by a PID water cooling system. The coils were placed at a depth that simulates the temperature distribution of lunar soil. The exterior of the test apparatus was insulated with fiberlass insulation.

Temperature at {NUMBER} locations was recorded by thermocouples embedded in the sand and protoype device. Temperature data, as well as voltage produced by the thermoelectric generator, were collected by arduino uno, which sent the data to a Raspberry Pi to write it to a CSV.

## Simulation

<img src="{{ "assets/images/SIM IMG" | relative_url }}" class="articleImg">

We used FEA thermal simulation in Fusion 360 to validate our experimental results (I unfortunately did not have Ansys at the time). We also used simulations to design heat sink in a way that would replicate the temperature disribution of lunar soil, and determine the wall thickness of the vaccum chamber.

This was my first exposure to simulations. While Fusion 360 is definitley not a real simulation software, it's all we had access to, and it made learning Ansys for Purdue Space Program feel like a natural transition.