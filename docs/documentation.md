---
layout: page
title: Documentation
permalink: /documentation/
menu: true
---
{% assign settings = site.collections.settings.docs | sort:'weight' %}
{% assign headingFunctions = site.collections.functions.docs | where: 'group', 'Heading' | sort:'weight' %}
{% assign headingMixins = site.collections.mixins.docs | where: 'group', 'Heading' | sort:'weight' %}
## Settings
{% for setting in settings %}
{% include_relative _layouts/setting.html %}
{% endfor %}
## Headings
### Functions
{% for function in headingFunctions %}
{% include_relative _layouts/function.html %}
{% endfor %}
### Mixins
{% for mixin in headingMixins %}
{% include_relative _layouts/mixin.html %}
{% endfor %}