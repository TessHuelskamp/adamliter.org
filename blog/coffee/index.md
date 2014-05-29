---
title: Adam Liter | Blog
layout: blog-coffee
---
## Coffee-Related Blog Entries
{% for post in site.categories.coffee %} {% capture y %} {{post.date | date:"%Y"}} {% endcapture %} {% if year != y %} {% assign year = y %}
### {{ y }}
{% endif %}
<p> <span style="font-weight:900"> {{ post.date | date:"%Y-%m-%d" }} </span> : <a href="{{ post.url }}"> {{ post.title }} </a> </p>
{% endfor %}