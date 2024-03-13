---
title: Projects
nav:
  order: 2
  tooltip: Software, datasets, and more
---

# {% include icon.html icon="fa-solid fa-wrench" %}Projects

IQR Lab is dedicated to open-sourcing our software and infrastructure. We aim to maintain several packages, applications, datasets, and benchmarks to enable the broader robotics community to build upon our work.

{% include section.html %}

{% include tags.html tags="publication, resource, website" %}

{% include search-info.html %}

## Projects

{% assign data = site.data["projects"]
  | default: site["projects"]
  | default: emptyarray
%}


{% for d in data %}
  {{ " " }}
  {% capture text %}

  {{ d.description }}
  {%
    include button.html
    link="{{ d.link }}"
    text="See our publications"
    icon="fa-solid fa-arrow-right"
    flip=true
  %}

  {% endcapture %}

  {%
    include feature.html
    image="{{ d.image }}"
    link="{{ d.link }}"
    title="{{ d.title }}"
    text=text
  %}

{% endfor %}

