---
title: Projects
permalink:
layout: default
emoji: "&#128295;"
---
{% for item in site.projects %}
* [**{{ item.title }}**]({{ item.url }})
   {{ post.excerpt }}
{% endfor %}
