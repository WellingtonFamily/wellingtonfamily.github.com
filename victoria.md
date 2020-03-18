---
layout: page
permalink: /victoria/
title: Victoria
nav: false
---

{% for i in site.victoria %}

<div class="project"> 
    <div class="thumbnail">
        <a href="{{ i.url }}">
        {% if i.thumbnail %}
        <img class="thumbnail" src="{{ site.assets }}{{ i.thumbnail }}?nf_resize=smartcrop&w=250&h=250"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}
        <span>
            <h1>{{ i.title }}</h1>
            <br/>
            <p>{{ i.description }}</p>
        </span>
        </a>
    </div>
</div>


{% endfor %}
