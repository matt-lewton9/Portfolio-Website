---
layout: project
title: Roommate Matcher
imgFilename: "roomateMain.png"
when: "Spring 2021"
order: 5
---
<img src="{{ "assets/images/roomateMain.png" | relative_url }}" class="articleImgMain">

I created a survey and python program to create a "compatibility score" for any two possible roommates. It considers over 30 different aspects of a roommate, such as common interests and living habits, etc. 

I distributed it on the Purdue Class of 2025 Discord server and it was used by over 150 students. It helped many people find freshman year roommates, including myself. I even had several people message me saying "Hey, I saw we got a high score on that roommate compatibility sheet".

There was already a spreadsheet circulating on the Discord server where over 100 students filled out information, however, such a large spreadsheet was difficult to analyze  to find roommates you might be similar to.

The program analyzed the unformatted text in the existing spreadsheet, and compared the similarity of different roommate's entries to create a "compatibility score". It awarded weighted points for similar sleep schedules, music taste, majors, etc.

I later created a custom survey that produced formatted data which could be more easily analyzed by the program.

The code is <a href="https://github.com/matt-lewton9/PurdueRoomate-Matcher" class="link" target="_blank" rel="noopener noreferrer">on Github</a>.