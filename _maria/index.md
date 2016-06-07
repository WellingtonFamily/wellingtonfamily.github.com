---
layout: index
title: "Maria"
---

{% for page in site.maria %}
{% unless page.title == "Maria" %}
  <p>
  <a class="page-link" href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a> -- 
  {{ page.summary | downcase }}
  </p>
{% endunless %}
{% endfor %}
