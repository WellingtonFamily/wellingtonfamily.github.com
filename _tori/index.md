---
layout: post_page
title: "Tori"
---

{% for page in site.tori %}
{% unless page.title == "Tori" %}
  <p>
  <a class="page-link" href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a> -- 
  {{ page.summary | downcase }}
  </p>
{% endunless %}
{% endfor %}
