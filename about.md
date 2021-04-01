---
title: About Me
emoji: "&#128100;"
layout: default
---
I was born in 1990 and raised in the suburbs of Detroit, Michigan in a family of four: [Jen Scharl](https://jenscharl.com) is my sister. We were blessed to have two parents who were very present in our lives. I consider it a blessing. I attended private school through high school, and undergraduate at [Hillsdale College](https://hillsdale.edu).

After college, I moved to Phoenix, Arizona, after of 2012 I left Michigan and took a job as an assistant teacher

<h2>&#128077; Things I Like</h2>
{% for item in site.data.likes.likes %}<a href="https://www.google.com/search?q={{ item }}" target="_blank"><button>{{ item }}</button></a>
{% endfor %}
<h2>&#128078; Things I Don't Like</h2>
{% for item in site.data.likes.dislikes %}<a href="https://www.google.com/search?q={{ item }}" target="_blank"><button>{{ item }}</button></a>
{% endfor %}
