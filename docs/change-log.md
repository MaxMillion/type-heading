---
layout: page
title: Change Log
permalink: /change-log/
menu: true
---
{% for changelog in site.collections.changelog.docs reversed %}
{% include_relative _layouts/changelog.html %}
{% endfor %}