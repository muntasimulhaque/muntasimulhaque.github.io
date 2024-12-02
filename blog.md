---
layout: default
title: Blogs
permalink: /blog/
---

<div class="blog-list">
    {% for post in site.posts %}
    <article class="blog-preview">
        <h3 class="blog-title">
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>
        <time class="blog-date">{{ post.date | date: "%B %-d, %Y" }}</time>
    </article>
    {% endfor %}
</div>