---
layout: page
title: Documentation
permalink: /documentation/
menu: true
---
{% for function in site.functions limit:1 %}
  {% include_relative _layouts/function.html %}
{% endfor %}