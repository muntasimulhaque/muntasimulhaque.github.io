---
layout: default
title: Muntasim Ul Haque
description: Personal site of Muntasim Ul Haque - Telecommunications professional specializing in submarine cable infrastructure
---

## About Me

[Previous content remains exactly the same...]

---

## Blog Posts

{% for post in site.posts %}
* [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

[Rest of your content remains the same...]