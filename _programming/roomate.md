---
layout: project
title: Roommate Matcher
imgFilename: "roomateMain.png"
when: "Spring 2021"
order: 5
---

<div class="imgCptnBox" style="float:right">
<img src="{{ "assets/images/roomateMain.png" | relative_url }}" class="articleImgMain">
<figcaption class="articleCaption">Roommate compatibility spreadeheet</figcaption>
</div>

I created a survey and python program to create a "compatibility score" for any two possible roommates. It considers over 30 different aspects of a roommate, such as common interests and living habits, etc. 

I distributed it on the Purdue Class of 2025 Discord server and it was used by over 150 students. It helped many people find freshman year roommates, including myself. I even had several people message me saying "Hey, I saw we got a high score on that roommate compatibility sheet".

There was already a spreadsheet circulating on the Discord server where over 100 students filled out information, however, such a large spreadsheet was difficult to analyze  to find roommates you might be similar to.

The program processed the unformatted text in the existing spreadsheet, and compared the similarity of different roommate's entries to create a "compatibility score". It awarded weighted points for similar sleep schedules, music taste, majors, etc. 

The algorithm created bins of common entries, then gave points to rommates who had answers in the same bin. Yes or no questions and numerical answers were the easiest, while very open ended questions like "favorite weekend activity" were harder to categorize and were given less weight.

I later created a google survey that produced formatted data which could be more easily analyzed by the program. I had users check boxes of common activities and music types, and the bin method was only used for the "other" write-in option.

The code is <a href="https://github.com/matt-lewton9/PurdueRoomate-Matcher" class="link" target="_blank" rel="noopener noreferrer">on Github</a>.