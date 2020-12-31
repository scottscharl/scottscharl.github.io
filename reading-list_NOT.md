---
title: Reading List
layout: default
emoji: "&#128218;"
---
<span>&#11088; Recommended</span>
<h2>In Progress</h2>
<ul>
{% for book in site.data.reading-list %}
  {% if book.year == blank or book.year == nil %}
  <li><b>{% if book.star %}&#11088; {% endif %}{{ book.title }}{% if book.subtitle %}: {{ book.subtitle }}{% endif %}<br>
    <p>by {{ book.author }}<span style="color:silver">{% if book.fiction == true %} &middot; fiction{% else %} &middot; nonfiction{% endif %}{% if book.amazon %} &middot; <a href="{{ amazon }}" style="color:silver">link</a>{% endif %}</span></p>
  </li>
  {% endif %}
{% endfor %}
</ul>
<h2>Completed</h2>
<ul>
{% for book in site.data.reading-list %}
  {% if book.year %}
  <li><b>{% if book.star %}&#11088; {% endif %}{{ book.title }}{% if book.subtitle %}: {{ book.subtitle }}{% endif %}</b><br>
    <p>by {{ book.author }}<span style="color:silver">{% if book.fiction == true %} &middot; fiction{% else %} &middot; nonfiction{% endif %} &middot; {{ book.year }}{% if book.amazon %} &middot; <a href="{{ amazon }}" style="color:silver">link</a>{% endif %}</span></p>
  </li>
  {% endif %}
{% endfor %}
</ul>
