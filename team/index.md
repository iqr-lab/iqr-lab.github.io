---
title: Team
nav:
  order: 4
  tooltip: About our team
header: images/background_1.jpg
footer: images/background_1.jpg
---

# {% include icon.html icon="fa-solid fa-users" %}Team

We are a team of scientists, superpets and robotic arms.

{% include section.html %}

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ^(?!pi$)" %}
