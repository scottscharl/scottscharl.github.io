---
title: Miscellaneous
emoji: "&#128526;"
links:
  - Litany
  - Liturgical-Calendar
  - Stocks
  - Weather
---
Some other pages I've created:
{% for item in page.links %}
- **[{{ item }}](/{{ item | downcase }})**
{% endfor %}
