---
title: Physics
permalink: /physics/
redirect_from: /projects/
author_profile: true
classes: wide
header:
  overlay_image: /assets/img/banner-physics.jpg
  overlay_filter: rgba(0, 0, 0, 0.35)
  caption: "Image: Daniel Dominguez/CERN"
---

Research projects in particle physics, current and past.

<div class="home-cards">
  {% for post in site.categories.Projects %}
  <a class="home-card" href="{{ post.url | relative_url }}">
    {% if post.header.teaser %}<div class="home-card__img"><img src="{{ post.header.teaser | relative_url }}" alt="" loading="lazy"></div>{% endif %}
    {% if post.label %}<p class="home-label">{{ post.label }}</p>{% endif %}
    <h3>{{ post.title }}</h3>
    <p>{{ post.excerpt | strip_html }}</p>
  </a>
  {% endfor %}
</div>
