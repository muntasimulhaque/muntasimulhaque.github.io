---
layout: default
title: Blogs
permalink: /blogs/
---

# Blog Posts

<div class="blog-list">
    {% raw %}{% for post in site.posts %}
    <article class="blog-preview">
        <h2 class="blog-title">
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h2>
        <time class="blog-date">{{ post.date | date: "%B %-d, %Y" }}</time>
    </article>
    {% endfor %}{% endraw %}
</div>