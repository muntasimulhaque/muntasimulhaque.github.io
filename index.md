---
layout: default
title: Muntasim Ul Haque
---

# Muntasim Ul Haque

I’m a telecommunications professional with over 8 years of experience working on projects that keep people connected.

Right now, I’m working in Bangladesh’s submarine cable systems, ensuring reliable, high-speed networks that reach millions. My work focuses on making sure our networks are resilient, efficient, and ready for the future.

I started my journey with a bachelor degree in Electrical and Electronic Engineering from the Islamic University of Technology, where I got hooked on the challenges of network and memory optimization. That passion has driven my work ever since!

## Links

- [LinkedIn](#)
- [Google Scholar](#)
- [X (formerly Twitter)](#)
- [Email](#)

## Publications

<div class="publication">
  <p><strong>Paper Title 1</strong></p>
  <p class="publication-meta">Journal Name, 2023</p>
  <p>A brief description of the paper or project.</p>
</div>

<div class="publication">
  <p><strong>Paper Title 2</strong></p>
  <p class="publication-meta">Conference Name, 2022</p>
  <p>A brief description of the paper or project.</p>
</div>

## CV

<div class="cv-section">
  <h2>Experience</h2>
  <div class="cv-entry">
    <p><strong>Telecommunications Engineer</strong>, Submarine Cable Systems, Bangladesh</p>
    <p class="cv-date">2017 – Present</p>
    <p>Working on ensuring reliable, high-speed networks for millions. Focusing on resilience, efficiency, and future-readiness of submarine cable systems.</p>
  </div>
</div>

<div class="cv-section">
  <h2>Education</h2>
  <div class="cv-entry">
    <p><strong>Bachelor of Science in Electrical and Electronic Engineering</strong></p>
    <p>Islamic University of Technology</p>
    <p class="cv-date">2013 – 2017</p>
  </div>
</div>

## Blog Posts

<ul class="post-list">
  {% for post in site.posts %}
  <li>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
  </li>
  {% endfor %}
</ul>