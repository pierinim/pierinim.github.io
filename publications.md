---
permalink: /publications/
title: Publications
---

As a member of the CMS Collaboration (and previously BaBar) I am co-author of more than
2,000 papers. Below are my publications with fewer than 50 authors, taken from
[INSPIRE-HEP](https://inspirehep.net/authors/1021028). See also
[Google Scholar](https://scholar.google.com/citations?user=3vZMAs4AAAAJ) and
[ORCID](https://orcid.org/0000-0003-1939-4268).

### Most cited

<ol>
{% assign top = site.data.publications | sort: "cites" | reverse %}
{% for p in top limit: 10 %}
  <li><a href="{{ p.url }}">{{ p.title }}</a> ({{ p.year }}) — {{ p.cites }} citations</li>
{% endfor %}
</ol>

### Full list

{% assign by_year = site.data.publications | group_by: "year" %}
{% for y in by_year %}
<h4>{{ y.name }}</h4>
<ul>
{% for p in y.items %}
  <li>
    <a href="{{ p.url }}">{{ p.title }}</a><br>
    <small>{{ p.authors }}{% if p.journal != "" %} — <em>{{ p.journal }}</em>{% endif %}{% if p.arxiv != "" %} — arXiv:{{ p.arxiv }}{% endif %} · <a href="{{ p.inspire }}">INSPIRE</a></small>
  </li>
{% endfor %}
</ul>
{% endfor %}
