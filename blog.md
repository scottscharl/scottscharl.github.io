---
title: Blog
emoji: "&#x2328;"
---
{% for post in site.posts %}
- [**{{ post.title }}**<span> - {{ post.date | date:"%b %e, %Y"}}</span>]({{ post.url }})
   {{ post.excerpt }}
{% endfor %}
