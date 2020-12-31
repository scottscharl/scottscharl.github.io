---
title: Reading List
layout: default
emoji: "&#128218;"
recommend_emoji: "&#128077;"
---
<span>{{ page.recommend_emoji }} </span>Recommended
## In Progress:
{% for item in site.data.reading-list %}
{% if item.year == blank or item.year == nil %}
- {% if item.star %} <span>{{ page.recommend_emoji }}</span> {% endif %}{%if item.amazon and item.subtitle %}[**{{ item.title }}: {{ item.subtitle}}**]({{ item.amazon }}){% else %}[**{{ item.title }}**]({{ item.amazon }}){% if item.subtitle %}: **{{item.subtitle }}** {% endif %}{% endif %}<br>
  by {%if item.authorlink %}[{{ item.author}}]({{ item.authorlink }} "{{ item.author}}'s site")
  {% else %}{{ item.author }}{% endif %}<span style="color:silver">&middot; {% if item.fiction == true %}fiction{% else %}nonfiction{% endif %}</span>
{% endif %}
{% endfor %}
## Completed in 2020:
{% for item in site.data.reading-list %}
  {% if item.year == 2020 %}
  - {% if item.star %} <span>{{ page.recommend_emoji }}</span> {% endif %}{%if item.amazon and item.subtitle %}[**{{ item.title }}: {{ item.subtitle}}**]({{ item.amazon }}){% else %}[**{{ item.title }}**]({{ item.amazon }}){% if item.subtitle %}{% endif %}{% endif %}<br>
    by {%if item.authorlink %}[{{ item.author}}]({{ item.authorlink }} "{{ item.author}}'s site")
    {% else %}{{ item.author }}{% endif %}<span style="color:silver">&middot; {% if item.fiction == true %}fiction{% else %}nonfiction{% endif %}</span>
  {% endif %}
{% endfor %}
## Completed in 2019:
{% for item in site.data.reading-list %}
  {% if item.year == 2019 %}
  - {% if item.star %} <span>&#11088;</span> {% endif %}{%if item.amazon and item.subtitle %}[**{{ item.title }}: {{ item.subtitle}}**]({{ item.amazon }}){% else %}[**{{ item.title }}**]({{ item.amazon }}){% if item.subtitle %}{% endif %}{% endif %}<br>
    by {%if item.authorlink %}[{{ item.author}}]({{ item.authorlink }} "{{ item.author}}'s site")
    {% else %}{{ item.author }}{% endif %}<span style="color:silver">&middot; {% if item.fiction == true %}fiction{% else %}nonfiction{% endif %}</span>
  {% endif %}{% endfor %}
