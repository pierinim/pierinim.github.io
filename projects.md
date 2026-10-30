---
title: Projects
permalink: /projects/
author_profile: true
classes: wide
---

Research projects, current and past.

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
