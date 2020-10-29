---
title: Blog
layout: default
emoji: "&#128221;"
---

<h1>{{ page.emoji }} {{ page.title }}</h1>
{% for post in site.posts %}
* [**{{ post.title }}**<span> - </span>{{ post.date | date: "%b %d, %Y" }}]({{ post.url }})
   {{ post.excerpt }}
{% endfor %}
<script async data-uid="42d6821210" src="https://motivated-founder-1392.ck.page/42d6821210/index.js"></script>