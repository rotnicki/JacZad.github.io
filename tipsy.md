---
layout: page
title: Testowanie tipów
---

{% for tip in tips %}
H2><datetime>{{ tip.date }}</time></h2>
<p> {{ tip.text }}</p>
{% if tip.url %}
<a href="{{ tip.url }}">Zobacz</a>
{% endif }}
{% if tip.icon %}
<p>Ikona {{ tip.icon }}</p>
{% endif %}
{% endfor %}