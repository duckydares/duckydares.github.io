---
title: Mood Playlist Generator
layout: default
permalink: /projects/mood-playlist-generator
author_profile: false
---

{% include base_path %}

I love music. Only real heathens can't...  

In that vien, I want to dabble more in the art. Here, I create a process for generating a set of songs from a given mood.

## In-Depth

_Simple Beginnings:_ Given a single mood, $$m$$, and a duration, $$T > 0$$, provide a set, $$P$$, of songs such that $$\smash{m = H(p) \forall p \in P}$$, where $$H$$ is the oracle indicating a song's mood.


### Considerations

To start considering how to tackle this objective I need to first consider a universe of known songs, $$\Omega$$, from which to draw $$P$$. In practical terms, it means I need access to an account with access to a set of songs...aka my own to start. Alternatively, I could scrape the web for artists and then utilize a streaming platform to determine their discography. Then I need to consider a set of moods to classify my songs into...and again the quickest path would be to consider all the moods that Spotify (my main music streaming platform) offers for playlists. From there it's utilizing ML methods to generate such an oracle or it's inverse mapping, $$p \in H^{-1}(m)$$.

_Approach_:
1. Connect to Spotify Web API
2. Generate a dataset based on account library OR web scraping
3. Construct a supervision dataset and perform prelimary data analysis
4. Determine valid types of algorithm to run on the dataset to perform mood generation on
5. Develop algorithms and run algorithm analysis
6. Extend....

### Code

I will be developing online in the repository: [mood-music-generator](https://github.com/duckydares/mood-music-generator)

##

{% include mathjax.html %}

{% for post in site.categories.projects %}
  {% if post.url contains "mood-music-generator" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}