---
title: Hello!
layout: default
emoji: "&#128075;"
separator: "&middot;&middot;"
---
I'm a husband and dad (now of 2!) from Colorado. On this site I share projects I've built and point others to fascinating people and ideas.

I started building this site in August 2019 as part of my personal commitment to "rigorous leisure." My goal is to spend as much time as I can building little projects that I share with the world.

If you'd like to connect, I'm available on [Twitter](https://twitter.com/scott_scharl) or [email](mailto:hello@scottscharl.com). If you'd like to support my work, you can [buy me a coffee](https://buymeacoffee.com/scottscharl)! Thank you for visiting!

## What I'm working on currently:
* Setting up Career Blues, my podcast about the meaning of work and the Good Life.

* Taking an intro. to JavaScript course at [Codecademy](https://www.codecademy.com/courses/introduction-to-javascript).

* Increasing engagement for [QuoteBot](/quotebot), my bot that collects quotes from friends and posts them to [Twitter](https://twitter.com/squotebot).

* Blogging [here](/blog) on my site.

* (more on my [Projects](/projects) page)

<h2>&#128077; Things I Like</h2>
{% for item in site.data.likes.likes %}<a href="https://www.google.com/search?q={{ item }}" target="_blank"><button>{{ item }}</button></a>
{% endfor %}
<h2>&#128078; Things I Don't Like</h2>
{% for item in site.data.likes.dislikes %}<a href="https://www.google.com/search?q={{ item }}" target="_blank"><button>{{ item }}</button></a>
{% endfor %}
