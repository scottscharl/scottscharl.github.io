---
title: Hello!
layout: default
emoji: "&#128075;"
---
I'm a husband and dad from Colorado.

I started building this site in August 2019 (using [Jekyll](https://jekyllrb.com)) as part of a personal commitment to "rigorous leisure."

Connect with me via [Twitter](https://twitter.com/scott_scharl) or [email](mailto:hello@scottscharl.com). Thank you for visiting!

## What I'm working on currently:

* [Blogging](/blog) here on my site.

* Rebuilding my [wife's website](https://jcscharl.com) using [Ghost](https://ghost.org).

<h2>&#128077; Things I Like</h2>
{% for item in site.data.likes.likes %}<a href="https://www.google.com/search?q={{ item }}" target="_blank"><button>{{ item }}</button></a>
{% endfor %}
<h2>&#128078; Things I Don't Like</h2>
{% for item in site.data.likes.dislikes %}<a href="https://www.google.com/search?q={{ item }}" target="_blank"><button>{{ item }}</button></a>
{% endfor %}
