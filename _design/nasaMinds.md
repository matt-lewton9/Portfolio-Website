---
layout: project
title: Lunar Thermoelectric Generator NASA MINDS 
when: "2020-2021"
imgFilename: "nasaMain.jpg"
order: 3
---

<img src="{{ "assets/images/nasaMain.jpg" | relative_url }}" class="articleImgMain">

## Project Overview

NASA MINDS is a national collegiate competition to develop something novel for the Artemis program.
For this competition, we designed and tested a lunar thermoelectric generator system which uses waste heat 
and the natural temperature gradient of the lunar regolith to generate electricity on the moon. We received NASA funding to construct and test the proposed thermoelectric system, and validated our results with thermal simulations. We received first place for our technical paper, and fourth place overall.

After the competition, conducted more comprehensive experiments which investigated design characteristics of the heat conductor assembly. We presented an expanded paper at IEEE MIT URTC 2021, which was published in <a href="https://ieeexplore.ieee.org/document/9701608" class="link" target="_blank" rel="noopener noreferrer">IEEE Xplore</a> and is public on <a href="https://arxiv.org/abs/2107.12583" class="link" target="_blank" rel="noopener noreferrer">arXiv</a>.

## Concept

There is a large temperature difference, between the soil on the moon’s surface, and just a few feet underground. This is because lunar soil’s thermal conductivity increases with depth as it becomes more compact and dense (like sand at the beach). This project theorized that the lunar soil could be used as a heat sink for a thermoelectric generator powered by solar radiation or waste heat from a lunar base.

This can be done by extending the cold side of the thermoelectric plates with a copper "radiator cylinder" to reach depths with a high thermal conductivity, which is insulated from the sides.

<img src="{{ "assets/images/teg.png" | relative_url }}" class="articleImg" style="float:left;height:300px">

## Design 

To test this concept experimentally, we built a prototype device and test apparatus to simulate the thermal conditions of the moon by conducting the experiment in a vacuum, providing heat to the surface via radiation, and creating a heat sink in the soil similar to what exists on the moon.

The prototype device consisted of thermoelectric generator modules at the surface, sitting on a modular radiator cylinder assembly, consisting of concentric copper cylinders which could be reconfigured for different experiments. The radiator cylinders were insulated with aerogel and enclosed in a steel pipe.

<img src="{{ "assets/images/testRig.png" | relative_url }}" class="articleImg">

For the test apparatus, we made the 16”x16”x48” vacuum chamber with 1/2” acrylic sheets, with holes for wires, pipes, and bolts cut by the supplier. The radiative heat source was three heat lamps that hung above the surface. Our lunar soil simulant was sand, which has the key property of increasing its thermal conductivity with depth. The “heat sink” was created by water in copper coils cooled to room temperature by a PID water cooling system. The coils were placed at a depth that simulates the temperature distribution of lunar soil.

Temperature at {NUMBER} locations was recorded by thermocouples embedded in the sand and prototype device. Temperature data, as well as voltage produced by the thermoelectric generator, were collected by Arduino Uno, which sent the data to a Raspberry Pi to write it to a CSV.

## Simulation

We used FEA thermal simulation in Fusion 360 to validate our experimental results. We also used simulations to design a heat sink in a way that would replicate the temperature distribution of lunar soil, and determine the wall thickness of the vacuum chamber.

This was my first exposure to simulations. While Fusion 360 is definitely not a real simulation software, it's all we had access to, and it made learning Ansys for Purdue Space Program feel like a natural transition.
