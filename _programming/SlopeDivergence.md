---
layout: project
title: Initial Slope by Divergence
imgFilename: "slopeMain.png"
when: "Spring 2022"
order: 2
---

<img src="{{ "assets/images/slopeMain.png" | relative_url }}" class="articleImgMain">

I developed this matlab algorithm in my ENGR 132 class to find the initial slope of a dataset. I know it's lame to include classwork in a portfolio, but this algorithm is pretty cool, and it performed really well.

The assignment was to find the initial slope of a hundred datasets that had significant noise and outliers. All of the datasets had the same logarithmic shape, where the slope approaches infinity as time approaches 0 from the left. My solution sets a "divergence tolerence" for the maximum acceptable difference between the average slope of two points, then iteratives through sets of points approaching 0 from infinity, finding the difference in average slope until it detects that the curve is above is above the divergence tolerence. By average slope of a point, I mean the slope of a line through that point and the origin. It then returns the average slope at that point as a possible initial 

Once a soltion is found, it is checked for error to see if is acceptable. 



This project is not on Github due to academic integrity rules.