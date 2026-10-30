---
title: Other projects
permalink: /other-projects/
author_profile: true
classes: wide
---

Work beyond high-energy physics: applying the methods developed for the LHC to autonomous
driving, edge AI and space, often together with industry.

<div class="home-cards">
  {% for post in site.categories.Other %}
  <a class="home-card" href="{{ post.url | relative_url }}">
    {% if post.header.teaser %}<div class="home-card__img"><img src="{{ post.header.teaser | relative_url }}" alt="" loading="lazy"></div>{% endif %}
    {% if post.label %}<p class="home-label">{{ post.label }}</p>{% endif %}
    <h3>{{ post.title }}</h3>
    <p>{{ post.excerpt | strip_html }}</p>
  </a>
  {% endfor %}
</div>
