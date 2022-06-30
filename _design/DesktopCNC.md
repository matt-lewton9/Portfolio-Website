---
layout: project
title: Desktop CNC Mill
when: "Summer 2022"
imgFilename: "cncMain.png"
order: 1
---

## Overview

Over the summer of 2022, I set out to make my own desktop CNC mill to machine small aluminum parts. Originally, I wanted it to be about the size of a 3D printer, cost around $500. However, after researching similar projects and a few design iterations, I realized that I couldn't really make a machine worth $500 for $500. My costs are also way higher off campus during the summer without access to a full machine shop and all the free aluminum and steel I could want. 

Although nothing was built, designing these mills was very fun, and a valuable experience. This was my first time designing specifically for rigidity, which was a new way of thinking about a design for me. The electronics and control side of this project was also completely foreign to me, so designing the system and sourcing components was tough, but necessary exposure. This was also a trial-by-fire initiation to Solidworks, which I love, and is now my preferred CAD package. The assembly all parts were defined by master sketches in the front, right, and top planes. This method was very robust, and it's how I'm doing all my assemblies from now on.

The right way to do this project, is to make something significantly larger for $3,000-$5,000, which would also be capable of cutting steel. I would like to attempt this before I graduate and lose access to the machine shop. 

<div class="imgCptnBox" style="float:right">
<img src="{{ "assets/images/cncMain.png" | relative_url }}" class="articleImgMain">
<figcaption class="articleCaption">V1 "3D Printer Design"<br>electronics box, brackets, and gusset plates not shown.</figcaption>
</div>

The electronics on all versions are the same. I was using a 500 Watt spindle with a built in ER-11 collet. I was using Nema-17 steppers to drive my 3 axes on 2 mm pitch lead screws. Surprisingly, they are able to handle my expected cutting forces while staying under the stepper drivers' current limit. The stepper drivers are integrated in the control board, which is running GRBL 1.1.

## V1

Version 1 is similar to a 3D printer in design. It was inspired by desktop CNC mills in the $3,000-$5,000 range, like the Carbide 3D Nomad or a Bantam.

This design had the table travel in Y, and the Z axis assembly travel in X above the table. Everything was contained in an aluminum extrusion frame, with 3D printed motor mounts, brackets, and gusset plates. Linear motion was on 12 mm linear rods.

This design had a few large flaws. For one, having the structural frame enclosing the machine made it easy to mount an enclosure, but it was not very rigid, or efficient use of aluminum, since the frame struts were unnecessarily large. Second, linear rods are not the mopst rigid linear motion system, althpugh they are cheap. Similar designs, such as the commercial mills listed above, overcome these rigidity issues with steel frames, and PVC or steel enclosures. Those solutions however, are not within my budget (at least off campus), and are not an efficient use of materials.

## V2

Version 2 has a few major upgrades from Version 1. 

It is a knee mill configuration, similar to large production CNC mills, with the table moving in X and Y, and the Z axis on a tower. The bed is no longer square, and is rectangular, which minimizes Z axis overhang for rigidity without significantly reducing machining volume.

The linear motion system has been upgraded to linear rails with carriages, and I'm using steel tubing instead of aluminum extrusion, again for rigidity.