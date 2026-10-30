---
permalink: /talks/
title: Talks
---

Seminars, conference talks, lectures and outreach, from my contributions on
[CERN Indico](https://indico.cern.ch/search/?q=Maurizio+Pierini).

{% assign by_year = site.data.talks | group_by_exp: "t", "t.date | date: '%Y'" %}
{% for y in by_year %}
<h4>{{ y.name }}</h4>
<ul>
{% for t in y.items %}
  <li><a href="{{ t.url }}">{{ t.title }}</a> — {{ t.event }} <small>({{ t.date | date: "%-d %b %Y" }})</small></li>
{% endfor %}
</ul>
{% endfor %}
