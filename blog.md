---
title: Blog
layout: default
emoji: "&#128221;"
---
{% for post in site.posts %}
* [**{{ post.title }}**<span> - </span>{{ post.date | date: "%b %u, %Y" }}]({{ post.url }})
   {{ post.excerpt }}
{% endfor %}
