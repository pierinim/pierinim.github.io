---
title: More
permalink: /more/
header:
  overlay_image: /assets/img/more-banner-zenseact.jpg
  overlay_filter: rgba(0, 0, 0, 0.3)
  caption: "Image: Zenseact"
---

{% for s in site.data.media %}
<h3>{{ s.section }}</h3>
<ul class="media-list">
{% for m in s.items %}
  <li>
    <a href="{{ m.url }}">{{ m.title }}</a>{% if m.lang == "it" %} <small>(in Italian)</small>{% endif %}
    <br><small>{{ m.outlet }}{% if m.year %} · {{ m.year }}{% endif %}</small>
    {% if m.note %}<br>{{ m.note }}{% endif %}
    {% if m.links %}<br><small>{% for l in m.links %}<a href="{{ l.url }}">{{ l.label }}</a>{% unless forloop.last %} · {% endunless %}{% endfor %}</small>{% endif %}
  </li>
{% endfor %}
</ul>
{% endfor %}
