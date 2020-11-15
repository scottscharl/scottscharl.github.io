---
title: Blog
layout: default_sub
emoji: "&#128221;"
---
{% for post in site.posts %}
* [**{{ post.title }}**<span> - </span>{{ post.date | date: "%b %d, %Y" }}]({{ post.url }})
   {{ post.excerpt }}
{% endfor %}
