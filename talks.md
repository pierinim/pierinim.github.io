---
permalink: /talks/
title: Talks
---

Seminars, conference talks, lectures and outreach, from my contributions on
[CERN Indico](https://indico.cern.ch/search/?q=Maurizio+Pierini), complemented with earlier
conference talks from INSPIRE proceedings. I have given more than 50 talks at international
conferences, including ICHEP, EPS-HEP and Moriond.

{% assign by_year = site.data.talks | group_by_exp: "t", "t.date | date: '%Y'" %}
{% for y in by_year %}
<h4>{{ y.name }}</h4>
<ul>
{% for t in y.items %}
  <li>{% if t.url != "" %}<a href="{{ t.url }}">{{ t.title }}</a>{% else %}{{ t.title }}{% endif %} — {{ t.event }}
    <small>({% if t.month_only %}{{ t.date | date: "%b %Y" }}{% else %}{{ t.date | date: "%-d %b %Y" }}{% endif %})</small></li>
{% endfor %}
</ul>
{% endfor %}
