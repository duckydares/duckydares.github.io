---
title: Projects
layout: archive
permalink: /projects/
author_profile: false
---

## Pending...

This page serves to present all of the various things I've dared to question and investigate. It will be akin to a more in-depth README.md of the projects that are on my Github (for those projecs that have some form of code).

{% include base_path %}

{% for post in site.project.projects %}
  {% include archive-single.html %}
{% endfor %}