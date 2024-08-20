---
layout: page
title: Course Content
description: Listing of course modules and topics.
nav_order: 1
---

# Course Content

All Lecture Slides: [link](https://drive.google.com/drive/u/0/folders/1cLsgt4L85JW1wXWJbJDoJZF_fKI113zT)

Full Youtube Playlist: [link](https://youtube.com/playlist?list=PLxh50khjoL6FZ2KtqzdZWx4vBBc5bOW7G&si=Y9vKc7AEUkk3-OTb)

{% for module in site.modules %}
{{ module }}
{% endfor %}
