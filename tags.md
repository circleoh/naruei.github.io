---
layout: page
title: Categories
permalink: /cats/
---



{% for tag in site.tags %}
### {{ tag[0] }}
{{ tag[1] | size }} posts
  {% for post in tag[1] %}
 - [{{ post.title }}]({% include relative %}{{ post.url }})
  {% endfor %}
{% endfor %}