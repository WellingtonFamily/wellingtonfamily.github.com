---
layout: default
permalink: /tori/
title: Tori
description: 
---
 <ul class="post-list">
    {% for entry in site.tori reversed %}
      <li>
        <h2><a class="post-title" href="{{ entry.url | prepend: site.baseurl }}">{{ entry.title }}</a></h2>
        <p class="post-meta">{{ entry.date | date: '%B %-d, %Y — %H:%M' }}</p>
        <p>{{ entry.description }}</p>
        <br/>
        <hr/>
      </li>
    {% endfor %}
</ul>