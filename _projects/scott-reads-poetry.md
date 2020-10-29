---
title: Scott Reads Poetry
layout: default_notitle
---

[<< back to Projects](/projects)

# {{ page.title }}

I read poems for your enjoyment. This project has been a great way to test my equipment and learn how to produce a podcast using [Anchor.fm](https://anchor.fm/scott-reads-poetry "Anchor.fm"). I'd love to hear your feedback [@scott_scharl](https://twitter.com/scott_scharl) or [hello@scottscharl.com](mailto:hello@scottscharl.com).

If you're enjoying my readings, [buy me a coffee](https://buymeacoff.ee/scottscharl)! Thanks for listening.

{% for item in site.data.scott-reads-poetry %}
**"{{ item.title }}" by {{ item.poet }}**<br>
<iframe src="{{ item.link }}" height="102px" width="350px" frameborder="0" scrolling="no"></iframe>
--
{% endfor %}
