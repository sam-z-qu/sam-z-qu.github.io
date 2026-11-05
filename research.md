---
title: Research
permalink: /research/
---

# Research

**Syntax:** movement, agreement, (anti-)locality, binding and reconstruction, finiteness, and clause-size effects.

**Semantics:** negation, event semantics, tense and aspect, temporal logic, modality, and anaphora.

## Working papers and slides

<ul class="papers">
{% for paper in site.data.papers %}
<li>
<p class="paper-title">{% if paper.pdf %}<a href="{{ paper.pdf | relative_url }}">{{ paper.title }}</a>{% else %}{{ paper.title }}{% endif %}</p>
<p class="paper-meta">{% if paper.coauthors %}With {{ paper.coauthors }}. {% endif %}{% if paper.status %}{{ paper.status }}. {% endif %}{{ paper.year }}{% if paper.slides %} · <a href="{{ paper.slides | relative_url }}">Slides</a>{% endif %}</p>
{% if paper.abstract %}<details><summary>Abstract</summary><p>{{ paper.abstract }}</p></details>{% endif %}
</li>
{% endfor %}
</ul>
