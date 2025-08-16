---
title: "Beranda"
layout: default
description: "Selamat datang di ALADIN66 — pusat artikel terbaru, ramalan togel, dan tren hiburan digital terkini."
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
