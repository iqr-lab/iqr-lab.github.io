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

  Our research vision comprises of several core pillars: (a) Reasoning over Multiple Interaction Types, (b) Representing Transfer Problems on a Spectrum of Similarity, (c) Trajectory Adaptation for Tool Transfer, and (d) Human-guided Object Mapping for Task Transfer.

  {%
    include button.html
    link="research"
    text="See our publications"
    icon="fa-solid fa-arrow-right"
    flip=true
    style="bare"
  %}

  {% endcapture %}

  {%
    include feature.html
    image="images/research_banner.png"
    link="research"
    title="Our Research"
    text=text
  %}

{% endfor %}

