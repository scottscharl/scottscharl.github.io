---
title: Who I Follow
layout: default
emoji: "&#128161;"
---
A list of some favorite bloggers, thought leaders, and Twitter accounts.
{% for item in site.data.whoifollow2 %}
## {{ item.category }}
{% for item in item.people %}
{% unless item.enable == false %}
* {% if item.website %}[**{{ item.name }}**]({{ item.website }}){% else %}**{{ item.name }}**{% endif %}{% if item.twitter %} <span>&middot;</span> [@{{ item.twitter}}](https://twitter.com/{{ item.twitter }} "Twitter"){% endif %}<br>{% if item.jobtitle and item.companyname and item.companylink %}{{ item.jobtitle }}, [{{ item.companyname}}]({{ item.companylink }}){% else %}{{ item.jobtitle }}{% if item.location %}<br>{{ item.location }}{% endif %}<br>{% endif %}{% if item.podtitle and item.podlink %}Host, [{{ item.podtitle }}]({{ item.podlink }})<br>{% endif %}{{ item.description }}
{% endunless %}
{% endfor %}
{% endfor %}
