---
layout: page
title: Testowanie tipów
---


{% for t in tip %}
<H2><datetime>{{ t.date }}</datetime></h2>
<p> {{ t.text }}</p>
{% if tip.url %}
<a href="{{ t.url }}">Zobacz</a>
{% endif %}
{% if t.icon %}
<p>Ikona {{ t.icon }}</p>
{% endif %}
{% endfor %}