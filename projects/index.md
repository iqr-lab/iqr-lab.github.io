---
title: Projects
nav:
  order: 2
  tooltip: Software, datasets, and more
---

# {% include icon.html icon="fa-solid fa-wrench" %}Projects

IQR Lab is dedicated to open-sourcing our software and infrastructure. We aim to maintain several packages, applications, datasets, and benchmarks to enable the broader robotics community to build upon our work.

{% include tags.html tags="publication, resource, website" %}

{% include search-info.html %}


{% assign data = site.projects
  | default: site["projects"]
  | default: emptyarray
%}


{% for d in data %}
  {% assign mod = forloop.index | modulo: 2 %}
  {% if mod == 0 %}
    {% assign flip-val = true %}
  {% else %}
    {% assign flip-val = false %}
  {% endif %}

  {{ " " }}
  {% capture text %}

  {{ d.description }}
  {%
    include button.html
    link=d.url
    text=d.button-text
    icon="fa-solid fa-arrow-right"
    flip=true
  %}

  {% endcapture %}

  {%
    include feature.html
    image=d.image 
    link=d.url
    title=d.title
    text=text
    flip=flip-val
  %}

{% endfor %}

