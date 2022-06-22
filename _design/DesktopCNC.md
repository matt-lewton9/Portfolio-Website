---
layout: project
title: Desktop CNC Mill
when: "Summer-Fall 2022"
imgFilename: "cncMain.png"
order: 1
---

*This project is ongoing.*

## Objective

I am making a desktop cnc mill to machine small aluminum 
parts. I will not be larger than a 3D printer, and I would like to keep the cost around $500.

<div class="imgCptnBox" style="float:right">
<img src="{{ "assets/images/cncMain.png" | relative_url }}" class="articleImgMain">
<figcaption class="articleCaption">V1 "3D Printer Design"<br>electronics box, brackets, and gusset plates not shown.</figcaption>
</div>

The electronics on all versions are the same. I'm using a 500 Watt spindle with a built in ER-11 collet. I am using Nema-17 steppers to drive my 3 axes on 2 mm pitch lead screws. Surprisingly, they are able to handle my expected cutting forces while staying under the stepper drivers' current limit. The stepper drivers are integrated in the control board, which is running GRBL 1.1.

## V1

Version 1 is similar to a 3D printer in design. It was inspired by desktop CNC mills in the $3,000-$5,000 range, like the Carbide 3D Nomad or a Bantam.

This design had the table travel in Y, and the Z axis assembly travel in X above the table. Everything was contained in an aluminum extrusion frame, with 3D printed motor mounts, brackets, and gusset plates. Linear motion was on 12 mm linear rods.

This design had a few large flaws. For one, having the structural frame enclosing the machine made it easy to mount the enclosure, but was not very rigid, and was not an efficient use of aluminum. Linear rods are not the best linear motion system, and can be improved upon. Similar designs, such as the commercial mills listed above, overcome these rigidity issues with solid metal frames and PVC or plexiglass enclosures. Those solutions however, are not within my budget, and are not an efficient use of materials.

## V2

Version 2 is currently in design, but has a few major upgrades from Version 1. 

It is a knee mill configuration, similar to large production CNC mills, with the table moving in X and Y, and the Z axis on a tower. The bed is no longer square, and is rectangular, which minimizes Z axis overhang for rigidity without significantly reducing machining volume.

The linear motion system has been upgraded to linear rails with carriages, and I'm using steel tubing instead of aluminum extrusion, again for rigidity.

I am waiting until I return to campus in the fall to build V2, since I will have access to free steel and a full machine shop.