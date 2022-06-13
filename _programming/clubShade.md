---
layout: project
title: Ice Rink Shade
imgFilename: "clubShadeMain.png"
when: "Spring 2021"
order: 6
---
<img src="{{ "assets/images/shadeRender.png" | relative_url }}" style="width:300;height:300px;float:right;padding: 0px 32px 32px 32px">

The Chevy Chase Country Club was considering a partial sun covering for their outdoor ice rink, so I created a simulation of how much of the rink would be shaded over the course of the day at different times of year.

The simulation calculates what portion of the rink is shaded based on the geometry of the rink cover and the position of the sun for every minute from 9am to 4pm, when the sun is the most intense.

It then outputs a graphic showing how the shaded region moves vertically, and illustrates how the covering shades more of the rink during months when the sun is low in the sky.

It also outputs a heat map, showing the distribution of total minutes of shade across the rink.

Using graphics for every day of the ice rink's season, from October to March, I created time lapses, showing how the effectiveness of the shade covering will change over time.

These graphics were used to help the club determine the position and size of the shade covering.

<div class="vids">
<figure class="video_container">
  <video controls="true" allowfullscreen="true">
    <source src="{{ "assets/videos/shade.mp4" | relative_url }}" type="video/mp4">
  </video>
</figure>

<figure class="video_container">
  <video controls="true" allowfullscreen="true">
    <source src="{{ "assets/videos/heat.mp4" | relative_url }}" type="video/mp4">
  </video>
</figure>
</div>

The code is <a href="https://github.com/matt-lewton9/club_shade" class="link">here</a> on github.