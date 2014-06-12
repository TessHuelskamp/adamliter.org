---
title: Adam Liter | Blog
layout: blog-default
---
## All Blog Entries

{% for post in site.posts %} {% capture y %} {{post.date | date:"%Y"}} {% endcapture %} {% if year != y %} {% assign year = y %}
### {{ y }}
{% endif %}

{% include blogroll.html %}

{% else %}
<p>There are no blog posts.</p>
{% endfor %}