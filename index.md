
---
layout: home
title: Βιογραφικά
---

Καλωσήρθες! Παρακάτω θα βρεις τα βιογραφικά των φοιτητών.

<ul>
{% for p in site.data.people %}
  <li><a href="{{ p.url | relative_url }}">{{ p.name }}</a></li>
{% endfor %}
</ul>
