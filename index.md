---
title: adamliter
layout: default
date: 2016-03-20
nav_node: home
---

# /about

I'm currently an MA student in linguistics at Michigan State University. My main research interests in linguistics include syntax, semantics, their interface, and architectural issues more broadly. (For more information, see my [research page][research].)

I **really** like coffee. I worked as a barista, off-and-on, for a few years at the [Dunn Bros at the Smith Douglas More House][DB].

I'm interested in system administration, programming, and web development. I've taught myself some of the basics and plan to learn more.

# /recent-updates

{% assign counter = 1 %}

<ul>
{% for post in site.categories.Updates %}
{% if counter < 6 %}
{% assign counter = counter | plus:1 %}
<li>
  <strong>{{ post.date | date: "%B %d, %Y" }}</strong>
  {{ post.excerpt | remove: '<p>' | remove: '</p>' | strip_newlines | markdownify }}
</li>
{% endif %}
{% endfor %}
</ul>

[research]: {{ site.url }}/research
[DB]: https://www.facebook.com/pages/Dunn-Bros-at-the-Smith-Douglas-More-House/133169107463
