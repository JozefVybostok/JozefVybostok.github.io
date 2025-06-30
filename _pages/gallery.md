---
layout: page
title: "Galéria"
permalink: /gallery/
---

Toto je galéria obrázkov z výskumu a terénnych meraní.

{% for file in site.static_files %}
  {% if file.path contains 'assets/img/gallery' %}
  <img src="{{ site.baseurl }}{{ file.path }}" width="300" alt="Foto"/>
  {% endif %}
{% endfor %}
