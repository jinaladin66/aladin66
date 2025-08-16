---
title: "Blog"
layout: default
description: "Info Terbaru ALADIN66"
---

<div class="post">
  <h2>Artikel Terbaru</h2>
  <ul>
    {% for post in site.posts limit:8 %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="meta">— {{ post.date | date: "%d %b %Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</div>
