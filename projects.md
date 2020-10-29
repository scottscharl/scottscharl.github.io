---
title: Projects
layout: default
emoji: "&#128295;"
---
Here are a few things I've built recently. I encourage anyone who's curious to dig in and figure out a new tool or app. Making something that you can share with the world--however simple it may be--is deeply satisfying.
{% for item in site.data.projects %}
* [**{{ item.name }}**]({{ item.link }} "{{ item.name }}")<br>
  {{ item.description }}
{% endfor %}
