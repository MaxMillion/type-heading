---
layout: page
title: Documentation
permalink: /documentation/
menu: true
---
{% for function in site.functions %}
  {% include_relative _layouts/function.html %}
{% endfor %}