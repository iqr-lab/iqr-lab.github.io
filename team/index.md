---
title: Team
nav:
  order: 4
  tooltip: About our team
header: images/iqr_background.png
footer: images/iqr_background.png
---

# {% include icon.html icon="fa-solid fa-users" %}Team

We are a team of scientists, superpets and robotic arms.

{% include section.html %}

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: phd" %}
{% include list.html data="members" component="portrait" filters="role: master" %}
{% include list.html data="members" component="portrait" filters="role: ra" %}
{% include list.html data="members" component="portrait" filters="role: undergrad" %}
{% include list.html data="members" component="portrait" filters="role: mascot" %}
