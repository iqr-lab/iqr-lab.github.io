---
title: Research
nav:
  order: 1
  tooltip: Published works
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

{% include search-box.html %}

{% include search-info.html %}
{{ site.data["citations"] }}
{% include list.html data="citations" component="citation" style="rich" %}
