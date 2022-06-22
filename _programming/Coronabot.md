---
layout: project
title: Discord Bots
imgFilename: "coronabotMain.png"
when: "2021-Present"
order: 3
---

<div class="imgCptnBox" style="float:right">
<img src="{{ "assets/images/coronabotMain.png" | relative_url }}" class="articleImgMain">
<figcaption class="articleCaption">Song being queued</figcaption>
</div>

Discord bots are the most fun I've ever had programming. I've written them using the <a href="https://discordpy.readthedocs.io/en/stable/index.html" class="link" target="_blank" rel="noopener noreferrer">discord.py</a> wrapper for the Discord API.

## Coronabot

My main bot is <a href="https://github.com/matt-lewton9/Coronabot" class="link" target="_blank" rel="noopener noreferrer">Coronabot</a>, which is packed with features.

It functions as a music bot with the standard features of playing, queueing, skipping and pausing songs from Youtube, as well as unique features such as looping songs, or queueing a specific portion of an existing youtube playlist.

It also has a built in soundboard, which the user can populate with their own MP3 files, as well as text-to-speech in voice calls for those without microphones. For server admins it has a "manual mode" hidden command, where you can send messages as the bot, usually from a hidden admin channel. Lastly, just for fun, it always monitors text channels to respond with dad jokes. If I said "I'm hungry.", it would say "Hi Hungry, I'm Dad."

## Other Bots

I also made a few smaller bots for niche projects:

ScrapeBot collected messages from a server to get training data for my friend's natural language project. It compiled 100,000+ messages from our server that meet certain requirements into a formatted text file.


<a href="https://github.com/matt-lewton9/Coronabot" class="link" target="_blank" rel="noopener noreferrer">CountBot</a> returns the number of messages sent by each user by date, which allows you to map user activity, which is pretty interesting. 