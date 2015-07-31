---
layout: page
title: Meetups 
excerpt: "An archive of Geekdinner.be meetups sorted by date."
search_omit: true
---

<ul class="post-list">
{% for meetup in site.categories.meetups %} 
  <li><article><a href="{{ site.url }}{{ meetup.url }}">{{ meetup.title }} <span class="entry-date"><time datetime="{{ meetup.date | date_to_xmlschema }}">{{ meetup.date | date: "%B %d, %Y" }}</time></span>{% if meetup.excerpt %} <span class="excerpt">{{ meetup.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
