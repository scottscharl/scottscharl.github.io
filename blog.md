---
title: Blog
layout: default
emoji: "&#128221;"
---
{% for post in site.posts %}
- [**{{ post.title }}**<span> - {{ post.date | date:"%b %e, %Y"}}</span>]({{ post.url }})
   {{ post.excerpt }}
{% endfor %}
