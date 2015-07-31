---
layout: page
title: Dinners
excerpt: "An archive of Geekdinner.be dinners sorted by date."
---

<ul class="post-list">
{% for dinner in site.categories.dinners %} 
  <li><article><a href="{{ site.url }}{{ dinner.url }}">{{ dinner.title }} <span class="entry-date"><time datetime="{{ dinner.date | date_to_xmlschema }}">{{ dinner.date | date: "%B %d, %Y" }}</time></span>{% if dinner.excerpt %} <span class="excerpt">{{ dinner.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
