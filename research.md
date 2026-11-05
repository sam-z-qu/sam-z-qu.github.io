---
title: Research
permalink: /research/
---

# Research

[Placeholder: one or two sentences on your research areas.]

## Working papers

<ul class="papers">
{% for paper in site.data.papers %}
  <li>
    <p class="paper-title">{% if paper.pdf %}<a href="{{ paper.pdf | relative_url }}">{{ paper.title }}</a>{% else %}{{ paper.title }}{% endif %}</p>
    <p class="paper-meta">{% if paper.coauthors %}With {{ paper.coauthors }}. {% endif %}{% if paper.status %}{{ paper.status }}. {% endif %}{{ paper.year }}</p>
    {% if paper.abstract %}<details><summary>Abstract</summary><p>{{ paper.abstract }}</p></details>{% endif %}
  </li>
{% endfor %}
</ul>
