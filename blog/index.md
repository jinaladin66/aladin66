---
title: "BERANDA"
layout: default
description: "Artikel terbaru ALADIN66: ramalan, tren angka, dan info hiburan digital."
---

<div class="post">
  <h2>Artikel Terbaru</h2>
  <ul style="list-style:none; padding:0; margin:12px 0">
    {% for post in site.posts limit:8 %}
      <li style="margin:12px 0; padding:12px; border:1px solid rgba(255,255,255,.08); border-radius:12px; background:#14141c">
        <a href="{{ post.url | relative_url }}" style="font-weight:800; color:#fff">{{ post.title }}</a>
        <div class="meta">Terbit: {{ post.date | date: "%d %b %Y" }}</div>
        {% if post.description %}<p style="margin:6px 0 0; color:#b6b6c3">{{ post.description }}</p>{% endif %}
      </li>
    {% endfor %}
  </ul>
</div>
