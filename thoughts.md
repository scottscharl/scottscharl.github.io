---
title: Thoughts
layout: default
emoji: "&#128394;"
---
{% for item in site.thoughts %}
* [**{{ item.title }}**]({{ item.url }})
   {{ post.excerpt }}
{% endfor %}
