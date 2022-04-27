---
title: Mood Playlist Generator
layout: archive
permalink: /projects/mood-playlist-generator/-post-1
author_profile: false
---

This is my first post since arriving at the two projects I am attempting to tackle. This project will mainly cover the basics / peripherals that need to be implemented in order for me to implemenent ML algorithms on the resulting datasets.
I think what I did last week was fruitful....it's just a bummer that I didn't accomplish much this week. I'll get better.

To remind us of the intention, the goal of this project is to build an algorithm that generates playlists based on moods selected by end users. In that effect as I outline in the main page I need to connect to my streaming platform's API and complete an O2 Auth challenge. Thank god for [spotipy](). They have already implemented an interface for the Spotify Web API allowing me to bystep the process of setting up an O2 Auth manager. Eventually I want to build my own for the knowledges sakes. Utilizing spotipy I have been able to gather user's (mine) data regarding saved albums and followed artists. This allows me to build a large database with all the music that the user listens to.

(Insert image of spotipy connecting successfully and loading Top 10 artists)

Next, I need to determine how to label all of this data with which mood it falls into the most. I can do this manually and skew this based on my perception or I can based it off of technical aspects such as tempo, # of intruments, etc. (Definitely something that needs to be considered more).

I have decided on an initial set of moods based on a paper from UCB making a claim that through unsupervised learning methods they were able to determine 13 distinct moods that people feel when they are listening to music. Some are definitely not what I would have expected. It's still better than selecting my own set of moods without any real prior knowledge of how to delineate between them.

I'm excited that I have made it to the set of having a construction process for a database, but now the real work actual begins. Cleaning the database and training/testing algorithms on the data to determine what the best learning methods are for this type of endeavor.