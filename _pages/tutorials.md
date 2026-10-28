---
layout: page
permalink: /tutorials/
title: tutorials
description: Tutorials with embedded notebooks and/or documentation
nav: true
nav_order: 6
---

## Methods Tutorials
Below are tutorials I wrote for Nellab Methods meetings:

- [Filtering](https://www.pophristic.com/wiki/docs/Preprocessing/Filtering/Filtering.html): An overview of temporal and spatial filtering in MEG data, with separate lessons for each and implementation code.
- [Canonical Correlation Analysis](https://www.pophristic.com/wiki/docs/MEG%20Analyses/Canonical%20Correlation%20Analysis.html): An introduction, mathematical derivation, and sample MEG/EEG implementation of Canonical Correlation Analysis.

## Notebooks

{% assign tutorial_pages = site.tutorials | where: "tutorial", true | sort: "title" %}
{% if tutorial_pages.size > 0 %}
<ul class="post-list">
{% for tutorial in tutorial_pages %}
<li>
<h3><a class="post-title" href="{{ tutorial.url | relative_url }}">{{ tutorial.title }}</a></h2>
{% if tutorial.description %}<p>{{ tutorial.description }}</p>{% endif %}
</li>
{% endfor %}
</ul>
{% else %}
<p>Add a notebook and its short companion page to the <code>_tutorials/</code> folder to list it here.</p>
{% endif %}