---
layout: page
permalink: /tutorials/
title: tutorials
description: Tutorials with embedded notebooks and/or documentation
nav: true
nav_order: 6
---

{% assign tutorial_pages = site.tutorials | where: "tutorial", true | sort: "title" %}
{% if tutorial_pages.size > 0 %}
<ul class="post-list">
{% for tutorial in tutorial_pages %}
<li>
<h2><a class="post-title" href="{{ tutorial.url | relative_url }}">{{ tutorial.title }}</a></h2>
{% if tutorial.description %}<p>{{ tutorial.description }}</p>{% endif %}
</li>
{% endfor %}
</ul>
{% else %}
<p>Add a notebook and its short companion page to the <code>_tutorials/</code> folder to list it here.</p>
{% endif %}