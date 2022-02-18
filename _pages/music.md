---
title: Music
layout: archive
permalink: /music/
author_profile: false
---

## Pending...

This page will primarily serve as a place to share my playlists. In addition, it'll archive:
- Interesting Music Videos
- Archive ALL of the music I have listened to (convert Spotify Album Song Lists to txt file)

{% include base_path %}

{% for post in site.music %}
  {% include archive-single.html %}
{% endfor %}