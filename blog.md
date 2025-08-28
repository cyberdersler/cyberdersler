---
layout: default
title: Blog
permalink: /blog/
---

<section id="blog" class="wrapper style2 fade-up">
  <div class="inner">
    <h1>📚 Blog Yazıları</h1>
    <p>Son kiber təhlükəsizlik məqalələri və dərslər:</p>

    <ul>
      {% for post in site.posts %}
        <li>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          <small>({{ post.date | date: "%d-%m-%Y" }})</small>
        </li>
      {% endfor %}
    </ul>
  </div>
</section>
