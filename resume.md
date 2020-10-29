---
title: Resume
layout: default
emoji: "&#128441;"
---
### Professional Experience

{% for item in site.data.resume0 %}

* **{{item.jobtitle}}**<br>
[**{{item.employer}}**]({{item.link}})<span> &middot; </span>{{item.location}}<span> &middot; </span>{{item.start}} to {{item.end}}<br>
{{item.description}}<br>
    {% if item.points.point1 %}- {{item.points.point1}}{% endif %}
    {% if item.points.point2 %}- {{item.points.point2}}{% else %}<br>{% endif %}
    {% if item.points.point3 %}- {{item.points.point3}}{% else %}<br>{% endif %}
<p></p>
{% endfor %}

### Education
* **Bachelor of Arts in History**<br>
[**Hillsdale College**](https://hillsdale.edu)<span> &middot; </span> 2008 to 2012
