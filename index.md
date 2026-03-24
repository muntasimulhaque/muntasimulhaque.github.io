---
layout: default
title: Muntasim Ul Haque
description: Personal site of Muntasim Ul Haque - Telecommunications professional specializing in submarine cable infrastructure
---

<h4 id="blog-posts">Blog Posts</h4>

{% for post in site.posts %}
* [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}