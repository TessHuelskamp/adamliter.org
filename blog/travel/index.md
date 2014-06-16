---
title: Adam Liter | Blog
layout: default
nav_child: 3
nav_node: travel
---
## Travel-Related Blog Entries

{% for post in site.categories.travel %} {% capture y %} {{post.date | date:"%Y"}} {% endcapture %} {% if year != y %} {% assign year = y %}
### {{ y }}
{% endif %}

{% include blogroll.html %}

{% else %}
<p>There are currently no blog posts in the <code>travel</code> category.</p>
{% endfor %}