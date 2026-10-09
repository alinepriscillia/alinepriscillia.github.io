---
layout: page
tutorial: true
title: Single-trial clustering tests
description: A walkthrough of group-level significance testing for single-trial MEG results using spatiotemporal clustering.
permalink: /tutorials/single-trial-clustering-tests/
notebook_file: 7,9_Single_trial_clustering_tests.ipynb
---

{% assign notebook_path = page.notebook_file | remove: ".ipynb" | prepend: "/tutorials/" | append: "/" | relative_url %}
<iframe
  src="{{ notebook_path }}"
  title="{{ page.title | escape }} notebook"
  style="display: block; width: 100%; min-height: 900px; border: 0;"
  loading="lazy"
  onload="this.style.height = this.contentWindow.document.documentElement.scrollHeight + 'px';"
></iframe>