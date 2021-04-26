---
title: Hello!
layout: default
emoji: "&#128075;"
---
I'm a husband and dad from Colorado.

I started building this site in August 2019 as part of my personal commitment to "rigorous leisure." Soon, curiosity turned to fascination. In early 2021 I decided to quit my job and commit to a career building software.



Connect with me via [Twitter](https://twitter.com/scott_scharl) or [email](mailto:hello@scottscharl.com). Thank you for visiting!

## What I'm working on currently:

* [Blogging](/blog) here on my site.

* My [Projects](/projects) page.

<h2>&#128077; Things I Like</h2>
{% for item in site.data.likes.likes %}<a href="https://www.google.com/search?q={{ item }}" target="_blank"><button>{{ item }}</button></a>
{% endfor %}
<h2>&#128078; Things I Don't Like</h2>
{% for item in site.data.likes.dislikes %}<a href="https://www.google.com/search?q={{ item }}" target="_blank"><button>{{ item }}</button></a>
{% endfor %}
